## JSTL
JSTL(JavaServerPages Standard Tag Library)
### Where does 'JSTL' work?
- JSP 페이지에서 자바형식의 코드를 사용하기 위한 방법으로 사용되는 Tag Library

### How to use 'JSTL', install method
  1. JSTL라이브러리가 필요하므로 **jar 파일**로 별도로 다운받아야 한다.
  2. 다운받은 **jar파일은** 이클립스에 properties > java Build path > Libraries > Add External JAR 버튼 클릭!
  3. 라이브러리 추가하기
 
    WebContent > WEB-INF > lib 안에 jstl.jar파일을 넣어주면 사용 가능하다.

![image](https://user-images.githubusercontent.com/42515875/48136895-2a021300-e2e4-11e8-8744-94afb4575d8d.png)

```
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %@>

<c:>
<h1>${list.num}</h1>
</c:>
```

### JSTL 태그
#### 1. <c:forEach>
 자바에서 for문 기능
    ```<c:forEach var ="i" begin="1 end="10" step="1"> ${} </c:forEach>```

#### 2. <c:set>
    
    
 
 <c:set var ="it" value ="${requestScope.넘겨받는 변수 이름}"/> 
 
  
  it이란 변수에 ${requestScope.변수이름} 값을 저장한다.

#### 3. <c:if>
    
    <c:if test ="${it != 'true'}">HTML태그 내용</c:if>
    

   it이란 변수가 true이면 HTML태그 내용 실행하게 된다.

    
    <c:if test="${it eq 'true'}"></c:if>
    

   'eq'를 '='대신 사용할 수 있다.

    
    <c:if test="${not empty sessionScope.name }"><h1>★${name}★</h1></c:if>
    
    
   'not empty' or 'empty' 세션을 유무파악


