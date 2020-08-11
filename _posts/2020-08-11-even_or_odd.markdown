---
title: "[Python] lv1 - 짝수와 홀수"
layout: post
date: 2020-08-11
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Python
star: false
category: blog
author: nanhee
description: Markdown summary with different options
---



### lv1 - 짝수와 홀수

정수 num이 짝수일 경우 Even을 반환하고 홀수인 경우 Odd를 반환하는 함수, solution을 완성해주세요.

<https://programmers.co.kr/learn/courses/30/lessons/12937>

#### 내가 푼 풀이
2로 나눴을 때 나머지가 0이면 Even, 아니면 Odd

```python

def solution(num):
    if num % 2 == 0 :
      return "Even"
    else :
      return "Odd"

print("결과 : " + solution(5))

```



#### 다른 사람의 풀이

```python

def evenOrOdd(num):
    if (num%2):
        return "Odd"
    else:
        return "Even"



def evenOrOdd(num):
    return num % 2 and "Odd" or "Even"

```

파이썬은 (num % 2 and "Odd")가 먼저 계산된다.
num이 짝수이면, num % 2 == 0 이 되어 연산식의 결과가 0 and "Odd"이 된다.
0은 False 임으로 이 연산은 False가 되어 or 뒤의 "Even"이 출력된다.

num이 홀수이면, num % 2 == 1 이 되고, 0을 제외한 모든 수는 True 값이므로
True and "Odd"가 되어 "Odd"가 출력된다.
