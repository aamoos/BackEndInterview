# 백엔드 개발자 CS
> Was란?
- 종류 : Web Logic, Web Spere, Jeus, Jboss, tomcat

- 특징
1. 웹 브라우저와 같은 클라이언트로부터 웹 서버가 요청을 받으면 애플리케이션에 대한 로직을 실행하여 웹 서버로 다시 반환해주는 소프트웨어
2. 웹 서버와 DBMS 사이에 동작하는 미들웨어로써, 컨테이너 기반으로 동작
3. 동적인 컨텐츠를 요청받아 처리 (jsp, asp, php 등)

> WebServer란?

- 종류 : Apache, NginX, IIS, WebTob

- 특징
1. 클라이언트가 서버에 페이지 요청을 하면 요청을 받아 정적 페이지(html, png, css)를 제공함
2. 클라이언트에서 요청이 올때 가장 앞에서 요청에 대한 처리를 함
3. 정적인 컨텐츠(html, css, image 등)을 요청받아 처리

![image](https://user-images.githubusercontent.com/37327676/177281162-a244f024-29bb-4e04-8a73-de5199d93fbe.png)

> DI, AOP, IOC 란?
>
> DI란?
- Dependency Injection의 줄임말로, 의존성주입 이라고 한다.

> Dependency Injection 방법
- @Autowird를 사용한 DI(타입 주입)

![image](https://user-images.githubusercontent.com/37327676/177284698-66e419eb-3fc7-470c-8e1a-d4320516a1c0.png)

- @AllArgsConstructor를 통한 주입

![image](https://user-images.githubusercontent.com/37327676/177284776-705616ea-4520-46b1-84da-2db4498f40a9.png)

- @RequiredArgsConstructor를 통한 주입

![image](https://user-images.githubusercontent.com/37327676/177283017-087062ec-ad75-44fc-aefd-2ad76968a384.png)

- @Setter를 통한 주입

> AOP란?
- Aspect-oriented Programming의 약어로 흩어진 Aspect를 모듈화 할 수 있는 프로그래밍 기법이다. 즉, 여러 곳에서 쓰이는 모듈화하고, 쓰이는 곳에 필요할 때 연결함으로써, 유지 보수 혹은 재사용에 용이하도록 프로그래밍 하는 것

> AOP 주요 개념
- Aspect : 여러 곳에서 쓰이는 코드 (공통 부분)을 모듈화한 것
- Target : Aspect를 적용하는 곳 (클래스, 메소드)
- Advice : 실질적으로 어떤 일을 해야할지에 대한 것, 실질적인 부가기능을 담은 구현체
- JointPoint : Advice가 적용될 위치, 끼어들 수 있는 지점, 메서드 진입 시점, 생성자 호출 시점, 필드에서 값을 꺼내올 때 등 다양한 시점에 적용가능
- PointCut : JointPoint의 상세한 스펙을 정의한 것

> AOP 구현체
- AspectJ
- 스프링 AOP

> IOC란?
1. 제어의 역전이라고 불림
2. 예전에는 의존관계의 제어를 개발자가 직접 해주었다. 그러나 제어권이 컨테이너로 넘어갔고 객체의 생성부터 생명주기의 관리까지 객체에 대한 제어를 프레임워크에서 하는것을 IOC라고 한다.

> XSS란?
1. 크로스 사이트 스크립팅, 즉 사이트 간 스크립팅이라는 이름의 웹 취약점 입니다.
2. 웹 사이트의 관리자가 아닌 악의적인 목적을 가진 제 3자가 악성 스크립트를 삽입하여 의도하지 않은 명령을 실행시키거나 세션 등을 탈취할 수 있는 해킹기법입니다. 

> XSS로 인한 위험성
1. 쿠키 및 세션정보 탈취
2. 악성 프로그램 다운 유도
3. 의도하지 않은 페이지 노출

> XSS 대응방법
1. 입력 값의 길이 제한 (이메일, 아이디, 패스워드 등 목적에 맞게)
2. replace 등의 함수를 이용한 치환
3. 입력 값에 대한 꼼꼼한 유효성 검사 (반드시 서버에서 수행)
4. 불가피하게 html 태그 사용을 허용해야 할 경우 화이트리스트를 만들어 특정 태그 입력만 허용

> SQL Injection (SQL 삽입 공격)
- SQL Injection이란 악의적인 사용자가 보안상의 취약점을 이용하여, 임의의 SQL문을 주입하고 실행되게 하여 데이터베이스가 비정상적인 동작을 하도록 조작하는 행위입니다.

![image](https://user-images.githubusercontent.com/37327676/177290118-7ea13a47-7454-49a1-af6e-e6a797aaa27d.png)

> SQL Injection 대응방안
- Prepared Statement 구문 사용 : Prepared Statement 구문을 사용하게 되면, 사용자의 입력 값이 데이터베이스의 파라미터로 들어가기 전에 DBMS가 미리 컴파일 하여 실행하지 않고 대기합니다. Spring Mybatis에서 #{}으로 선언하는것과 

