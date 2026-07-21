# 만들고, 운영하고, 자동화하는 실행형 개발자 강준혁 👋

> 아이디어를 서비스로 만들어 **직접 출시·운영**하고, 반복 업무는 **AI로 자동화**합니다.
> 백엔드·인프라부터 시스템 레벨 검증까지 혼자 끝까지 밀어붙이는 실행형 개발자입니다.

현재 **한국정보통신기술협회(TTA) GS인증 시험원**으로 ISO/IEC 25023·25051 기반 소프트웨어 품질 인증을 수행하고 있습니다.

**주요 실적**

- 🛠 **직접 만들고 출시한다** — Spring Boot 백엔드·인프라를 단독 설계해 iOS·Android 실서비스 운영
- 🤖 **반복 업무를 자동화한다** — n8n · Claude · Gemini로 회의록·검증·행정업무 자동화 (1일 → 1시간, 약 95%↓)
- 🔍 **시스템 레벨까지 파고든다** — JDBC로 DBMS를 코드 검증해 권한·캐시·경계값 결함까지 탐지

---

## 🚀 Projects

### 1. 해빗 (H-Habit) — 실서비스 운영 중 (2025.08 ~ )
> 습관 인증 앱 · iOS · Android 정식 배포 · **실사용자 154명** 운영 중 (2026.07 기준)

[![Google Play](https://img.shields.io/badge/Google_Play-다운로드-414141?style=for-the-badge&logo=googleplay&logoColor=white)](https://play.google.com/store/apps/details?id=com.h_habit.app)
[![App Store](https://img.shields.io/badge/App_Store-다운로드-0D96F6?style=for-the-badge&logo=appstore&logoColor=white)](https://apps.apple.com/kr/app/h-habit/id6761158866)

**Stack** Spring Boot · PostgreSQL(Supabase) · Cloudflare R2 · Firebase · AWS Lightsail · GitHub Actions
**Team** 4인 팀 · 본인은 **백엔드 · 인프라 단독 + PM**

- API 서버 **단독 설계·구현** + AWS Lightsail·Docker·Nginx 인프라 직접 운영, GitHub Actions CI/CD 자동화
- **4주 리텐션 66%** · 누적 인증 7,063건 · 총 습관 수행 806시간
- **배포 이후 심각도 높은 결함 0건 유지**

### 2. Altibase JDBC 검증 자동화 — TTA (2025 ~ )
> 국산 상용 DBMS(Altibase 7.3) 기능을 JDBC 기반으로 자동 검증하는 테스트 자동화 프로젝트
> 🔗 [github.com/00KANGJK/altibase-jdbc-automation](https://github.com/00KANGJK/altibase-jdbc-automation)

**Stack** Java 17 · Maven · JUnit 5 · AssertJ · Allure

- CLI 수작업 검증을 **1,000+개 JUnit 테스트 스위트로 자동화** (JDBC 접속 → 케이스별 쿼리 실행 → 기대값 자동 비교)
- 권한·캐시·경계값처럼 수작업으론 재현이 어려운 **DBMS 결함을 반복 검증으로 탐지·리포팅**, 환경 의존 기능은 feature flag로 실행 범위 안전 제어

### 3. n8n 회의 자동화 — 노코드 + AI (2025)
> 회의 후처리(회의록 정리 · 할 일 분배)를 자동 파이프라인으로 제거

**Stack** n8n · Gemini · Slack · GitHub

- Google Meet 회의록 → **Gemini로 요약·할 일 추출 → 회의록 자동 생성 → Slack·GitHub 이슈 자동 등록** = 정리·배분 자동 완료

### 4. 다미화학 홈페이지 — 외주 운영 중 (2025.12 ~ )
> 🔗 [damychem.com](https://damychem.com)

**Stack** Vite · TypeScript · Netlify

- B2B 화장품 원료 업체 소개 페이지 **단독 개발·배포·운영**(외주 계약 기반), Claude로 개발 사이클 단축 + 도메인·사내 이메일 연동·지속 유지보수

### 5. ClassHub — 학생 프로젝트 (2024.01 ~ 2024.06)
> 🔗 [github.com/HGU-WALAB/ClassHub](https://github.com/HGU-WALAB/ClassHub)

**Stack** Spring Boot · JPA · MariaDB

- SQL 튜닝·인덱싱으로 쿼리 성능 개선, API 페이징 처리 및 응답속도 병목 분석, 회귀 테스트 기반 안정성 검증

---

## 🛠 Skills & Tools

> 가장 자주 사용하는 핵심 스택 — 🟢 **능숙**: 주도적으로 사용 · 🟡 **활용**: 실무 활용 경험

### 🟢 능숙
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![AWS](https://img.shields.io/badge/AWS%20Lightsail-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

### 🟡 활용
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Claude](https://img.shields.io/badge/Claude-D97757?style=for-the-badge&logo=claude&logoColor=white)

---

## 📊 검증 · 품질 실적 (TTA)
> GS인증 시험원으로 수행한 누적 검증 실적 (ISO/IEC 25023 · 25051 기반)

| 영역 | 경험 |
|------|------|
| 📋 **누적 규모** | **16개 제품 GS인증 완료 · 17번째 진행 중** |
| 🌐 **검증 도메인** | 웹 · 모바일 · AI · DB · 펌웨어 (이커머스 · B2B SaaS · 교육 등) |
| ⚡ **업무 자동화** | **Python · AI로 반복 검증·행정업무 1일 → 1시간 (약 95%↓)** |

---

## 🏅 Certifications & Training
- 🏆 **ISTQB CTFL** — 취득 (2026.06, 한국어)
- 🏆 **CSTS Foundation Level** — 취득 (2025.07, 한국정보통신기술협회)
- 📚 Playwright 기반 웹 자동화 테스트 실무 기초 — TTA 아카데미 (2026.01)
- 📚 프로젝트 관리와 SW 품질관리 — TTA 아카데미 (2025.10)

---

## 🎓 Education
- 🎓 **숭실대학교 정보과학대학원** — 소프트웨어공학 석사 (2025.09 ~ 재학 중, 4.4 / 4.5)
- 🎓 **한동대학교** — AI 컴퓨터공학 학사 (2019.02 ~ 2025.02, 3.4 / 4.5)

---

## 📈 Currently
- 🔭 TTA에서 **GS인증 시험원**으로 품질 검증 수행 중 — **현재 17번째 제품 GS인증 시험 진행**
- 🌱 **해빗(H-Habit)** 앱 운영 (Spring Boot 백엔드 + 인프라 담당) · 실사용자 154명
- 💼 **다미화학 홈페이지** 외주 운영 · 유지보수 중

---

## 📫 Contact
- 📧 Email: [kth00021000@gmail.com](mailto:kth00021000@gmail.com)
- 💼 LinkedIn: [linkedin.com/in/kjh0210](https://www.linkedin.com/in/kjh0210/)
