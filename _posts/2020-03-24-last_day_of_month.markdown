---
title: "[Tableau] 월의 마지막 일자 계산하기"
layout: post
date: 2020-03-24 12:31
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


### Last of Day of Month / 월의 마지막 일자 계산하기
```
DATE(DATEADD('day',-1,DATEADD('month',1,DATETRUNC('month',[Date]))))
```


#### 상세 계산식
```
DATETRUNC('month', [Date])
```
[Date] 에 'month'까지 잘라낸다.
ex) 2020-01-31 → 2020-01-01

```
DATEADD('month', 1, [Date])
```
[Date] 의 'month'에 1 더한다.
ex) 2020-01-01 → 2020-02-01

```
DATEADD('day', -1, [Date])
```
[Date] 의 'day'에 1 뺀다.
ex) 2020-02-01 → 2020-01-31
