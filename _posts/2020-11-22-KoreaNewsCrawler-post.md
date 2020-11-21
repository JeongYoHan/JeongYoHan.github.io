---
layout: post
title:  "KoreaNewsCrawler 이란"
date:   2020-11-22 
---
2020.11.22
open source software


이 크롤러는 네이버 포털에 올라오는 언론사 뉴스 기사들을 크롤링 해주는 크롤러입니다.
크롤링 가능한 기사 카테고리는 정치, 경제, 생활문화, IT과학, 사회, 세계, 오피니언입니다. 
스포츠 기사같은 경우 야구, 축구, 농구, 배구, 골프, 일반 스포츠, e스포츠입니다.



이 메서드는 수집하려고자 하는 카테고리는 설정하는 메서드입니다.
파라미터에 들어갈 수 있는 카테고리는 '정치', '경제', '사회', '생활문화', 'IT과학', '세계', '오피니언'입니다.
파라미터는 여러 개 들어갈 수 있습니다.
category_name: 정치, 경제, 사회, 생활문화, IT과학, 세계, 오피니언 or politics, economy, society, living_culture, IT_science, world, opinion

set_date_range(startyear, startmonth, endyear, endmonth)

이 메서드는 수집하려고자 하는 뉴스의 기간을 의미합니다. 기본적으로 startmonth월부터 endmonth월까지 데이터를 수집합니다.

start()

이 메서드는 크롤링 실행 메서드입니다.

예시

```phython
from korea_news_crawler.articlecrawler import ArticleCrawler

Crawler = ArticleCrawler()  
Crawler.set_category("정치", "IT과학", "economy")  
Crawler.set_date_range(2017, 1, 2018, 4)  
Crawler.start()
```

 실행 결과
 
 

![image1]https://github.com/20-2-SKKU-OSS/2020-2-OSS-11/blob/gh-pages/_img/article_result.PNG


![sport_resultimg]https://github.com/20-2-SKKU-OSS/2020-2-OSS-11/blob/gh-pages/_img/sport_resultimg.PNG

