# Introduction

[2021년 제4회 KB국민은행 소프트웨어 경진대회](http://www.kbsccoding.com/) 프론트엔드 저장소

## Stack
- Frontend : React, Typescript

## Features
### 1. 로그인 기능 구현
- API key 입력 후 버튼 클릭 시 백엔드에 로그인 요청 전송(`POST`)
- 로그인 성공 시 홈 페이지로 이동, 로그인 실패 시 메세지 화면 표시

### 2. 보유 코인 정보 화면 표시
- 버튼을 통해 보유 코인 및 상위 20개 코인 정보 확인 가능
- 전일 거래 정보 요청(`GET`)
  - 보유하고 있는 코인 정보 요청
  - 상위 20개 코인 정보 요청
- 실시간 변동되는 정보 요청(`GET`)
  - 10초에 1번씩 백엔드에 최신 정보 요청
  - 보유하고 있는 코인의 실시간으로 변동되는 정보 요청
  - 상위 20개 코인 정보의 실시간으로 변동되는 정보 요청
- 각 코인 클릭 시 세부 정보 화면 별도 표시

### 3. 거래 시작/종료
- 거래 시작 버튼 클릭 시 백엔드에 거래 시작 요청 전송(`GET`)
  - 거래 시작 버튼이 종료 버튼으로 변경됨
  - 백엔드에서는 작성된 로직에 따라 자동 거래 진행, 로그 기록
- 거래 종료 버튼 클릭 시 백엔드에 거래 종료 요청 전송(`GET`)
  - 기록된 거래 로그를 받아서 프론트에 표시