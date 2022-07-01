# Javascript-basic-explanation

## JavaScript의 자료형과 Java만의 특성은 무엇일까?

자바스크립트(Javascript)
자바스크립트(Javascript)는 객체(Object)기반의 스크립트 언어입니다.
HTML로는 웹의 내용을 작성하고, CSS로는 웹을 디자인하며, 자바스크립트(JavaScript)로는 웹의 동작을 구현할 수 있습니다. 자바스크립트(JavaScript)는 주로 웹 브라우저에서 사용되는 Node.js와 같은 프레임워크를 사용하면 서버 측 프로그래밍에서도 사용할 수 있습니다.


### 자바스크립트(JavaScript)의 특징
1. 자바스크립트(JavaScript)는 객체 기반의 스크립트 언어입니다.
2. 자바스크립트(JavaScript)는 동적이며, 타입을 명시할 필요가 없는 인터프리터언어입니다.
3. 자바스크립트(JavaScript)는 객체 지향형 프로그래밍과 함수형 프로그래밍을 모두 표현할 수 있습니다.

### 자바스크립트와 자바의 비교

### 자바스크립트 표준
1996년 넷스케이프(Netscape)는 자바스크립트(JavaScript)를 국제 표준안으로 만들기 위해서 ECMA(European Computer Manufacturers Association)에 제출합니다
그 결과 ECMA는 ECMAScript라는 새로운 표준을 제정하였고, 그 첫 번째 버전인 ECMA-262를 1997년에 공표합니다.
ECMAScript는 자바스크립트(JavaScript)뿐 아니라 마이크로소프트의 JScript나 어도비의 액션스크립트도 따르는 국제 표준이 됩니다.
현재 자바스크립트(JavaScript)의 최신 표준은 2015년에 발표된 ECMAScript6입니다.

### 자바스크립트의 자료형
JavaScript의 타입과 자료형 구조

동적 타입
JavaScript는 느슨한 타입(loosely typed)의 동적(dynamic)언어입니다. JavaScript의 변수는 어떤 특정 타입과 연결되지 않으며, 모든 타입의 값으로 할당 및 재할당 가능합니다.

let = foo = 42 // foo가 숫자
foo = "bar"  // foo가 이제 문자열
foo = true // foo가 이제 블리언


원시타입
객체를 제외한 모든 타입은 불변 값(변경 할 수 없는 값)을 정의합니다. 예를 들어 (C 언어와는 달리) 문자열은 불변합니다. 이런 일련의 타입을 "원시값"이라고 합니다.

Boolean 타입
Boolean 타입은 논리요소를 나타내며 true와 false 두가지의 값을 가질 수 있습니다.

Null타입
null타입은 null하나의 값만 가질 수 있습니다.

undefined 타입
값을 할당하지 않은 변수는 undefined 값을 가집니다.

Number타입
ECMAScript는 Number와 BigInt두 가지의 내장 숫자 타입을 가지고 있습니다.
Number 타입은 배정밀도 64비트 이진형식 IEEE 754값(-(2^53 - 1)부터 2^53 - 1까지의 수)입니다. Number 타입은 부동소수점 숫자 외에도 +Infinity, -Infinity, NaN("Not a Number") 세 개의 상징적인 값을 가집니다.
Infinity 범위내에서 가능한 가장 크거나 작은 수를 확인하려면 Number.MAX VALUE와 Number.MIN VALUE 상수를 사용할 수 있습니다.
Number 타입의 값 중 두가지 방식으로 표현할 수 있는 유일한 값으로 0이 있습니다. 0은 -0과 +0 둘다로 표현할 수 있습니다(0은 +0의 별칭입니다)

실제로는 이 사실이 영향을 주는 것은 거의 없습니다. 예컨대 +0 === -0은 참입니다. 그러나 0으로 나눌 경우 둘의 차이를 볼 수 있을 것입니다.

> 42 / +0
Infinity
> 42 / -0
-Infinity

BigInt 타입
BigInt 타입은 임의 정밀도로 정수를 나타낼 수 있는 JavaScript 숫자 원시 값입니다. BigInt를 Number의 안전 한계를 넘어서는 큰 정수도 안전하게 저장하고 연산할 수 있습니다.

BigInt는 정수 끝에 n을 추가하거나 생성자를 호출해 생성할 수 있습니다.

Number의 안전 한계는 Number.MAX SAFE INTEGER로 알아볼 수 있습니다. BigInt의 도입 이후로는 이 한계를 넘는 숫자에 대해 계산이 가능합니다.

다음 예제는 Number.MAX_SAFE_INTEGER 밖으로 나가는 정수에서도 예상된 값을 반환하는 것을 보입니다.

> const X = 2n ** 53n;
9007199254740992n

> const y = x + 1n;
9007199254740993n

#### JavaScript 객체와 불변성이란?

#### 호이스팅과 TDZ는 무엇일까?
