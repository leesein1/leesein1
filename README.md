<div align="center">

# Sein Lee

### .NET Backend · Full-Stack Developer

**실제 업무와 생활에서 발생하는 반복 작업을 자동화하고,  
기존 시스템을 더 나은 구조로 개선하는 개발자입니다.**

C# / .NET을 중심으로 백엔드와 데이터베이스를 다루며,  
React + TypeScript 기반 프론트엔드까지 확장해 서비스를 직접 설계하고 운영합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-111827?style=flat-square&logo=githubpages&logoColor=white)](https://leesein1.github.io)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/leesein1)

</div>

---

## Featured Projects

### 🚗 FaultMon — Real-time Vehicle Fault Monitoring

> **Legacy .NET MVC 시스템을 React + ASP.NET Core Web API 구조로 리뉴얼한 실시간 차량 고장 관제 시스템**

실무에서 경험한 관제 시스템을 개인 프로젝트로 재구현한 뒤,  
기존 Front/Backend 통합형 MVC 구조를 **React SPA + ASP.NET Core API**로 분리하여 리뉴얼했습니다.

- 실시간 장애/고장 이벤트 수신 및 관제
- SignalR 기반 실시간 통신
- Kakao Map 기반 GPS 위치 시각화
- 검색 / 상세 / 통계 / 상태별 관제 화면
- 기존 MVC 구조 → Front / API 분리 리팩터링

**Current Architecture**

`FaultMon-Front (React)` ↔ `REST API / SignalR` ↔ `SeinServices.Api (.NET 8)` ↔ `MSSQL`

**Repositories**  
[Frontend - FaultMon-Front](https://github.com/leesein1/FaultMon-Front) · [Backend - SeinServices.Api](https://github.com/leesein1/08.SeinServices.Api) · [Legacy V1 - FaultMon](https://github.com/leesein1/FaultMon)

`React` `Vite` `ASP.NET Core` `SignalR` `MSSQL` `Kakao Map`

---

### 🏡 Chungyak Manager — Housing Subscription Automation

> **매일 직접 확인하던 청약 공고 수집·변경 감지·마감·알림 과정을 자동화한 개인 서비스**

실제 청약 정보를 관리하면서 느낀 반복 작업을 줄이기 위해 만들었습니다.
외부 API 데이터를 수집하고 DB에 동기화한 뒤, 프론트엔드에서 조회하고 알림까지 이어지는 구조입니다.

- 공공주택 모집공고 자동 수집 및 DB 동기화
- 신규 / 일정 변경 / 상태 변경 감지
- 마감 공고 자동 처리
- 즐겨찾기 및 알림 관리
- GitHub Actions 기반 외부 스케줄 실행
- React 기반 대시보드 / 검색 / 상세 화면

**Repositories**  
[Frontend - chungyak_manage_web](https://github.com/leesein1/chungyak_manage_web) · [Backend - SeinServices.Api](https://github.com/leesein1/08.SeinServices.Api)

`React` `ASP.NET Core` `Azure SQL` `GitHub Actions` `Slack`

---

### ⚙️ Monthly Excel — Business Automation Tool

> **실제 반복 업무를 줄이기 위해 제작하고 실사용 중인 WinForms 기반 업무 자동화 프로그램**

엑셀과 웹 브라우저를 반복해서 오가며 처리하던 업무를 자동화하기 위해 시작했고,  
실제 사용자 피드백을 반영하며 여러 업무 도구를 하나의 프로그램으로 확장했습니다.

- 네이버 카페 데이터 수집 및 Excel 정리
- WebView2 기반 블로그 업무 지원
- 이미지 일괄 변환 / 미리보기
- 키워드 정리 / 검사기 / 번역 도구
- 비동기 처리 및 CancellationToken 기반 취소
- GitHub Releases 기반 배포 / 자동 업데이트 구조

[Repository - Monthly_Excel](https://github.com/leesein1/Monthly_Excel)

`.NET 8` `WinForms` `WebView2` `Selenium` `ClosedXML` `ImageSharp`

---

### 💍 Wedding Template — Mobile Wedding Invitation

> **실제 결혼식을 위해 직접 제작한 React + TypeScript 모바일 청첩장**

React와 TypeScript 학습을 실제 서비스 제작으로 연결한 프로젝트입니다.
모바일 환경을 중심으로 사용자 경험과 인터랙션을 직접 구현했습니다.

- 모바일 퍼스트 반응형 UI
- 이미지 갤러리 / 터치·드래그 인터랙션
- Kakao Map 위치 안내
- 실시간 예식일 카운트다운
- 계좌 복사 / 식순 / 배경음악 등 실제 청첩장 기능

[Repository - wedding-template](https://github.com/leesein1/wedding-template)

`React` `TypeScript` `Vite` `Tailwind CSS` `Kakao Map`

---

## Backend Platform

### 🔧 SeinServices.Api

개인 프로젝트별 백엔드를 하나의 ASP.NET Core Web API 서버에서 관리하는 **통합 Backend Platform**입니다.

```text
SeinServices.Api
├─ FaultMon
│  ├─ REST API
│  ├─ SignalR Hub
│  └─ Scheduler
│
└─ Chungyak
   ├─ Public API Sync
   ├─ Search / Favorite
   ├─ Close / Alarm Jobs
   └─ Slack Notification
```

- Controller / Service / Data 계층 분리
- Swagger API 문서화
- Scheduler / GitHub Actions 연동
- Docker 기반 배포 경험
- 운영 환경의 UTC/KST 시간대 문제 및 Cold Start 이슈 대응

[Repository - 08.SeinServices.Api](https://github.com/leesein1/08.SeinServices.Api)

---

## Tech Stack

**Backend**  
![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Classic ASP](https://img.shields.io/badge/Classic%20ASP-555555?style=flat-square&logo=windows&logoColor=white)

**Frontend**  
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

**Database / Infra**  
![MSSQL](https://img.shields.io/badge/MSSQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

---

## Study & Practice

대표 프로젝트와 별도로 CS 기초와 새로운 기술을 꾸준히 학습하고 기록합니다.

- [CS Study](https://github.com/leesein1/cs-) — 자료구조 / 알고리즘 / OS / Network / Database
- [Programmers](https://github.com/leesein1/programmers) — 알고리즘 문제 풀이
- [React Study](https://github.com/leesein1/React-Study) — React / Hooks 학습 기록
- [TypeScript Study](https://github.com/leesein1/TypeScript-Study) — TypeScript 기초 학습 기록

---

<div align="center">

### Build things that solve real problems.

**반복되는 불편을 발견하고, 코드로 줄이고, 더 나은 구조로 다시 개선합니다.**

</div>
