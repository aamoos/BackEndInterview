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
> DI란?
- Dependency Injection의 줄임말로, 의존성주입 이라고 한다.

> Dependency Injection 방법
- @Autowird를 사용한 DI(타입 주입)
- 
![image](https://user-images.githubusercontent.com/37327676/177282715-1dd9cd0c-f2e9-462f-bcb7-25324258a897.png)

- @AllArgsConstructor를 통한 주입
- 
![image](https://user-images.githubusercontent.com/37327676/177282921-2da95c73-55fe-4136-9273-f5050799e125.png)

- @RequiredArgsConstructor를 통한 주입
- 
![image](https://user-images.githubusercontent.com/37327676/177283017-087062ec-ad75-44fc-aefd-2ad76968a384.png)

- @Setter를 통한 

> AOP란?

>IOC란?
