# 만들고, 운영하고, 자동화하는 실행형 개발자 강준혁 👋

> 아이디어를 서비스로 만들어 **직접 출시·운영**하고, 반복 업무는 **AI로 자동화**합니다.
> 백엔드·인프라부터 시스템 레벨 검증까지 혼자 끝까지 밀어붙이는 실행형 개발자입니다.

**한국정보통신기술협회(TTA) GS인증 시험원**으로 ISO/IEC 25023·25051 기반 품질 인증을 수행하면서,
사이드로 습관 앱 **'해빗'을 출시·운영**하고 **JDBC 검증·회의록 정리 같은 반복 업무를 코드로 자동화**하고 있습니다.

무엇을 하는 사람이냐면 —

- 🛠 **직접 만들고 출시한다** — Spring Boot 백엔드·인프라를 단독 설계해 iOS·Android 실서비스 운영
- 🤖 **반복 업무를 자동화한다** — n8n · Claude · Gemini로 회의록·검증·행정업무 자동화 (1일 → 1시간, 약 95%↓)
- 🔍 **시스템 레벨까지 파고든다** — API·DB·인증·보안 결함을 코드 단계에서 차단 (약 10만 건 개인정보 보호)

---

## 🚀 Projects

### 1. 해빗 (H-Habit) — 실서비스 운영 중 (2025.08 ~ )
> 습관 인증 앱 · iOS · Android 정식 배포 · 사용자 약 200명 운영 중

[![Google Play](https://img.shields.io/badge/Google_Play-다운로드-414141?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=com.h_habit.app)
[![App Store](https://img.shields.io/badge/App_Store-다운로드-0D96F6?style=for-the-badge&logo=appstore&logoColor=white)](https://apps.apple.com/kr/app/h-habit/id6761158866)

**Stack** Spring Boot · PostgreSQL(Supabase) · Cloudflare R2 · Firebase · AWS Lightsail · GitHub Actions
**Team** 4인 (대표 / PM / **백엔드 · 인프라 단독 담당**)

- Spring Boot 기반 API 서버 **단독 설계 · 구현**, AWS Lightsail · Docker · Nginx 인프라 직접 운영
- GitHub Actions로 빌드 · 테스트 · 배포 파이프라인 자동화
- 관리자 · 사용자 권한별 로그인 시나리오 기능 테스트 통합
- **배포 이후 심각도 높은 결함 0건 유지**

### 2. Altibase JDBC 검증 자동화 — TTA (2025 ~ )
> 국산 상용 DBMS(Altibase 7.3) 기능을 JDBC 기반으로 자동 검증하는 테스트 자동화 프로젝트
> 🔗 [github.com/00KANGJK/altibase-jdbc-automation](https://github.com/00KANGJK/altibase-jdbc-automation)

**Stack** Java 17 · Maven · JUnit 5 · AssertJ · Allure

- CLI 수작업 검증을 **1,000+개 JUnit 테스트 스위트로 자동화** (JDBC 접속 → 케이스별 쿼리 실행 → 기대값 자동 비교)
- 권한 · 캐시 · 경계값처럼 수작업으론 재현이 어려운 **DBMS 결함을 반복 검증으로 탐지 · 리포팅**
- 환경 의존 기능(DB Link · Replication · Backup/Recovery)은 feature flag로 실행 범위 안전 제어

### 3. n8n 회의 자동화 — 노코드 + AI (2025)
> 회의 후처리(회의록 정리 · 할 일 분배)를 자동 파이프라인으로 제거

**Stack** n8n · Gemini · Slack · GitHub

- Google Meet 회의록 → **Gemini로 요약 · 할 일 추출 → 회의록 자동 생성 → Slack · GitHub 이슈 자동 등록**
- 회의 종료 = 정리 · 배분 자동 완료 · 노코드(n8n) + AI로 실제 반복 업무 제거

### 4. 다미화학 홈페이지 — 외주 운영 중 (2025.12 ~ )
> 🔗 [damychem.com](https://damychem.com)

**Stack** Vite · TypeScript · Netlify

- B2B 화장품 원료 업체 소개 페이지 **단독 개발 · 배포 · 운영** (외주 계약 기반)
- AI(Claude)로 개발 사이클 단축, Netlify 배포 + 클라이언트 도메인 · 사내 이메일 연동, 운영 중 업데이트 지속 반영

### 5. ClassHub — 학생 프로젝트 (2024.01 ~ 2024.06)
> 🔗 [github.com/HGU-WALAB/ClassHub](https://github.com/HGU-WALAB/ClassHub)

**Stack** Spring Boot · JPA · MariaDB — 백엔드 개발 · DB 최적화

- SQL 튜닝 + 인덱싱으로 쿼리 성능 개선, API 페이징 처리 및 응답속도 병목 구간 분석, 회귀 테스트 기반 안정성 검증

### 6. 선한영향력가게 리뉴얼 (2024.09 ~ 2024.12)
**Stack** Spring Boot · Spring Security · JPA · MariaDB — 백엔드 · 보안 인증 시스템

- Spring Security 기반 인증 / 권한 관리 시스템 구현, API 보안성 검토 · 예외 처리 강화, GitHub Actions + Cloudtype CI/CD 구축

### 7. CRA 인프라 — 동아리 운영 (2022.08 ~ 2025.02)
**Role** 회장 (한동대 최대 규모 전산 동아리 100명+) · **Stack** Docker · Nginx

- Docker + Nginx 기반 다중 프로젝트 컨테이너 배포 환경 구축, 리버스 프록시로 격리된 테스트 환경 운영, 코드 리뷰 · 크로스체크 프로세스 도입

---

## 🛠 Skills & Tools

### Backend
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![JPA](https://img.shields.io/badge/Spring%20JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)

### Infra / DevOps
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![AWS](https://img.shields.io/badge/AWS%20Lightsail-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare%20R2-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=for-the-badge&logo=netlify&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

### Automation / AI
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=claude&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### QA / Testing
![JUnit5](https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Chrome DevTools](https://img.shields.io/badge/Chrome%20DevTools-4285F4?style=for-the-badge&logo=googlechrome&logoColor=white)
![Invicti](https://img.shields.io/badge/Invicti%20Netsparker-00A4EF?style=for-the-badge&logoColor=white)
![ISO 25000](https://img.shields.io/badge/ISO%2025023%2F25051-FF6B6B?style=for-the-badge&logoColor=white)

### Language / Tools
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white)

---

## 📊 검증 · 품질 실적 (TTA)

> 한국정보통신기술협회(TTA) GS인증 시험원으로 수행한 누적 검증 실적

| 영역 | 경험 |
|------|------|
| 🌐 **웹 / 모바일 앱** | 다수 도메인 (이커머스, B2B SaaS, 교육 등) |
| 🤖 **AI 기반 앱** | 엣지 케이스 TC 설계로 무한 로딩 결함 사전 차단 |
| 🗄️ **DB · 펌웨어** | 데이터 정합성 · 시스템 통신 검증 |
| 📋 **누적 검증 규모** | **15개 제품 / ISO 25023 · 25051 기반** |
| 🧪 **TC 작성 평균** | **프로젝트당 150건 이상** |
| 🛡️ **보안 결함 발견** | **크리티컬 2건 → 약 10만 건 개인정보 보호** |
| ⚡ **업무 자동화** | **Python · AI 활용 / 1일 → 1시간 (약 95% 효율)** |

---

## 🏅 Certifications & Training

- 🏆 **CSTS Foundation Level** (2025.07) — 한국정보통신기술협회
- 📅 **ISTQB CTFL** — 2026.06 응시 예정 (한국어)
- 📚 Playwright 기반 웹 자동화 테스트 실무 기초 — TTA 아카데미 (2026.01)
- 📚 프로젝트 관리와 SW 품질관리 — TTA 아카데미 (2025.10)

---

## 🎓 Education

- 🎓 **숭실대학교 정보과학대학원** — 소프트웨어공학 석사 (2025.09 ~ 재학 중, 4.4 / 4.5)
- 🎓 **한동대학교** — AI 컴퓨터공학 학사 (2019.02 ~ 2025.02, 3.4 / 4.5)

---

## 📈 Currently

- 🔭 TTA에서 **GS인증 시험원**으로 다양한 도메인 제품 품질 검증 수행 중
- 🌱 **해빗(H-Habit)** 앱 운영 (Spring Boot 백엔드 + 인프라 담당)
- 💼 **다미화학 홈페이지** 외주 운영 · 유지보수 중
- 🎯 **직접 만들고 · 운영하고 · 자동화하는** 실행형 포지션으로 성장 중
- 📖 **ISTQB CTFL** 6월 응시 준비 중

---

## 📫 Contact

- 📧 Email: [kth00021000@gmail.com](mailto:kth00021000@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/kjh0210](https://www.linkedin.com/in/kjh0210/)
