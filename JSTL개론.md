## JSTL
JSTL(JavaServer Pages Standard Tag Library)
JSP 페이지에서 기존의 태그로 처리하기 힘든 부분을 담당하는 Tag Library

JSTL라이브러리가 필요하므로 **jar 파일**로 별도로 다운받아야 한다.

다운받은 **jar파일은** 이클립스에 properties > java Build path > Libraries > Add External JAR 버튼 클릭!

라이브러리 추가하기

파일에 

https://user-images.githubusercontent.com/42515875/48136895-2a021300-e2e4-11e8-8744-94afb4575d8d.png

```
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %@>

<c:>
<h1>${list.num}</h1>
</c:>
```
