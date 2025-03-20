# Bit Operator Assignment<br>비트 연산자 과제

## Purpose<br>목적:
This assignment helps you explore Python’s bit operators by reading a bit of a specific location from an integer and displaying its binary representation. Let's practice taking user input, using bitwise operations, and formatting output.<br>이 과제는 이진수로 저장된 정수의 특정 위치의 비트를 읽고 그 값을 표시함으로써 Python의 비트 연산자를 이해하는 데 도움이 될 것입니다. 사용자 입력, 비트 연산, 출력 형식을 연습해 봅시다.

Also let's try to understand why almost everything in this class starts from 0 instead of 1.<br>그리고 이 강의에서 왜 대부분의 것이 1이 아닌 0부터 시작하는지 이해해 봅시다.
## Description: <br>설명:
Write a Python program that:<br>다음과 같은 Python 프로그램을 작성하세요:

1. Prompts the user to enter an integer `i` (`0 <= i < 256`).<br>사용자에게 정수 `i` (`0 <= i < 256`)를 입력하라는 메시지를 표시합니다.
1. Prompts the user to enter a bit position `j` (`0 <= j < 8`).<br>사용자에게 비트 위치 `j` (`0 <= j < 8`)를 입력하라는 메시지를 표시합니다.
1. Print a line of 10 dashes (`-`) to separate the input from the output.<br>입력과 출력을 구분하기 위해 10개의 대시(`-`)로 구분된 줄을 출력합니다.
1. Prints the binary representation of `i` as an 8-bit string (e.g., "00000101" for 5).<br>`i`의 이진 표현을 8비트 문자열로 출력합니다 (예: 5의 경우 "00000101").
1. Prints the "bit mask" used in the bit operation to extract the `j`'th bit.<br>`j`번째 비트를 추출하는 데 사용된 "비트 마스크"를 출력합니다.
1. Prints whether the `j`'th bit of `i` is on (hint: comparison operator).<br>`i`의 `j`번째 비트가 켜져 있는지 출력합니다 (힌트: 비교 연산자).

## Instructions:<br>지침:
* Use `input()` to get `i` and `j` from the user. Convert the inputs to integers with int().<br>`input()`을 사용하여 사용자에게 `i`와 `j`를 입력받습니다. 입력값을 `int()`로 정수로 변환합니다.
* To find the `j`'th bit:<br>`j`번째 비트를 찾으려면:
    * Initialize another variable `k` with `1`. Let's call this "bit mask".<br>다른 변수 `k`를 `1`로 초기화합니다. 이 변수를 "비트 마스크" 라고 부릅시다.
    * Shift `k` left by `j` to get a value with only the `j`'th bit set.<br>`j`번째 비트에 설정된 값만을 읽을 수 있도록 `k`를 `j` 만큼 왼쪽으로 이동시킵니다.
    * Whether the bit operation `i & k` result is greater than `0` will tell us if the `j`th bit is on.<br>`i & k` 비트 연산 결과가 `0`보다 큰지 여부로 `j`번째 비트가 켜져 있는지 알 수 있습니다.
* Using f-string, indicate the binary form of `i`. Allocate at least 8 seats and pad the empty seats with `0`.<br>f-string을 사용하여 `i`의 이진 형태를 나타냅니다. 최소 8자리를 확보하고 빈자리는 `0`으로 채웁니다.
* In the same way, print the bit mask used in your bit operation.<br>같은 방식으로 비트 연산에 사용된 비트 마스크를 출력합니다.
* We will not validate input yet.<br>입력이 유효한지는 이 과제에서는 아직 검사하지 않겠습니다.

## 8 Bit Position Table:<br>8 비트 위치 표:
|          | MSB |     |     |     |     |     |     | LSB |
|:---------------------:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
| Bit Position (j)<br>비트 위치 (j) | 7   | 6   | 5   | 4   | 3   | 2   | 1   | 0   |
| Bit Value (for 19)<br>비트 값 (19의 경우)  | 0   | 0   | 0   | 1   | 0   | 0   | 1   | 1   |

MSB = Most Significant Bit (leftmost), LSB = Least Significant Bit (rightmost).<br>MSB = 최상위 비트 (가장 왼쪽), LSB = 최하위 비트 (가장 오른쪽).

## Example Run:<br>실행 예시:

* input
```
Enter an integer (0-255): 19
Enter bit position (0-7): 2
```
* output
```
----------
00010011 : binary representation of 19
00000100 : bit mask for position 2
Is bit of 19 at position 2 on? False
```

## Tips:<br>팁:

* Experiment with different values of `i` and `j` to see how the bits change.<br>`i`와 `j`의 다양한 값을 실험하여 비트가 어떻게 변하는지 확인하세요.
* Use `print()` statements to make your output readable.<br>`print()` 문을 사용하여 출력을 읽기 쉽게 만드세요.
* Ask your instructor if you’re unsure about bit positions.<br>비트 위치에 대해 확신이 없으면 강사에게 문의하세요.

__Happy coding! 즐거운 코딩!__

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
