### CRUD
- **C**reate, **R**ead, **U**pdate, **D**elete
### JPA
- JPA(Java Persistence API)
- java의 ORM기술표준이다.
- 생산성 향상 - 기본적인 CRUD를 직접 작성하지 않아도 된다.
### ORM
- ORM(**O**bject-**R**elational **M**apping)
- 객체의 관계형 데이터베이스를 매핑한다는 의미이다.
- ORM프레임워크에는 'EclipseLink', 'DataNucleus', '하이버네이트'가 있다.

### MyBatis
- MyBatis나 스프링 JdbcTemplate은 SQL Mapper이다. 객체와 SQL을 매핑한다.  
따라서 SQL을 개발자가 따로 작성해야한다. 결국 SQL의존적인 개발을 피할 수 없다.  
하지만 ORM은 객체와 테이블을 매핑한다. 따라서 SQL을 자동으로 만들어준다. SQL 의존적인 개발을 피할 수 있다.

**[출처]**  [[JPA] JPA,하이버네이트,ORM이란? JPA가 MyBatis와 다른점은?](https://blog.naver.com/kbh3983/220911550813)|**작성자**  [뽕](https://blog.naver.com/kbh3983)
### Maven
- **Maven**은 프로젝트를 관리하기 위한 **빌드도구**이다.
-  JAVA기반 프로젝트의 **라이프 사이클 관리**를 목적으로 사용한다.
 - pom.xml파일에 사용할 라이브러리나 모듈을 적어놓으면 해당 라이브러리와 다른 의존성이 있는 라이브러리까지 자동으로 다운로드해서 버전을 관리해 준다.
- 프로젝트를 하다보면 JAVA의 여러 라이브러리를 필요로 하게되는데 pom.xml에 형식에 맞게 라이브러리를 적어 놓으면, 알아서 의존성 있는 라이브러리까지 다운로드해준다.
 > MAVEN 장점
 -  따로 jar파일을 다운로드 해서 복사하는 수고로움이 없다. 
그래서 버전관리가 수월하다.
 - 자동으로 jar파일을 다운로드한다. 
> MAVEN 단점
- 네트워크가 연결되어 있어야 한다.


### Gradle
- 빌드 배포도구이다.
- 안드로이드 프로젝트를 만들면 Gradle도 같이 생긴다.
- 안드로이드 스튜디오(IDE)와 빌드 시스템이 서로 독립적이다.
- 안드로이드 스튜디오는 코드의 편집만을 담당하고, **빌드는 Gradle을 통해서 수행된다.**



라이브러리를 추가하려면 jar파일을 다운받아서 설정해줘야 했지만, 라이브러리 관리도구인 **ant, maven, Gradle**등의 라이브러리 관리 도구를 사용하게 되었다.
이 중 안드로이드 스튜디오가 Gradle을 채택해서 쓰고 있다.


> reference by [출처 블로그](https://blog.naver.com/indy9052/221354214398).
