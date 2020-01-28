---
title: "[Tableau] 날짜 필터 최근일자순으로 정렬하기"
layout: post
date: 2020-01-23 12:00
image: /assets/images/markdown.jpg
headerImage: false
tag:
- Tableau
- Tableau basic
- Tableau tip
- 태블로
- 태블로기초
- 태블로팁
star: false
category: blog
author: nanhee
description: Markdown summary with different options
---


### 태블로 날짜 필터 최근일자순으로 정렬하기
오늘 포스팅할 내용은 **날짜 필터 최근일자순으로 정렬** 이다.
날짜를 필터로 넣었을 때 최근일자부터 보이게 하려고 한다.

### Sample
Sample은 'Brand', 'Category', 'Date', 'Product', 'Sales'로 구성되어 있으며 'Date'를 [날짜] 형식으로 변환했다.

![](https://github.com/nanheee/nanheee.github.io/blob/master/assets/basic/basic_datesorting_1.png?raw=true)


'계산된 필드 만들기'로 아래와 같이 입력한다.
정렬이 가능하게 Date에서 년/월/일을 별도로 가져와 텍스트 형태로 저장한다.
![](https://github.com/nanheee/nanheee.github.io/blob/master/assets/basic/basic_datesorting_2.png?raw=true)


위에서 만든 필드를 마우스우클릭 하고, 기본속성 > 정렬에 들어간다.
![](https://github.com/nanheee/nanheee.github.io/blob/master/assets/basic/basic_datesorting_3.png?raw=true)


정렬 순서 : 내림차순, 정렬 기준 : 데이터 원본 순서로 한 뒤 확인을 누른다.
![](https://github.com/nanheee/nanheee.github.io/blob/master/assets/basic/basic_datesorting_4.png?raw=true)


필터에 넣으면 아래와 같이 최근일자부터 보이는 것을 확인할 수 있다.
왼쪽 : 변경 전 / 오른쪽 : 변경 후

![](https://github.com/nanheee/nanheee.github.io/blob/master/assets/basic/basic_datesorting_5.png?raw=true)
