# String Interpolation with Float Inputs and Formatted Operation Outputs<br>부동 소수점 입력과 형식화된 연산 출력으로 문자열 내삽
* Exercise File: `exercise.py`<br>실습 파일: `exercise.py`
* Get two float values from the keyboard using the `input()` function.<br>`input()` 함수를 사용하여 키보드에서 두 개의 부동 소수점 값을 입력받으세요.
    * Use the following prompts for the `input()`:<br>`input()`에 다음 프롬프트를 사용하세요:
        * `number 0:`
        * `number 1:`
    * Convert the input values to floats using `float()`. The inputs may include decimal numbers (e.g., `3.14`, `-2.5`).<br>`float()`를 사용하여 입력 값을 부동 소수점으로 변환하세요. 입력에는 소수점 숫자가 포함될 수 있습니다 (예: `3.14`, `-2.5`).
* Perform the following arithmetic operations on the two float values:<br>두 개의 부동 소수점 값에 대해 다음 산술 연산을 수행하세요:
    * Addition 덧셈 (`+`)
    * Subtraction 뺄셈 (`-`)
    * Multiplication 곱셈 (`*`)
    * Division 나눗셈 (`/`)
* Display the original variables and the results using **string interpolation** within a `print()` statement for each operation.<br>각 연산에 대해 **문자열 내삽**을 사용하여 원래 변수와 결과를 `print()` 문으로 표시하세요.
    * Before printing the operations, print a horizontal line of 10 dashes (`----------`) to separate the prompts from the output.<br>연산을 출력하기 전에, 프롬프트와 출력을 구분하기 위해 10개의 대시(`----------`)로 된 수평선을 출력하세요.
    * Each line must start with an operation label followed by tab characters (`\t`) to align the equations:<br>각 줄은 연산 레이블로 시작하고, 방정식을 정렬하기 위해 탭 문자(`\t`)가 뒤따라야 합니다:
        * `Addition:\t`
        * `Subtraction:\t`
        * `Multiplication:\t`
        * `Division:\t`
    * Format all numbers (both input values and the result) using a fixed-width, 3-decimal-place format equivalent to `%8.3f`:<br>모든 숫자(입력 값과 결과 모두)에 `%8.3f` 포맷을 적용하세요:
        * Total width of 8 characters (including sign, digits, and decimal point).<br>총 8자 폭 (부호, 숫자, 소수점 포함).
        * Exactly 3 decimal places (e.g., `3.14` becomes `3.140`, `2.5` becomes `2.500`).<br>정확히 3자리 소수점 (예: `3.14`는 `3.140`, `2.5`는 `2.500`).
    * String interpolation must be implemented using one of the following methods:<br>문자열 내삽은 다음 방법 중 하나를 사용하여 구현해야 합니다:
        * f-strings
        * `.format()`
        * `%`
    * Concatenation with `+` as below is **not allowed** and will fail the test.<br>아래와 같이 `+`를 사용한 연결은 **허용되지 않으며** 테스트에서 통과되지 않을 것입니다.
        ```python
        "Addition:\t" + str(num0) + " + " + str(num1) + " = " + str(num0 + num1)
        ```
    * Also using commas (`,`) in `print()` statements for concatenation is **not allowed** and will fail the test.<br>`print()` 문에서 쉼표(`,`)를 사용한 연결 또한 **허용되지 않으며** 테스트에서 통과되지 않을 것입니다.
        ```python
        "Addition:\t", num0, "+", num1, "=", num0 + num1
        ```
* Use only `print()` and `input()` functions in your code.<br>코드에서 `print()`와 `input()` 함수만 사용하세요.
* Example Input<br>입력 예시
```
3.14
2.5
```
* Example Output<br>출력 예시
```
Addition:		3.140 +   2.500 =   5.640
Subtraction:	3.140 -   2.500 =   0.640
Multiplication:	3.140 *   2.500 =   7.850
Division:		3.140 /   2.500 =   1.256
```

## Grading Criteria<br>채점 기준

| Criteria | Points |
|:--------:|:------:|
| Is the code written according to Python syntax?<br>코드가 파이썬 문법에 따라 작성되었는가? | 2 |
| Does the code satisfy the requirements?<br>코드가 요구사항을 충족하는가? | 3 |

``From here is common to all assignments.``

## Submission<br>제출 방법

1. Modify the contents of the `exercise.py` file to write your program.<br>`exercise.py` 파일의 내용을 수정하여 프로그램을 작성합니다.
2. Use the GitHub online editor to commit and push your changes. (See below for detailed instructions)<br>GitHub 온라인 편집기를 사용하여 수정 사항을 커밋하고 푸시합니다. (자세한 사용법은 아래 참조)
3. At the Actions tab of your Github repository, please check the result.<br>깃헙 저장소의 Actions 탭에서 결과를 확인 바랍니다.

## How to Use the GitHub Online Editor<br>Github 온라인 편집기 사용법

* Press the <kbd>.</kbd> key while viewing the files in your repository on GitHub. This will launch a web version of VS Code.<br>저장소의 [Code] 탭을 선택 후 <kbd>.</kbd> 키를 누르면 MS VS Code 의 Web version 이 시작됨
* Make your changes to the `exercise.py` file.<br>`exercise.py` 파일을 수정
* To commit your changes, click on the branch icon on the left sidebar (the third icon after the magnifying glass).<br>수정 사항을 commit 등록 하려면 왼쪽에서 줄 셋 아래 (확대경 다음) 세번째 가지치기 아이콘 선택
* Click the "+" sign next to the filename to stage your changes.<br>파일 이름의 오른쪽 + 기호 선택 (staging)
* Write a brief description of your changes in the text box above.<br>위 빈칸에 변경 사항 설명 입력
* Click "Commit & Push."<br>[커밋 및 푸시] 선택
* Click "Back to Repository" on the branch icon to return to your repository.<br>줄 셋 의 [리포지토리로 이동] 선택하여 저장소로 복귀

## NOTICE REGARDING STUDENT SUBMISSIONS<br>제출 결과물에 대한 알림

* Your submissions for this assignment may be used for various educational purposes. These purposes may include developing and improving educational tools, research, creating test cases, and training datasets.<br>제출 결과물은 다양한 교육 목적으로 사용될 수 있을 밝혀둡니다. (교육 도구 개발 및 개선, 연구, 테스트 케이스 및 교육용 데이터셋 생성 등).

* The submissions will be anonymized and used solely for educational or research purposes. No personally identifiable information will be shared.<br>제출된 결과물은 익명화되어 교육 및 연구 목적으로만 사용되며, 개인 식별 정보는 공유되지 않을 것입니다.

* If you do not wish to have your submission used for any of these purposes, please inform the instructor before the assignment deadline.<br>위와 같은 목적으로 사용되기 원하지 않는 경우, 과제 마감일 전에 강사에게 알려주기 바랍니다.

``Until here is common to all assignments.``
