# Code Lion 수강 기록
<details close>
<summary> 일단 만드는 HTML/CSS</summary>

### HTML TAG 정리
1. `<!DOCTYPE html>` = 가장 윗줄에 작성한다.  <br>
2. `<html>`, `</html>` = 필요 없는 태그임에도 작성한다.  <br>
3. `<head>` = 부가적인 정보를 제공한다.   <br>
>   (1) `<meta charset="UTF-8">` - 한글을 사용한다고 명시.  <br>
>   (2) `<title>`, `</title>` = 검색키워드  <br>
>   (3) `<link rel="stylesheet" href="css주소">` -> 단독적으로 사용 가능. 슬러시 태그로 닫지 않는다.  <br>
4. `<body>` = 컨텐츠를 다루는 태그. 대부분의 내용을 다룸.  <br>
>   (1) `<h1>`, `</h1>` = 글꼴의 크기  <br>
>   (2) `<p>`, `</p>` = 일반 문서 작성 시  <br>
>   (3) `<footer>`, `</footer>` = 웹페이지 하단에 공통적으로 써 있는 내용, 안내문 (html 문서에서 위치 중요.)  <br>
>   (4) `<p(div,...) class="이름">` = 같은 태그를 여러 묶음으로 나눠주는 역할을 한다.  <br>
>   (5) `<div>` = `<section>` = `<article>` = 꾸며주기 위해 묶는 태그. 각각은 </>로 닫아줘야 한다.  <br>
 <br>

### CSS 문법 정리 
: CSS는 꾸미는 작업이 전적으로 이루어지는 공간이다. 중괄호 내 순서는 중요하지 않다. 기본적인 구조는 다음과 같다.  <br>
``` 
      태그 or .클래스이름 {  <br>
       꾸밀 요소: 내용;  <br>
       }  <br>
```
  <br>

1. 글꼴  <br>
>   (1) text-align: 글꼴 위치; = 글꼴 정렬  <br>
>   (2) font-size: 크기px; = 글꼴 크기  <br>
>   (3) font-weight: bold; = 폰트의 두께(두껍게)  <br>
>   (4) font-style: italic; = 폰트 스타일(기울여서)  <br>
>   (5) color: 색상; = 글꼴 색상  <br>
2. 박스  <br>
>   (1) width: 크기px; = 박스 폭 조정  <br>
>   (2) heigt: 크기px; = 박스 높이 조정  <br>
>   (3) margin-left: auto;  <br>
>      margin-right: auto; = 박스 가운데 정렬  <br>
3. border: 두께px 방식 색상; = 박스 테두리 설정  <br>
>   - border-top/bottom/right/left = 상, 하, 좌, 우 개별 크기 조절  <br>
4. padding  <br>
padding: 크기px; = border(테두리)와 내용 사이의 간격  <br>
>   - padding-top/bottom/right/left = 상, 하, 좌, 우 개별 크기 조절  <br>
5. margin: 크기px; = 박스의 바깥 영역  <br>
>   - margin-top/bottom/right/left = 상, 하, 좌, 우 개별 크기 조절  <br>
6. box-shadow: 0 1px 20px 0 rgba(0,0,0,0.1);  <br>
>   (1) 0 = 가로축으로 그림자가 얼마나 뻗어나가는지. 양(우), 음(좌)  <br>
>   (2) 1px = y축 그림자 이동  <br>
>   (3) 20px = 그림자의 흐린 정도, 블러값  <br>
>   (4) 0 = 그림자의 퍼짐도, 스프레드값  <br>
>   (5) rgba(0,0,0,0.1); = red, green, blue, 투명도. / rgb의 범위는 0~255.  <br>
7. 사진  <br>
>   (1) `<img src="images/이름.png">`  = 사진 추가  <br>
>   (2) `<img class="이름" src="images/이름.png">` = 이미지 클래스 생성  <br>
>   (3) `<a href="url">img class="이름" src="images/이름.png"></a>` = 링크 삽입 / a 태그  <br>
8. 기타  <br>
>   (1) background-color: 색상; = 배경 색상  <br>
>   (2) line-height: 크기px; = 줄간격  <br>
  <br>
  
### 구글 웹 폰트 적용 
1. CSS에 다음 코드를 입력해 글꼴을 불러온다.  <br>
>     `@import url('구글 폰트 url')`  <br>
2. CSS에 다음 코드를 입력해 글꼴을적용한다.  <br>
```
      \* {  <br>
          font-family: '폰트이름';  <br>
      }  <br>
```
<br>

### margin, padding 초기화
: 기본값이 브라우저마다 다르기 때문에 초기화가 필요하다.  <br>
 ```
    body, h1, h2    {  
        margin: 0px;  
        padding: 0px;  
    }  
```
  
### 한 줄에 내용 좌우측 배치하기 
1. float: left(or right); = 둥둥 떠다니되, 왼(or 오른)쪽에서.  <br>
2. HTML에서 한 줄에 배치하고자 하는 내용을 class 'A'로 묶는다.   <br>
3. CSS에서 .A 내용 안에 다음 코드를 입력한다.  <br>
: overflow: hidden; = 모든 float 요소들을 묶고, 다른 html에 영향이 가지 않도록 설정한다.  <br>
  <br>

</details>