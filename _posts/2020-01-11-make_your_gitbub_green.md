---
title: Github 매일 올리기(잔디밭 깔기) 목표 달성을 위한 Plugin
date: 2020-08-30 12:32:00 -0400
categories: github
---
- 참고문헌 : [1일1커밋 목표로하기](https://fernando.kr/20)

## 개요
![image](/_posts/images/github_green.png)
- 누구나 github를 잘 관리하는것을 목표로 하지만 생각보다 잘 되지 않는다. 
- 최소한 1일 1커밋을 달성하면서 github와 친숙해지고 이를 잊어버리지 않고자 하는 plugin을 소개하려 한다.(Mac OS 기준)

## 방법
### 1. BitBar download : [BitBar](https://getbitbar.com/)
#### 1.1 Getting Bitbar
```shell
$ brew cask install bitbar
```
- 해당 오픈소스 소프트웨어는 맥 상단 메뉴바에 위치하며 다양한 사용자들이 올려놓은 플러그인을 설치할 수 있다.
  
#### 1.2 Setting Plugin Path
- 사용자가 원하는 위치에 plugin path를 설정할 수 있으며, 해당 폴더에 플러그인 소스가 다운로드 된다.
  
### 2. Github plugin Download
- Link : [Download github plugin](https://getbitbar.com/plugins/Dev/GitHub/github-contribution.10m.rb)
- Add to Bitbar 하게 되면 자동으로 plugin 폴더에 다운로드 된다.
  
### 3. Setting plugin

#### 3.1 .bitbarrc 파일 생성
1. 
   ```shell
   $ vi ~/.bitbarrc
   ```
   - .bitbarrc 파일을 생성해 준다.
2. 
   ```text
   ;# ~/.bitbarrc 
   [github_contribution] 
   username = GITHUB_ID_HERE 
   max_contributions = 10  
   ```
   - username 에 자신의 github id를 입력해 준다

#### 4. 완료
- BitBar 를 referesh 해주게 되면 최근 10일간의 커밋이 되었는지 안되었는지 보이게 되며, 갯수는 옵션(위의 10) 으로 조정할 수 있다.
