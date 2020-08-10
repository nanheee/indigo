---
title: "[Python] lv1 - 가운데 글짜 가져오기"
layout: post
date: 2020-08-10 12:31
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Python
star: false
category: blog
author: nanhee
description: Markdown summary with different options
---



### lv1 - 가운데 글짜 가져오기
<https://programmers.co.kr/learn/courses/30/lessons/12903>

#### 내가 푼 풀이
// : 나눗셈 이하를 버리는 연산자
% : 나눗셈 후 나머지를 구하는 연산자

```Python
 def solution(s):
    if len(s) % 2 != 0:
      answer = s[len(s)//2]
    else:
      answer = s[len(s)//2-1]+s[len(s)//2]
    return answer

print(solution("power"))

```



#### 다른 사람의 풀이

```python

def string_middle(str):

    return str[(len(str)-1)//2:len(str)//2+1]

print(string_middle("power"))

```
