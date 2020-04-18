# HTML 문서구조
 - 크롬 브라우저 설치
 - 크롬 개발자 도구 열기
 - 윈도우(Ctrl + Shift + i)
 -[접속](http://www.amazon.com)
 
# 특징 
 - head 는 문서에 추가적인 정보를 포함
 - body 화면에 표현되어야할 div같은 것들이 포함
 - HTML은 계층적
 - HTML은 tag를 사용해서 표현 
 `<tag class='title>안녕하세요</tag>`
 
 - [jsbin](https://jsbin.com/?html,output) tool
```<html>
  <head>
    <meta charset = "utf-8">
    <meta name== "viewport" content ="width=device-width, initial-scale=1">
    <title>저를 소개해요</title>
    <link rel ="sytlesheet" href = "css/style.css"
    <script src ="js/start.js"></script>
  </head>
  <body>
    <h1>안녕하세요</h1>
    <div>코드스쿼드 크롱입니다</div>
    <script src ="js/library.js"></script>
    <script src ="js/main.js"></script>
   </body>
  </html>
```
- meta : 문서 그 자체를 설명하는 태그
- style : css 를 담을 수 있다
- script : javascript를 담는다. 해석이 느려질 수 있어 웬만하면 </body>아래쪽으로
- src : 외부파일
