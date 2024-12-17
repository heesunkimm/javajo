# Spring Legacy Project로 숙박 예약 플랫폼 만들기

## 프로젝트 목적
 - 목표: 게스트는 숙소 검색, 예약, 결제, 위시리스트 관리 기능을 이용할 수 있으며, 호스트는 숙소 등록, 예약 관리, 수익 확인 기능을 제공합니다. 어드민은 계정 관리, 고객 지원, 결제 내역 관리 등을 담당합니다.
 - 주요 기능: 숙소 검색, 예약, 결제, 수익관리, 계정관리 등
 - 개발 기간 : 2024.06.03 ~ 2024.07.16 (총 44일)
 - 개발 인원: 5명 (김미현, 김희선, 원미현, 채성진, 최진영)

## 프로젝트 결과
 - 호스트에서 등록한 숙소 정보를 게스트가 조회하고, 위시리스트 추가 및 삭제 기능을 구현
 - 성수기, 비수기 이용 요금을 다르게 설정, 이용 날짜 선택 시 각 날짜별 숙박비를 책정하여 평균 숙박비용이 표시
 - 카카오맵 API를 이용해 숙소 위치 조회 가능
 - 숙소 관련 문의는 작성자와 해당 숙소의 호스트만 조회 가능하며, 호스트의 답변 상태를 확인 가능
 - 결제는 아임포트 API를 통해 진행, 결제 수단으로 카카오페이 사용, 결제 완료시 예약 내역 페이지에서 예약 내역을 확인 가능
 - 숙소의 예약 내역을 확인할 수 있으며, 이용 날짜 전까지 예약 취소가 가능
 - 이용 날짜가 지나고 숙소 이용이 종료되면 리뷰 작성이 가능하며, 작성한 리뷰는 숙소 리뷰 페이지에서 확인 가능

## 파일구조
    javajo/
    ├── settings/
    ├── src/
    │ ├── main/
    │ │  ├── java/
    │ │  │   └── com/
    │ │  │      └── javajo/
    │ │  │         └── project/
    │ │  │            ├── dto/
    │ │  │            ├── service/
    │ │  │            ├── socialLogin/
    │ │  │            └── Controller Files...
    │ │  ├── resources/
    │ │  │  ├── log4j.xml
    │ │  │  └── application.properties
    │ │  └── Webapp/
    │ │    ├── WEB-INF/
    │ │    │  ├── spring/
    │ │    │  │  ├── appServlet/
    │ │    │  │  └── root-context.xml
    │ │    │  ├── views/
    │ │    │  └── web.xml
    │ │    └── resources/
    │ └── test/
    ├── target/
    ├── .classpath
    ├── .gitignore
    ├── .project
    ├── springBeans
    ├── pom.xml
    └── README.md

## 기술 스택
 - Environment
   - Framework: Spring STS3
   - Build Tool: Maven
   - Database: Oracle
   - Project Type: Spring Legacy Project
  
 - Development
   - Front-end: HTML, CSS, JavaScript, jQuery, JSP, Ajax
   - Back-end: Spring, MyBatis
   - Payment API: import
