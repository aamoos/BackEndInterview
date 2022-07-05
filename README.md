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

>IOC란?
1. 제어의 역전이라고 불림
2. 예전에는 의존관계의 제어를 개발자가 직접 해주었다. 그러나 제어권이 컨테이너로 넘어갔고 객체의 생성부터 생명주기의 관리까지 객체에 대한 제어를 프레임워크에서 하는것을 IOC라고 한다.
