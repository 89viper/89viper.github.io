﻿---
title: Github repository와 컴퓨터 local folder 연결하기
categories: programming
tags: Github, Git
---

## 요약<br/>
$ git remote add origin [git repository 주소]

<!-- more -->

# Github repository와 컴퓨터 local folder 연결하기

## 방법
1. Git bash or cmd 창 열기
2. Github repository를 연결할 폴더로 이동(cd 명령어 사용)
3. 해당 폴더에서 Git 초기화<br/>
$ git init
4. 폴더와 repository 연결<br/>
$ git remote add origin https://주소<br/>
- repository 주소는 녹색 버튼(Clone or download) 누르면 확인 가능<br/>
![checkrepoaddress](http://drive.google.com/uc?export=view&id=1u0BziUOtkZfXzkQlGJ_wheZzaHfqYwug)
5. 연결되었는지 확인(1)<br/>
$ git pull origin master<br/>
repository에서 local folder로 파일들을 가져오는 명령어
6. 연결되었는지 확인(2)<br/>
$ git add test.md<br/>
$ git commit -am "new" <br/>
$ git push origin master<br/>
local folder의 변경사항을 repository에 적용시킴

