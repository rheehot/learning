## EL 태그
EL(Expression Language)<br>

- EL 형식 : ```<%= %>```
- 자바 코드를 사용하지 않고 더 간편하게 출력을 지원하는 도구
- java와 동일한 연산기능 제공, ==, eq, !=, ne, and, or, not, empty, not empty

${empty cookie} <br>
${not empty cookie}


Attribute형식에서는 ```${cont +1}```이런 식으로 사용한다.

attribute란 : 메소드를 통해서 저장되고 사용되는 데이터이다.

setAttribute("key", value) -> 값을 넣는다.

getAttribute("key") -> 값을 가져온다.


- param : 요청 파라미터의 <파라미터 이름, 값> 매핑을 저장한 Map객체
parameter형식은 ```${param.no}```이런 식으로 사용한다.

### 객체의 메소드 호출

<%
  method md = new method();
  request.setAttribute("t", md);
%>
