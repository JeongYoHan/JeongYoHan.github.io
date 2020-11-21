---
layout: post
title: KoreanNewsCrawler 프로젝트에 관하여
description: 프로젝트에 관한 내용
date:   2020-11-22 

---

1.프로젝트 진행사항


팀원 별로 역할을 정했다.

코딩 수정 & 코드 추가 3명

github 관리 1명

정적페이지 관리 2명


코드 수정은 일단 코멘트를 이해하기 쉽게 간단하게 하는 것부터 시작했다.



class SportCrawler:
    def __init__(self):
        self.category = {'야구': "kbaseball", '축구': "kfootball", '농구': "basketball", '배구': "volleyball", '일반 스포츠': "general", 'e스포츠': "esports"}
        self.category = {'야구': "baseball", '축구': "football", '농구': "basketball", '배구': "volleyball", '일반 스포츠': "general", 'e스포츠': "esports"}
        self.selected_category = []
        self.date = {'startyear': 0, 'endyear': 0, 'endmonth': 0}



