## 들어가기 전에
- 서버에서 전송한 데이터가 클라이언트에 도착해야 할 곳은 'Browser'이다
- Browser에는 데이터를 해석해주는 `parser`와 데이터를 화면에 표현해주는 `rendering` 엔진이 포함되있음
## 
![구성요소](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/layers.png)
- User interface : 주소 표시 줄,뒤로/ 앞으로 가기 단추,책갈피 메뉴 등등 페이지가 표시되는 창을 제외한 브라우저 모든 부분 표시

- Browser engine : UI와 렌더링 엔진 간의 동작을 마샬링?

- Rendering engine : 요청 된 콘텐츠를 표시함, 콘텐츠가 HTML인 경우 렌더링 엔진은 HTML CSS를 구문 분석하고 구문 분석 된 콘텐츠를 화면에 표시

- Networking engine : HTTP 요청과 같은 네트워크 호출에 사용

- Javascript interpreter : JavaScript 코드를 구문 분석하고 실행하는데 사용

- UI backend : 콤보 상자 & 창과 같은 기본 위젯 그리는데 사용


## rendering engine
 - browser 마다 다른 rendering engine 을 사용
    - Internet Exploerer 는 Trident
    - Firefox Gecko
    - Safari WebKit
    - Chrome & Opera Webkit
    
![주요 흐름](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/flow.png)

### 주요흐름

- 렌더링 엔진은 HTML 문서 파싱 시작 -> 콘텐츠 트리라는 트리에서 요소를 `DOM노드`로 변환
- 엔진은 외부 CSS 파일과 스타일 요소 모두에서 스타일 데이터 구문 분석
- HTML의 시각적 지침과 함꼐 정보를 스타일링
- `렌터트리`에는 색상 & 치수와 같은 시각적 속성이 있는 사각형이 포함
- 그 후에 `레이아웃` 프로세스로 , 이는 각 노드에 화면에 표시 될 정확한 좌표를 제공함
- `페인팅` 렌더 트리가 순회하고 각 노드는 UI 백엔드 레이어를 사용하여 페인팅됨


## parsing
- 문서를 parsing 한다는 것은 코드가 사용할 수 있는 구조로 번역하는 것을 의미

![parsing](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/image009.png)

## HTML 구성요소
```html
<html> 
 <body> 
  <p>안녕하세요</ p> 
  <div> <img src = "example.png" /> 
  </div>
 </body>
</html>
```
- mark up 의 DOM 트리구조
![DOM](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/image015.png)

## CSS parsing
-css parsing 구조
-`p.div`,`error` : selector
- `margin.top:3px;`: ,declaration , element 간 간격

## render tree
![tree](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/image025.png)


![css](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/image023.png)
 
