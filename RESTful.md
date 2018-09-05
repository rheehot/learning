# What is RESTful
  - Representational State Transfer(REST) 
  - 하나의 클라이언트를 위한 서버를 구성하는 것이 비효율적,,,,
    이를 보완하는 것이 RESTful
  - 하나의 서버로 여러개의 클라이언트를 대응시키도록 한다.
### REST 특징
  1. HTTP 프로토콜 표준을 사용한다. -> HTTP의 캐싱기능 사용 가능
  2. REST API 메시지만 보고 쉽게 이해가능
  3. REST 서버는 API를 제공하고, 일반 비지니스 로직을 서버단 처리 기능을 한다.
  
### REST의 구성
  - Resource (URL)
      1. URL은 Resource를 표현해야 한다.
  - HTTP Method (GET, POST, PUT, DELETE)
      1. Resource에 대한 것은 HTTP Method(GET, PUT, PUSH, DELETE)로 표현한다.
  - Representations (express)
  
  
### REST API 중심 규칙
  - HTTP Method의 표현방식(행위 GET, PUT, POST, DELETE)이 URL에 들어가선 안된다.
  ```
  URL >>> GET / github/insert/repogit   (X)
  URL >>> GET / github/repogit          (O)
  ```
  
  
