# 인구 이동 맵(Population Movement Map)
-----------------

## 1. 소개(Intro)
-----------------
- 인구 이동 데이터(전입/전출 자료)를 이용하여, 어디에서 어디로 인구의 이동이 이루어지는지 시각화 도구 제공
- 인구 이동 데이터를 분석하고 분석 결과를 Chart화 하여 출력하는 도구 제공

## 2. 시스템 구성(System Configration)
-----------------
- Back-end Framework: python django
- Front-end Framework: React.js
- Front-end Library: D3.js, jQuery
- Message Queue: RabbitMQ
- Database: PostgreSQL, MongoDB

## 3. 주요 기능(Main Function)
-----------------
#### 3.1 우선 구현 기능
- 일정 지역 내에서의 인구 이동 시각화
- 기종점(O/D)를 선택하여 목적지 별 인구 이동 시각화
- 지도의 단위는 시/군/구까지 지원

#### 3.2 구현 예정 기능
- 데이터 분석 도구 지원
- 기존 인구 전입/전출 데이터를 바탕으로 추가적인 정보를 출력하는 도구
- 해당 도구의 Chart화 도구
- 추가 정보를 바탕으로 인구 이동 시각화 지원

## 4. 데이터 출처(Source of data)
-----------------
- 통계청 마이크로데이터서비스 [[Link](http://mdis.kostat.go.kr/pageLink.do?link=content/blankPage&curMenuNo=MOB_01)]
- 인구 전입/전출과 관련된 데이터 사용
- 현재 2017년 01월 부터 12월까지의 데이터 사용
- 데이터 종류는 아래 참조
- [전라북도 > 도외 전출]
- [도외 > 전라북도 전입]
- [전라북도 내 전입/전출]

## 5. 일정 수립
-----------------
- 2019.01 > 기본 구조 생성, 벡엔드 개발(데이터 파싱 등), 웹 서버 테스트, 기본 서비스 기능 확인
- 2019.02 > message queue 사용 여부 확인 및 적용, 프론트엔드 개발, 우선구현기능 완료
- 2019.03 > 데이터 분석 도구 개발, 향후 개발 일정 수립