#### 수학에 대한 전반적인 정리 Everything (at least for me...) of Math

### 1. 자연수 (natural number)

#### 1.1 거듭제곱 (exponentiation)

```
거듭제곱(exponentiation)은 지수(power)만큼 반복해서 자신을 곱해라는 뜻입니다.
exponentiation is number of self repeat multiply.

예를 들어 2^3은 자신을 3번을 구해라는 의미입니다.
For example, 2^3 means multiply itself 3 times.

2*2를 해서 자신의 값이 4가 되었습니다.
we calculate a 2*2. Now, value of expression is 4.

자신의 현재 값은 4이므로 4*2를 해야 합니다.
current value of expression is 4. so we calculate a 4*2.

그러므로 2^3은 8입니다.
so, 2^3 is 8.

# 자바스크립트를 사용한 생각의 단계의 식
Expression of thinking step using javascript

var x = '2^3'
var number = parseInt(x.substr(0,1))
var power = x.indexOf("^") + 1
var number_of_repeat = x.substr(power)
var result = number;

for(i=1;i<number_of_repeat;i++) {
   result = result * number;
}

console.log(result);
```

### 2. 정수와 유리수 (integer and rational number)

### 3. 일차방정식 (linear equation)

### 4. 좌표평면, 그래프 (coordinate plane, graph)

### 5. 도형의 기초 (the basis of a figure)

### 6. 평면도형 (a plane figure)

### 7. 입체도형 (a solid figure)

### 8. 통계 (statistics)

### 9. 유리수와 근사값 (rational number and approximate value)

### 10. 식의 계산 (the calculation of an expression)

### 11. 연립방정식 (system of equations)

### 12. 부등식 (inequation)

### 13. 확률 (probability)

### 14. 도형의 성질 (properties of shapes)

### 15. 도형의 닮음 (shape resemblance)

### 16. 다항식 (polynomials)

### 17. 방정식과 부등식 (equations and inequalities)

### 18. 도형의 방정식 (equations in shapes)

### 19. 집합과 명제 (sets and propositions)

### 20. 함수 (function)

### 21. 수열 (sequences)

### 22. 지수함수와 로그함수 (exponential and logarithmic functions)

### 23. 1차 함수(linear function)

### 24. 3차 함수 (cubic function)

### 25. 비선형 함수(Nonlinear function)와 활성화 함수(Activation functions)

### 26. MFCC(Mel-Frequency Cepstral Coefficient)

### 27. Fast Fourier Transform

### 28. Filler determine model, Filler classifier model

### 29. 이진 분류 (Binary Classification)

### 30. 로지스틱 회귀 (logistic regression)

### 31. 로지스틱 회귀 경사 하강법(Logistic Regression Gradient Descent)

### 32. 하이퍼 매개변수 (Hyper parameter)

### 33. 순전파 (forward propagation)

### 34. 역전파 (back propagation)

### 35. 브로드캐스팅(Broadcating in Python)

### 36. 벡터화(Vectorization)

### 37. FF 알고리즘 (forward forward algorithm)

#### f(x) = x^3

```
3차 함수인지 판별하는 방법 (다항식이 아닌 경우)

함수의 최고차 항의 차수를 확인하면 된다.
최고차 항의 차수가 n이라고 치면 해당 항은 n항이라고 생각하면 된다.

* 숫자만 있는 항은 상수항이라고 부른다.

1.함수의 계수는 함수의 항의 상수 앞에 있는 숫자이다.
2.x3의 계수는 3이다.
3.차수는 변수가 곱해진 횟수이다
4.x는 3번 곱해졌으므로 (x^3) 차수값은 3이다.
5.^가 없는 상수항의 차수는 1이다 (3x = 3 * x == 1)
6.변수(paramter)가 없다면 차수 값은 0이다.
```

```
3차 함수는 3차 다항 함수이다.
따라서 3차 함수의 그래프는 최대 3개의 근을 가질 수 있다.
즉, 최대 3개의 점과 x축 교차할 수 있다.

복소수 근은 항상 쌍(켤레근)으로 발생하므로 3차 함수는 항상 1개 또는 3개의 실수 0을 갖는다.
*  2개의 실제 0을 가질 수 없음

3차 함수는 차수가 3인 다항 함수며 형식(일반형)은 f(x) = ax3 + bx2 + cx + d과 같다.
a, b, c 및 d는 실수이고 a ≠ 0이다.

기본 3차 함수(parent cubic function)는 f(x) = x 3이다.

3차 함수는 홀수차수 다항식을 포함하므로 적어도 하나의 실근을 갖음

예를 들어 x 3 = 0(x = 0) 을 충족하는 실수는 하나뿐이므로 3차 함수 f(x) = x 3 은 실수 근을 하나만 갖음

* 3차 함수는  모든 대수 함수가 다항 함수 이므로 대수 함수이다.

# 3차 함수의 절편(intercepts)

함수의 절편에는 x 절편과 y 절편의 두 가지 유형이 있다.

함수의 x 절편은 루트 (또는) 0이라고도 한다.
삼차 함수의 차수가 3이므로 최대 3개의 근을 가질 수 있다.

모든 함수의 복소수 근은 항상 쌍으로 발생하므로 함수는 항상 0, 2, 4, ... 복소수 근을 갖음
따라서 함수는 0개 또는 2개의 복소수 근을 가질 수 있다. 그러므로 하나 또는 세 개의 실근 또는 x-절편을 가짐.

3차 함수의 x 절편을 찾으려면 y = 0(또는 f(x) = 0)으로 대체하고 x 값을 구함


f(x) = x3 - 4x2 + x - 4의 절편을 구하려면 f(x) = 0으로 대체해야 한다.
그런 다음 아래와 같은 과정을 거친다.

x3 - 4x2 + x - 4 = 0
x2 (x - 4) + 1 (x - 4) = 0
(x - 4) (x2 + 1) = 0
x - 4 = 0; x2 + 1 = 0
x = 4 ; x2 = -1
x = 4 ; x = ± i

복소수는 x 절편이 될 수 없다.
따라서 f(x)에는 (4, 0)인 하나의 x 절편만 가질 수 있다.

# 3차 함수의 Y 절편
```

```
f(x) = x^3는 3개의 근을 가지는 3차 함수(cubic function)이다.
함수의 근을 구하기 위해서는 이차 공식 (-b² ± √(b² - 4ac)) / 2a을 사용하여 구하여야 한다.

1.x = (-0 ± √(0^2 - 4(1)(0))) / 2(1)
2.x = (0 ± √(0)) / 2
3.x = (0 ± 0) / 2
4.x = 0 / 2
5.x = 0

근의 값 중 하나의 값은 0이다

근의 합은 -b/a와 같다, 즉 b = 0이고 a = 1이므로 근의 합은 -0/1 = 0이다. 
따라서 다른 두 근의 합은 0이 되어야 한다.

x = -1을 함수에 대입하면 f(-1) = (-1)^3 = -1
x = 1을 함수에 대입하면 f(1) = (1)^3 = 1

따라서 함수의 세 근은 x = 0, x = -1 및 x = 1이다
```
