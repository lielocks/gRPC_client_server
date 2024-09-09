# QUICK START

### gRPC 를 통해 인증 과정을 거치는 구매 판매 도메인 프로젝트

RESTful API를 활용하여 구매, 판매 주문 CRUD를 수행하는 grpc-client-trade 서버와 grpc-client-trade 와 gRPC를 통해 소통하며, 회원가입 로그인 및 인증을 담당하는 grpc-server-auth 구조의 프로젝트 입니다

<br>


### ERD diagram

![Untitled](https://github.com/user-attachments/assets/482b2159-342b-48c1-a53f-5dd9487e43ca)


## Project

### grpc-client-trade - 자원서버

- grpc-client-trade 서버의 RESTful API 포트는 9999번, grpc 포트는 50052번에서 실행됩니다.

### grpc-server-auth - 인증서버

- grpc-server-auth 서버의 RESTful API 포트는 8888번, grpc 포트는 50051번에서 실행됩니다.

<br>


### 필수 조건

- [필수 소프트웨어] JDK 17 
- [데이터베이스] MariaDB


<br>


### 설치

다음 단계를 따라 프로젝트를 설치해주세요

1. **Repository Clone**

   ```
   git clone https://github.com/lielocks/gRPC_client_server.git
   ```

2. **환경변수 .env 파일 위치**

      env 파일 root : **/src/main/resources/properties/env.properties**

      >
      > ![image](https://github.com/user-attachments/assets/9a81027f-8f40-45bf-8d4e-8718539b5648)
      >

      해당 사진처럼 **`resources 폴더 밑에`** `properties 폴더 생성` 해주시고 **env.properties 명의 파일을 생성해주세요.**

      ![image](https://github.com/user-attachments/assets/f1bb1271-d1d4-49c2-92ef-16fd4d9caec3)

      메일을 통해 전달드릴 env 파일의 형식입니다 . <br> 참고 부탁드립니다.

<br>


### API 명세서 확인 방법

각각의 서버를 구동시킨 후 아래 url 로 접속시 해당 화면을 통해 API 명세서를 확인하실 수 있습니다.

<br>

1. **grpc-client-trade `자원서버`**

- http://localhost:9999/swagger-ui/index.html


> ![image](https://github.com/user-attachments/assets/9067e724-e456-4bc3-a9ec-d8e6863ec3ff)


<br>

2. **grpc-server-auth `인증서버`**

- http://localhost:8888/swagger-ui/index.html

> ![image](https://github.com/user-attachments/assets/f3c0091b-bdd7-45a4-be2c-1901c795688f)

