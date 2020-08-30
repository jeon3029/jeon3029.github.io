---
title: Markdown 사용법
date: 2020-08-30 23:49:00 -0400
categories: markdown
---
## 1. 개인적인 Markdown에 대한 소회
마크다운 양식을 처음 접하고 사용하게 된지 이제 1년이 다 되어간다. [**Markdown**](https://whatismarkdown.com/)은 텍스트 기반의 마크업 언어로서 문법이 쉽고 단순하고 html과 같은 다른 서식 문서로 쉽게 변환이 가능해서 README파일 등에 자주 사용되곤 한다.<br>
개인적으로는 목차를 쭉 작성해 놓고 의식의 흐름 순서대로 작성하고 적절하게 '#' '-' 들만 붙여주게 되면  예쁘게 변환되기 때문에 디자인적 감각이 무딘 나에게 아주 유용한 에디터 언어다. <br>
또한 github기준으로 READMD파일이 항상 md로 짜여져 있기 떄문에 자신의 github를 잘 포장하고 싶다면 알아두면 좋다.
- 참고 : [위키피디아_마크다운](https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4)
 

## 2. 마크다운 사용법(문법)
### 2.1. 헤더(Header)
- html의 ```<h1>, <h2>...```  과 같다고 생각하면 된다
```
# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
```

# This is a H1
## This is a H2
### This is a H3
#### This is a H4
##### This is a H5
###### This is a H6
- h1을 사용하게 되면 자동으로 밑줄이 그어진다.

### 2.2. 인용(Quote)
- 인용문을 작성할 때 사용한다.(중첩할 수도 있다.)
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

### 2.3 목록(List)
1.  순서있는 목록을 작성한다.
   
  ```
  1. 첫번째
  2. 두번째
  3. 세번째
  ```

  1. 첫번째
  2. 두번째
  3. 세번째
   
2.  순서없는 목록을 작성한다.
  ```
  * 1단계
    - 2단계
      + 3단계
        + 4단계
  ```

* 1단계
  - 2단계
    + 3단계
      + 4단계
- 혼합하여 사용할 수있고 하나만 사용해도 된다.
- 