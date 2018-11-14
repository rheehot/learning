## EL 태그
EL(Expression Language)<br>

- EL 형식 : ```<%= %>```
- 자바 코드를 사용하지 않고 더 간편하게 출력을 지원하는 도구
- java와 동일한 연산기능 제공, ==, eq, !=, ne, and, or, not, empty, not empty
- 라이브러리 없이 사용가능, JSP2.0버전 이후부터 사용가능
- 변수값이 scope에 저장되어 있어야만 사용가능하다.
- scope는 page context, request, response, session, application을 말한다. 이안에 변수 이름을 함께 저장하면 나중에 **${변수}** 로 값을 불러올 수 있다.


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

### 1. 변수태그 (set)
 > <c:set var = "변수명" value = "값">
### 2. 출력태그(out)
> <c:out value = "출력값>
### 3. 삭제태그(remove)
  > <c:remove var ="변수명"> 
### 4. 조건처리문(if)
- else는 없다.
> <c:if test ="조건식" var = "변수명">
### 5. 조건처리(choose)
- java의 switch와 유사하다.
> <c:choose>
>   <c:when test = "조건식1"> 조건식 실행</c:when>
> </c:choose>

### 6. 반복문처리(forEach)
> <c:forEach begin ="시작값" end="끝값" step="증감값" var ="변수명">
>   <c:forEach item="객체명" var="변수">
