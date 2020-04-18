# HTTP(Hypertext Transfer Protocol)
## 서버와 클라이언트가 인터넷상에서 데이터를 주고받기 위한 프로토콜
### HTTP 작동방식
- HTTP는 서버/클라이언트 모델을 따른다
- 장점 - 불특정 다수 대상 서비스에 적합
	    - 클라이언트와 서버가 계속 연결상태가 아니라서 최대연결 수 보다 훨씬 많은 응답을 처리할 수 있음
		
- 단점 - 연결을 끊어 버리기 때문에,클라이언트 이전 상황을 알 수 없음
		-이러한 특징 때문에 Cookie와 같은 기술이 등장함
## URL(Uniform Resource Locator)
### 인터넷 상의 자원의 위치
- 특정 웹 서버의 특정 파일에 접근하기 위한 경로 or 주소
 `https://www.edwith.org/boostcourse-web/lecture/16661/#`
	
- 요청 method -GET,PUT,POST,PUSH,OPTIONS 등의 요청 방식
- 요청 URI 요청하는 자원의 위치를 명시
- HTTP프로토콜 버전 - 웹 브라우저가 사용하는 프로토콜 버전
	
- `GET` - 정보를 요청하기 위해 (SELECT)
- `POST` - 정보를 넣기 위해 (INSERT)
- `PUT`  - 정보를 업데이트 하기 위해(UPDATE)
- `DELETE` - 정보를 삭제하기 위해(DELETE)
- `HEAD` - 헤더 정보만 요청함,해당 자원의 존재 유무,서버문제 확인 시 사용하는
- `OPTIONS` - 웹서버가 지원하는 METHOD 종류를 요청
- `TRACE` -클라이언트 요청을 그대로 반환,
	
