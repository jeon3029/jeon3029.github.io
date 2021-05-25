---
title: Github 매일 올리기(잔디밭 깔기) 목표 달성을 위한 모듈 소개(2)
date: 2021-05-25 13:32:00 +0900
categories: github brew plugin
---
- 참고문헌 : [맥에서 1일 1커밋 관리를 효과적으로 하기](https://fernando.kr/develop/2021-02-03-github-jandi-statusbar/)

## 개요
- 저번에 작성했던, [Github 매일 올리기(잔디밭 깔기) 목표 달성을 위한 Plugin](https://jeon3029.github.io/github/make_your_gitbub_green/) 를 보완하고자 글을 작성한다.
- rb 스크립트를 통한 plugin 연동이 일반 사용자들에게는 어려움이 있을 수 있기 때문이다.

## 방법
1. Brew 를 통한 Cask 다운로드
```shell
$ brew update 
$ brew install --cask jandi-statusbar 
```

2. 자신의 Github ID 설정
![image](/assets/images/github_green2.png)

* 위 설정을 모두 마쳤다면 끝이다.
* 비교하고 싶은 상대 ID를 설정하여 비교할 수 있다.