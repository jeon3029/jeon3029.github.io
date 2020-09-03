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
```text
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

### 2.3 목록(List)
---
1.  순서있는 목록을 작성한다.<br>
   
  ```text
  1. 첫번째
  2. 두번째
  3. 세번째
  ```

  1. 첫번째
  2. 두번째
  3. 세번째
---
2.  순서없는 목록을 작성한다.<br>
   
  ```text
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

### 2.4 코드

#### 2.4.1 프로그램 소스코드
- "\```" 를 사용하여 앞뒤에 묶으면 코드를 첨부할 수 있다. (예시에서 '\\'는 무시)
```
\ ```cpp
\ #include<iostream>
\ int main(){
\   cout<<"Hello World!";
\   return 0;
\ }
\ ```
```

```cpp
#include<iostream>
int main(){
  cout<<"Hello World!";
  return 0;
}
```

#### 2.4.2 수평선 만들기
- 각 구역별로 나누어 줄 때 사용한다.

```
* * *

***

*****

- - -

---------------------------------------
```

* * *

***

*****

- - -

---------------------------------------

### 2.5 링크
- 링크를 삽입할 때 사용한다.

#### 2.5.1 참조링크
```
[link name][id]
[id]:URL "Optional Title(On Hover)"

// code
Link: [Google][googlelink]
[googlelink]: https://google.com "Go google"
```
- 사용 예
  - Link: [Google][googlelink]

[googlelink]: https://google.com "Go google"

#### 2.5.2 외부링크
```
[Title](link)

//code
[Google](https://google.com, "google link")
```
- 사용 예
  - Link: [Google](https://google.com, "google link")

#### 2.5.3 자동연결
```
일반적인 URL 혹은 이메일주소인 경우 적절한 형식으로 링크를 형성한다.

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>
```

* 외부링크: <http://example.com/>
* 이메일링크: <address@example.com>

### 2.6 강조
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```

* *single asterisks*
* _single underscores_
* **double asterisks**
* __double underscores__
* ~~cancelline~~

> ```문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다.```   
> 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.

### 2.7 이미지 삽입
- img, gif 모두 동일하다
```
![Alt text](/path/to/img.jpg)
![Alt text](/path/to/img.jpg "Optional title")
```

![카카오 라이언](https://t1.kakaocdn.net/kakaocorp/main/kakao10/img/asset03.png)
![카카오 라이언](https://t1.kakaocdn.net/kakaocorp/main/kakao10/img/asset03.png "라이언")

- 사이즈 조절은 html코드 ```<img width="" height=""></img>```를 이용한다.

예
```
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="Kakao Rion"></img><br/>

<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="Kakao Rion"></img>
```

<img src="https://t1.kakaocdn.net/kakaocorp/main/kakao10/img/asset03.png" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="Kakao Rion"></img>

<img src="https://t1.kakaocdn.net/kakaocorp/main/kakao10/img/asset03.png" width="40%" height="30%" title="%(비율) 크기 설정" alt="Kakao Rion"></img>

## 참고

- [참고문헌1 마크다운 사용법](https://gist.github.com/ihoneymon/652be052a0727ad59601)
- [참고문헌1 마크다운 사용법](https://post.naver.com/viewer/postView.nhn?volumeNo=24627214&memberNo=42458017)