# Step 1 : 계산

### 기능 요구 사항
- 사용자가 입력한 문자열 값에 따라 사칙 연산을 수행할 수 있는 계산기를 구현해야 한다.
- 문자열 계산기는 사칙 연산의 계산 우선순위가 아닌 입력 값에 따라 계산 순서가 결정된다.
    - 즉, 수학에서는 곱셈, 나눗셈이 덧셈, 뺄셈 보다 먼저 계산해야 하지만 이를 무시한다.
    - 예를 들어 "2 + 3 * 4 / 2"와 같은 문자열을 입력할 경우 2 + 3 * 4 / 2 실행 결과인 10을 출력해야 한다.

### Class
- Calculator
- Operators 연산자
    - 사칙 연산 이외의 문자 입력시, 에러
    - 0으로 나눌때 에러
- Operand
- StringConverter
    - 연산자 순사가 잘못 들어왔을 경우, 에러



## Step 2기 : 숫자 클릭

### 기능 요구 사항
- 사용자가 피연산자 0 ~ 9 버튼을 누르면 화면에 해당 숫자가 화면에 보여야 한다.


## Step 3 : 수식

### 기능 요구 사항
- 입력된 피연산자가 없을 때, 사용자가 피연산자 0 ~ 9 버튼을 누르면 화면에 해당 숫자가 화면에 보여야 한다.
 -> 1 클릭 -> 1
5 + -> 1 클릭 -> 5 + 1
- 입력된 피연산자가 있을 때, 기존 숫자 뒤에 해당 숫자가 화면에 보여야 한다. 예를 들면, 8이 입력되어 있을 때 9를 입력하면 89가 보여야 한다.
8 -> 9 클릭 -> 89
- 입력된 피연산자가 없을 때, 사용자가 연산자 +, -, ×, ÷ 버튼을 누르면 화면에 아무런 변화가 없어야 한다.
 -> + 클릭 ->
- 입력된 피연산자가 있을 때, 사용자가 연산자 +, -, ×, ÷ 버튼을 누르면 해당 기호가 화면에 보여야 한다.
1 -> + 클릭 -> 1 +
1 + -> - 클릭 -> 1 -
- 입력된 수식이 없을 때, 사용자가 지우기 버튼을 누르면 화면에 아무런 변화가 없어야 한다.
 -> 지우기 클릭 ->
- 입력된 수식이 있을 때, 사용자가 지우기 버튼을 누르면 수식에 마지막으로 입력된 연산자 또는 피연산자가 지워져야 한다.
32 + 1 -> 지우기 클릭 -> 32 + -> 지우기 클릭 -> 3 -> 지우기 클릭 ->  -> 지우기 클릭 ->
- 입력된 수신이 완전할 때, 사용자가 = 버튼을 누르면 입력된 수식의 결과가 화면에 보여야 한다.
3 + 2 -> = 클릭 -> 5
- 입력된 수신이 완전하지 않을 때, 사용자가 = 버튼을 눌렀을 때 완성되지 않은 수식입니다 토스트 메세지가 화면에 보여야 한다.
3 + -> = 클릭 -> 완성되지 않은 수식입니다
