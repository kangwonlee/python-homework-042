# Coin Denomination Calculator Assignment<br>동전 세기

* Exercise File: `exercise.py`<br>실습 파일: `exercise.py`

## Overview<br>개요

In this assignment, you will write a Python program to calculate the number of coins needed to represent a given amount of currency.<br>이 과제에서는 주어진 통화 금액을 나타내는 데 필요한 동전의 수를 계산하는 Python 프로그램을 작성할 것입니다.

You will use the `//` (floor division) and `%` (modulo) operators to break down the total amount into specific coin denominations: 500, 100, 50, 10, 5, and 1 units.<br>
나눗셈의 몫 `//` 와 나머지 `%` 연산자를 사용하여 입력된 금액에 해당하는 500, 100, 50, 10, 5, 1 단위 동전의 갯수를 계산하세요.
This exercise will help you understand how these operators work and how to apply them in a practical problem.<br>
이 연습은 이러한 연산자의 작동 방식을 이해하고 실제 문제에 적용하는 데 도움이 될 것입니다.

## Objectives<br>목표

* Learn to use the `//` (floor division) operator to determine how many whole times a number fits into another.<br>`//` (나눗셈의 몫) 연산자를 사용하여 한 숫자가 다른 숫자에 몇 번이나 완전히 들어가는지 알아보세요.
* Learn to use the `%` (modulo) operator to find the remainder after division.<br>`%` (나머지) 연산자를 사용하여 나눗셈 후 나머지를 구하세요.
* Practice taking user input and performing calculations in Python.<br>Python에서 사용자 입력을 받고 계산을 수행하는 과정을 연습하세요.
* Develop problem-solving skills by breaking down a total amount into smaller denominations.<br>총 금액을 더 작은 단위로 나누며 문제 해결 능력을 키우세요.

## Problem Description<br>문제 설명
Your task is to create a Python program that:<br>이 과제는 다음과 같은 Python 프로그램을 만드는 것입니다:

1. Prompts the user to enter an amount of currency (an integer).<br>사용자에게 통화 금액(정수)을 입력하라는 메시지를 표시합니다.
1. Calculates how many coins of each denomination (500, 100, 50, 10, 5, and 1) are needed to make up that amount.<br>해당 금액을 구성하는 데 필요한 각 단위 (500, 100, 50, 10, 5, 1) 동전 수를 계산합니다.
1. Prints the number of coins for each denomination.<br>각 단위별 동전 수를 출력합니다.

### Example<br>예시

* Input 입력: 1237
* Output 출력:
  ```
  500: 2
  100: 2
  50: 0
  10: 3
  5: 1
  1: 2
  ```

## Requirements<br>요구 사항

* Use the input() function to get the currency amount from the user (assume it’s a natural number).<br>input() 함수를 사용하여 사용자에게 통화 금액(자연수로 가정)을 입력받으세요.
* Use the `//` operator to calculate the number of coins for each denomination.<br>`//` 연산자를 사용하여 각 단위의 동전 수를 계산하세요.
* Use the `%` operator to calculate the remaining amount after each step.<br>`%` 연산자를 사용하여 각 단계 후 남은 금액을 계산하세요.
* Process the denominations in this order: 500, 100, 50, 10, 5, 1.<br>단위를 다음 순서로 처리하세요: 500, 100, 50, 10, 5, 1.
* Display the results clearly, showing the number of coins for each denomination.<br>각 단위별 동전 수를 알기 쉽게 표시하세요.
* Your program should work for any natural number input.<br>프로그램은 모든 자연수 입력에 대해 작동해야 합니다.

## Hints<br>힌트

* Start with the largest denomination (500) and work your way down to the smallest (1).<br>가장 큰 단위(500)부터 시작하여 가장 작은 단위(1)까지 진행하세요.
* After calculating the number of coins for a denomination, subtract that amount from the total before moving to the next denomination.<br>한 단위의 동전 수를 계산한 후, 다음 단위로 넘어가기 전에 그 금액을 총액에서 빼세요.
* Use variables to keep track of the remaining amount after each step.<br>각 단계 후 남은 액수를 저장하기 위해 변수를 사용하세요.

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
