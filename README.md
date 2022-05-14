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
# 자세한 날씨 : weather - description
print("날씨는 ",data["weather"][0]["description"],"입니다.")
# 현재 온도 : main - temp
print("현재 온도는 ",data["main"]["temp"],"입니다.")
# 체감 온도 : main - feels_like
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