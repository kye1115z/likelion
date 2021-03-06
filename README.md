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
     `@import url('구글 폰트 url')`  <br>
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


<details close>
<summary> 파이썬 기초 </summary>

### 오늘은 뭐 드실? (직접)
```import random
import time

lunch = ["된장찌개", "피자", "제육볶음", "짜장면"]

while True:
    print(lunch)
    item = input("음식을 추가 해주세요 : ")
    if(item == "q"):
        break
    else:
        lunch.append(item)
print(lunch)

set_lunch = set(lunch)
while True:
    print(set_lunch)
    item = input("음식을 삭제해주세요 : ")
    if(item == "q"):
        break
    else:
        set_lunch = set_lunch - set([item])

print(set_lunch, "중에서 선택합니다.")
print("5")
time.sleep(1)
print("4")
time.sleep(1)
print("3")
time.sleep(1)
print("2")
time.sleep(1)
print("1")
time.sleep(1)
print(random.choice(list(set_lunch)))
```

### 익명 질문 게시판(직접)
```total_list = []
while True:
    question = input("질문을 입력해주세요 : ")
    if question == "q":
        break
    else:
        total_list.append({"질문" : question, "답변" : ""})


for i in total_list:
    print(i["질문"])
    answer = input("답변을 입력해주세요 : ")
    i["답변"] = answer
print(total_list)
```

</details>

<details close>
<summary> 파이썬 심화 </summary>

### 실시간 검색어 확인하기
1. 요청하기 
`Response = requests.get(url)`
2. 기능
`print(response.text)`

`print(response.url)`

`print(response.content)`

`print(response.encoding)`

`print(response.headers)`

`print(response.json)`

`print(response.links)`

`print(response.ok)`

`print(response.status_code)`

3. Beautiful Soup
:문자열 덩어리를 Beautiful Soup에 정렬해놓음.

3-1. import
`From bs4 import BeautifulSoup`

3-2. parsing
: 데이터를 의미 있는 값으로 변환하는 것
`Beautifulsoup(response.text, ‘html.parser’)`

3-3. 기능
1) `print(soup.title.string)` = title 태그 안 문자 출력. 실제 제목값만 출력.
2) `print(soup.span)` = span 태그 출력, 가장 상단에 위치한 span 태그 하나.
3) `print(soup.findAll(‘span’))` = 모든 span 태그 출력함.

4. 파일로 저장하기
```
File = open(“daum.html”, “w”)
File.write(response.text)
File.close() 
```

5. 직접 짜보기
```
from bs4 import BeautifulSoup
import requests
from datetime import datetime

url = "http://www.daum.net/"
response = requests.get(url)
soup = BeautifulSoup(response.text, 'html.parser')
rank = 1

results = soup.findAll('a','link_favorsch')

print(datetime.today().strftime("%Y년 %m월 %d일의 실시간 검색어 순위입니다.\n"))

for result in results:
    print(rank,"위 : ",result.get_text(),"\n")
    rank += 1
```

### 날씨 정보 받아오기
1. API 링크 적용하기
```
city = “Seoul”
apikey = “나의 api key”
api = f“https://api.openweathermap.org/data/2.5/weather?q={city}&appid={apikey}”
print(api)
```

2. 날씨 받아오기
```
Result = requests.get(api) -> 요청보내기
Print(result.text) 
```

3. Json 모듈(JavaScript object natiation)
: 데이터를 주고 받을 때 사용하는 포맷

3-1. 타입 변경하기

`Data = json.loads(result.text)`

3-2. 필요한 결과만 불러오기
: print(data["key값"])
```
print(data["name"],"의 날씨입니다.")
print("날씨는 ",data["weather"][0]["description"],"입니다.")
print("현재 온도는 ",data["main"]["temp"],"입니다.")
print("하지만 체감 온도는 ",data["main"]["feels_like"],"입니다.")
# 최저 기온 : main - temp_min
print("최저 기온은 ",data["main"]["temp_min"],"입니다.")
# 최고 기온 : main - temp_max
print("최고 기온은 ",data["main"]["temp_max"],"입니다.")
# 습도 : main - humidity
print("습도는 ",data["main"]["humidity"],"입니다.")
# 기압 : main - pressure
print("기압은 ",data["main"]["pressure"],"입니다.")
# 풍향 : wind - deg
print("풍향은 ",data["wind"]["deg"],"입니다.")
# 풍속 : wind - speed
print("풍속은 ",data["wind"]["speed"],"입니다.")
```

4. 언어 단위 변경하기
: 각각에 알맞은 파라미터를 추가한다.
4-1. 영어 -> 한글
```
api = f"""http://api.openweathermap.org/data/2.5/\
weather?q={city}&appid={apikey}&lang={lang}"""

```

4-2. 화씨 -> 섭씨
```
api = f"""http://api.openweathermap.org/data/2.5/\
weather?q={city}&appid={apikey}&lang={lang}&units=metric"""
```

5. 직접 짜보기
```
import requests
import json

city = "Seoul"
apikey = "나의 api key"
lang = "kr"
# units - metric
api = f"""http://api.openweathermap.org/data/2.5/\
weather?q={city}&appid={apikey}&lang={lang}&units=metric"""

result = requests.get(api)
# print(result.text)

data = json.loads(result.text)

# 지역 : name
print(data["name"],"의 날씨입니다.")

print("날씨는 ",data["weather"][0]["description"],"입니다.")

print("현재 온도는 ",data["main"]["temp"],"입니다.")

print("하지만 체감 온도는 ",data["main"]["feels_like"],"입니다.")

print("최저 기온은 ",data["main"]["temp_min"],"입니다.")

print("최고 기온은 ",data["main"]["temp_max"],"입니다.")

print("습도는 ",data["main"]["humidity"],"입니다.")

print("기압은 ",data["main"]["pressure"],"입니다.")

print("풍향은 ",data["wind"]["deg"],"입니다.")

print("풍속은 ",data["wind"]["speed"],"입니다.")

```

### 번역하기
1. googletrans 모듈
: 언어 감지 및 번역을 도와주는 모듈

1-1. 언어감지란?

:입력한 값이 어떤 언어인지 파악하는 것

1-2. 번역이란?

: 특정한 언어의 뜻을 파악해서 그 뜻을 특정한 언어에 대응시키는 것

1-3. import

`from googletrans Import Translator`

2. 언어 감지하기 
: translator(), detect()

```
translator = translator()
sentence = "안녕하세요. 코드라이언입니다."
detected = translator.detect(sentence)
```

2.1 출력 결과

Print(detected)

> Detected(lang=ko, confidence=1.0)

> 한국어/100% 신뢰

Print(detected.lang)

>	Ko

> 언어 감지함.


3. 번역하기
: translate(text, dest, src) = translate(번역을 원하는 문장/번역하려는 언어/text의 언어감지)

`Result = (translator.translate(sentence,’en’))`

3.1 출력 결과

Print(detected.lang, “:”, sentence)
> Ko: 안녕하세요 코드 라이언입니다.
Print(result.dest, “:”, result.text)
> En: hello, this is Code Ryan.

3.2 언어

1) 프랑스어 = fr

2) 베트남어 = vi

3) 스페인어 = es

4) 중국어 = zh-CN

5) 아랍어 = ar

6) 독일어 = de

7) 몽골어 = mn

8) 힌디어 = hi

4. 직접 짜보기
```
from googletrans import Translator

translator = Translator()

sentence = input("번역을 원하는 문장을 입력해주세요 : ")
dest = input("어떤 언어로 번역을 원하시나요?")

result = translator.translate(sentence,dest)
detected = translator.detect(sentence)

print("===========출 력 결 과===========")
print(detected.lang,":",sentence)
print(result.dest,":",result.text)
print("=================================")

```

### 메일 보내기
1. SMTP
: Simple Mail Tranfer Protocol(간단하게 메일을 보내기 위한 약속)

SMTP = email client -> email server or email server -> email server 

IMAP = email server -> email client

1.1 SMTP 메일 서버 연결

* smtplib 호출 `import smtplib`

* 메일서버에 연결 
Smtplib.SMTP(서버주소, 포트번호)

```
SMTP_SERVER = 	“smtp.gmail.com”
SMTP_PORT = 465
Smtp = smtplib.SMTP(SMTP_SERVER,SMTP_PROT)
```

* SSL 처리(보안)

`smtp = smtplib.SMTP_SSL(SMTP_SERVER,SMTP_PROT)`

1.2 메일 서버에 로그인 하기
`Print(smtp.login(“kye1115z@likelion.org”, “비밀번호”))`

2. 메일 보내기
2.1 MIME

: 전자우편을 위한 표준 포맷

2.2 email.message 모듈

: MIME로 담을 폼을 만든다.

`from email.message import EmailMessage`

`Message = EmailMessage()`

2.3 이메일의 내용을 담기

` message.set_content(“코드라이언 수업 중입니다.”) `

2.4 MIME-Header

```
Message[“Subject”] = “이것은 제목입니다.”
Message[“From”] = kye1115z@likelion.org
Message[”To”] = kye1115z@gmail.com

```



5. 직접 짜보기
```
from email.message import EmailMessage
import smtplib

# SMTP 접속을 위한 서버, 계정 설정
SMTP_SERVER = "smtp.gmail.com"
# google의 SMTP server 포트 주소는 465
SMTP_PORT = 465


# 이메일 유효성 검사 함수
def is_valid(addr):
    import re
    if re.match('(^[a-zA-Z0-9.+_-]+@[a-zA-Z0-9-]+.[a-zA-Z]{2,3}$)', addr):
        return True
    else:
        return False

message = EmailMessage()
message.set_content("코드라이언 메일링 수업 - 본문입니다.")

message["Subject"] = "코드라이언 메일링 수업입니다."
message["From"] = "###@gmail.com"
message["To"] = "###@gmail.com"

smtp = smtplib.SMTP_SSL(SMTP_SERVER,SMTP_PORT)
smtp.login("###@gmail.com","######")

is_valid("###@gmail.com")
if smtp.send_message(message)=={} :
    print("성공적으로 메일을 보냈습니다.")

smtp.quit()
```


</details>

<details close>
<summary> JavaScript </summary>

screenshot
![screensh](./img1/image.png)

### JavaScript 기초
:웹브라우저에서 사용하기 위해 만들어진 프로그래밍 언어. UI를 동적으로 구성할 수 있으면 브라우저뿐만 아니라 서버에서도 사용 가능함.

- console.log() : 콘솔의 특정 내용을 출력
    - console.log(1+2+3+4+5); 연산이 가능함.

1. 변수
: 값을 저장할 수 있는 메모리 공간(숫자, 문자, 참/거짓)

2. 라이브 서버 연결
: 내 컴퓨터를 서버처럼 작동시켜 웹개발에 도움을 준다.

- http://127.0.0.1:5500/js_syntax.html
    - 127.0.0.1 = 내 컴퓨터 주소
    - 5500 = 포트 번호
    - js_syntax.html 파일명
    
1) 뼈대 만들기

: `! (enter)`

2) \<head\> 태그 안 자바스크립트 코드 넣기

```
<script>
let favoriteArtist = 'IU';
console.log(favoriteArtist);
</script>
```

3. 자료형

1) 숫자형

2) 문자열

3) 참/거짓

4) Null/Undefined  
null은 빈 값을 할당, undefined는 값 자체를 할당하지 않음.

4. 연산자

1) 산술연산자  
2) 문자결합연산자  
3) 대입연산자  
4) 증감연산자  
5) 비교연산자  
6) 논리연산자  

5. 제어문

1) 조건문  
```
if(month >= 3 && month <= 5){
   console.log("따스한 햇살 가득한 봄");
} else if (month >= 6 && month <= 8){
  console.log("쨍쨍 햇빛 여름");
} else if (month >= 9 && month <= 11){
  console.log("가을");
} else{
  console.log("겨울");
}
```

2) 반복문  

6. 함수
```
const a = 1;
const b =2;
const sum = a+b;
console.log(sum);

function add(num1, num2){
    return num1 + num2;
    console.log("실행되지 않습니다.")
}   ,
const sum2 = add(100,200);
console.log(sum2);
```

7. 객체
```
const sample = {
    'key with space' = true
};

const likelion = {
    name : '멋쟁이사자처럼'
    age : 10
};
```

### HTML+JS
1. 배열(array)

: const 배열명 = [첫번째 요소, 두번째 요소, ..., n번째 요소];

- 여러 자료를 변수 하나에 저장 가능
- 순서 개념 있음

2. DOM  
: 문서 객체 모델, 구조화된 문서 표현하는 형식의 도메인 객체 모델.

`document.getElementByle('id값'); //노드 취득`
`document.getElementsByTagName('태그 이름'); //모든 요소 노드들을 탐색해 반환`
`document.getElementsByClassName('class 값');`
`document.querySelector('css선택자');`
`document.querySelectorAll('css 선택자');`

1) index.html
```
<body>
    <ul id="animals">
        <li class="animal">lions</li>
        <li class="animal">tiger</li>
        <li class="animal">bear</li>
    </ul>
    <script src="./practice.js"></script>
</body>
```

2) main.css
```
.box {
    width: 100%;
    height: 50px;
    border-radius: 10px;
    border: 2px solid rgb(133, 133, 133);
}

.purple {
    background-color: rgb(132, 125, 243);
}

.yellow{
    background-color: rgb(255, 255, 0);
}
```

3) practice.js
```
document.querySelectorAll(".animal")[2].innerHTML = "dog";

animals.innerHTML += "<li class = 'animal'>Cat</li>";

document.querySelectorAll(".box")[0].classList.add("purple");

document.querySelectorAll(".box")[0].classList.remove("pruple");

document.querySelectorAll(".box")[0].classList.toggle("yellow");
```

4. Event  
: 어떤 사건을 발생시키는 것.

1) Event type

:이벤트의 종류를 나타내는 문자열
```
EventTarget.addEventListener(
'eventType', function, useCapture);
```

2) index.html
```
<body>
    <div class = "bar>여기 눌러봐</div>
    <div class="newBar">짠 내가 생겼어</div>
    <script src="./practice.js"></script>
</body>
```

3) main.css
```
body {
    font-family: "Do Hyeon", sansserif;
}

.bar    {
    width: 100%;
    height: 50px;
    bacground-color: rgb(165, 145, 255);
    text-align: center;
    padding-top: 20px;
}

.newBar {
    width: 100%;
    height: 50px;
    background-color: rgba(255, 166, 0, 0.731);
    text-align: center;
    padding-top: 20px;
    display: n;
}
```

3) practice.js

```
document.querySelector(".bar").addEventListener("click", fucntion () {
    document.querySelector(".bar").innerHTML = "눌렀어!";

    document.querySelector(".newBar").classList.toggle("show");
})
```

5. Scroll Event
`window.addEventListener('scroll', function() {});`

6. 타이머 함수
`)
`setTimeout (타이머가 만료된 후에 호출될 콜백함수 or 문자열 , 시간)`

```
setTimeout(() => {
    document.querySelectorAll(".timeout")[0].style.display = "none";}, 5000);
```
2)
`setInterval(타이머가 만료된 후에 호출될 콜백함수 or 문자열, 시간)`

```
setInterval(function () {
    timecnt--;
    $(".timeout").html(`${timecnt}초 이내 구매시 사은품 증정`);
}, 1000);
```

</details>

<details close>
<summary> 프론트엔드트랙-React </summary>

<img src="https://user-images.githubusercontent.com/78716896/182359134-0965350b-5b76-461c-bd17-45b52bc06b97.png">

</details>

### 
# 멋쟁이사자처럼 HUFS 세션 기록
<details close>
<summary> 크롤링(Youtube TOP 100) </summary>


### 라이브러리 설치
```!pip install selenium
!apt-get update
!apt install chromium-chromedriver
!cp /usr/lib/chromium-browser/chromedriver /usr/bin
```
이 코드 입력하고 다시 설치해보세요
``` !pip install folium==0.2.1
```
#라이브러리 설치
```!pip install selenium
!apt-get update
!apt install chromium-chromedriver
!cp /usr/lib/chromium-browser/chromedriver /usr/bin
```
### import 라이브러리
```#libraries
from selenium import webdriver
from bs4 import BeautifulSoup
```

### import time    #  time.sleep(대기시간)
```import pandas as pd
```

#Colab에선 웹브라우저 창이 뜨지 않으므로 별도 설정한다.
 
```options = webdriver.ChromeOptions()
options.add_argument('--headless')        # Head-less 설정
options.add_argument('--no-sandbox')
options.add_argument('--disable-dev-shm-usage')
driver = webdriver.Chrome('chromedriver', options=options)
```

### 페이지 접속하기
```url = 'https://youtube-rank.com/board/bbs/board.php?bo_table=youtube&page=1'
driver.get(url)
```
#BeautifulSoup 활용하여 데이터 정리하기
```html = driver.page_source
html

soup = BeautifulSoup(html, 'html.parser')
```
### 4. 원하는 정보 찾기
#채널 html 뭉치 찾아보기
```channel_list = soup.select('tbody > tr')
len(channel_list)
```
#tr만 찾으면 102개가 나옴. 상위의 것까지 포함되어서
#부모 tbody 했더니 101개 아직도 ㄴ!

```channel_list = soup.select('table > tbody > tr')
len(channel_list)
```
#아직도 ㄴ! 하나 더 올라가자

```channel_list = soup.select('form > table > tbody > tr')
len(channel_list)
```
### 더 편리하게 찾는 방법
#channel_list = soup.select('.aos-init.aos-animate')
#len(channel_list)

#100일 줄 알았는데 왜 2개일까요? class 이름이 다르다! aos-init만 공통적. 뒤의 것을 빼자.

```channel_list = soup.select('.aos-init')
len(channel_list)
```
#개별 정보 출력은 list 출력과 같다!
```channel_list = soup.select('form > table > tbody > tr')
channel_list[0]
```
#채널 100개 중 한 개를 선택해서 분석해보자!
```channel = channel_list[0] #블핑 것으로..
channel
```
#채널명 찾기
```title = channel.select('h1 > a')
len(title)

title = channel.select('h1 > a')[0].text.strip()
```
#리스트 대괄호 없애기 위해 [0], 꺾새 없어지고 tap으로만 .text, 나머지 tap 없애기 .stirp()

title

#카테고리 정보 정리해보기
```category = channel.select('p.category')[0].text.strip()
category
```
#구독자 정보 정리해보기
```subscriber = channel.select('td.subscriber_cnt')[0].text.strip()
subscriber
```
#뷰 정보 정리해보기
```view = channel.select('td.view_cnt')[0].text.strip()
view
```
### 채널 하나의 정보를 수집하기
##1. 채널 선택하기
   channel = channel_list[0]
##2. 1개의 채널 정보를 정리
   title = channel.select('h1 > a')[0].text.strip()
   category = channel.select('p.category')[0].text.strip()
   subscriber = channel.select('td.subscriber_cnt')[0].text.strip()
   view = channel.select('td.view_cnt')[0].text.strip()
#3. cnffurgkrl
#print(title, category, subscriber, view)

#100개는? 반복문을 활용해서!
for channel in channel_list:

  title = channel.select('h1 > a')[0].text.strip()
  category = channel.select('p.category')[0].text.strip()
  subscriber = channel.select('td.subscriber_cnt')[0].text.strip()
  view = channel.select('td.view_cnt')[0].text.strip()

print(title, category, subscriber, view)

### 리스트에 이 모든 정보를 저장하기
```results = [] #<-정보를 저장할 빈 리스트 생성
for channel in channel_list:

  title = channel.select('h1 > a')[0].text.strip()
  category = channel.select('p.category')[0].text.strip()
  subscriber = channel.select('td.subscriber_cnt')[0].text.strip()
  view = channel.select('td.view_cnt')[0].text.strip()
  #출력하기
  data = [title, category, subscriber, view]
  results.append(data)
results
```
### 리스트를 데이터프레임(표 모양)으로 바꾸기
#pandas를 활용하여 엑셀 파일에 저장하기

```import pandas as pd

df = pd.DataFrame(results)
df
```
#column명을 바꾼다
```df.columns = ['title', 'category', 'subscriber', 'view']
df
```
#데이터프레임 엑셀로 저장할 때(저장은 누워서 떡먹기) 확장자명 쓰기
#인덱스도 삭제할 수 있다
```df.to_excel('./youtuble_rank_top100.xlsx', index=False)

!pwd

ls

!cd drive/MyDrive
```
</details>
