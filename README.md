# 이영균 (Younggyun Lee)

Technical Support Engineer · 백엔드 개발 경험 기반 기술지원 · 업무 자동화

고객이 겪는 문제를 재현하고, 원인을 코드·로그·데이터 수준에서 확인한 뒤, 개발팀과 고객 양쪽이 이해할 수 있는 말로 정리합니다.

[LinkedIn](https://www.linkedin.com/in/younggyunlee) · [Notion Portfolio](https://swamp-force-6e6.notion.site/Developer-YG-s-289e71bb7258468fb045b6d70b54eb10) · younggyun12@hotmail.com

---

## Summary

- 백엔드 개발 3년 5개월 (교환기 연동 모바일 앱 서버 개발 + 서비스 운영 병행)
- 현재 B2B SaaS 기술지원 엔지니어 (풀필먼트 도메인, 2026.03~)
- API·DB·로그를 직접 확인할 수 있어, 단순 문의 전달이 아니라 원인 후보까지 좁혀서 개발팀에 넘깁니다
- 반복되는 문의와 수작업은 스크립트, 체크리스트, 내부 도구로 바꿔 왔습니다
- AI 도구(Claude Code)를 업무와 개인 프로젝트에 적극 활용합니다. 요구사항 정의, 설계 방향 결정, 결과물 검증과 배포·운영을 맡는 방식입니다
- 개인 서비스를 직접 운영하면서 배포, 모니터링, 장애 대응, API 비용 관리까지 맡고 있습니다

---

## Experience

### 두핸즈 (DoHands) · 제품팀 기술지원 엔지니어
2026.03 ~ 현재 · 풀필먼트 SaaS (핸디봇 · 바이스)

- 고객사 기술 문의 접수, 재현, 원인 분석 및 답변
- 이슈를 버그 / 기능개선 / 기능요청으로 분류해 개발팀 백로그(Jira)에 등록하고 처리 상황 추적
- Slack 기술문의 스레드를 정해진 양식의 Jira 티켓으로 옮기는 과정을 AI 워크플로우로 자동화
- 내부 운영용 주문 배정 도구 개발 진행 (Cloudflare Workers, TypeScript/Hono, Queues, KV, D1)
- 반복 문의에 대한 대응 가이드와 기술 문서 정리

### GNTEL · 연구소 개발1팀 백엔드 개발자
2022.10 ~ 2026.03 · 교환기 연동 하이브리드 앱 (mCaller, CallBanner, MobileOffice 등)

서비스 운영 · 장애 대응
- iOS / Android 환경별로 이슈를 분리해 추적하는 방식을 만들어 원인 파악 시간 단축
- 하이브리드 콘텐츠 배포·버전 관리 흐름을 재정비하고 배포 이력 추적·백업 체계 마련
- 반복 배포·점검 작업을 Shell 스크립트와 체크리스트로 표준화해 누락과 재작업 감소
- 고객사·영업·개발 사이에서 장애 원인과 조치 계획을 정리해 공유

기능 개발 · 유지보수
- OTP 로그인(SMS / FCM Push), 조직도·주소록, 사용자·권한 관리 기능 개발
- Swagger 기반 API 문서화, 공통 응답·에러 처리 구조 정비

---

## How I Handle Issues

| 단계 | 하는 일 |
|---|---|
| 정리 | 고객이 원하는 결과와 현재 상황, 환경(버전·권한·데이터)을 분리해서 적습니다 |
| 재현 | 환경·단계·기대값·실제값을 고정하고 같은 조건에서 재현합니다 |
| 원인 확인 | API 요청/응답, 로그, DB 데이터를 직접 보고 원인 후보를 좁힙니다 |
| 전달 | 개발팀에는 재현 절차와 근거를, 고객에게는 영향 범위와 선택지를 전달합니다 |
| 재발 방지 | 같은 문의가 반복되면 문서, 체크리스트, 자동화로 바꿉니다 |

---

## Selected Projects

직접 기획하고 AI 도구(Claude Code)로 구현해 배포·운영한 프로젝트입니다. 제 역할은 문제 정의, 기능 범위 설정, 구조 결정, 결과물 검증, 배포 후 운영입니다.

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [BeautyPost](https://github.com/lirongzzuin/beautypost-public) | 1인 뷰티샵이 시술 사진을 올리면 인스타·블로그 게시글, 게시용 사진, 릴스 영상을 만들어 주는 서비스. 2026.10~ 운영 중 ([beautypost.shop](https://beautypost.shop)) | TypeScript, Hono, React PWA, Neon Postgres, Gemini·Claude API, ffmpeg |
| [BabyGoGo](https://github.com/lirongzzuin/babygogo) | 내 주변 유아 동반 가능 장소 위치 기반 검색. 카카오·구글·네이버 API 교차 활용, API 비용 제어 설계 | Next.js 14, Supabase, PostGIS, PWA |
| [KIS Discord Alert Bot](https://github.com/lirongzzuin/KIS_Discord_Alert_Bot) | 한국투자증권 OpenAPI로 잔고·체결 변동을 Discord로 알림. 상시 운영 중 | Python, KIS OpenAPI, Discord API |
| [Job Recommend Bot](https://github.com/lirongzzuin/job-recommend-bot) | 채용 공고를 매일 수집해 조건에 맞는 공고만 추려서 알림 | JavaScript |
| 소확잼 | 운세·테스트·퀴즈 콘텐츠 웹 서비스. 운영 중 ([sohwakzem.xyz](https://sohwakzem.xyz)) | Next.js 14, Supabase, AdSense |
| 자동매매 시스템 | 국내·해외 주식과 암호화폐 거래소 API 연동 자동매매·모니터링. 장애 알림, 테스트 코드, 컨테이너 배포 적용 | Python, TypeScript, Docker, Fly.io, Oracle Cloud |

링크가 없는 프로젝트는 비공개 저장소입니다. 필요하시면 코드와 운영 내역을 따로 공유드리겠습니다.

<details>
<summary>그 외 프로젝트</summary>

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| AutoPilot | 이메일 분류, 자동 응답, 업무 워크플로우 자동화 | Next.js 14, Supabase, Prisma |
| 돌봄다리 | 가족 돌봄 인력과 수요자 매칭 | Astro 5, Cloudflare D1/R2/KV, Claude API |
| 짠내왕 | 최저가 추적·절약 팁 공유 | Next.js, Supabase, Upstash Redis |
| [취향영수증](https://github.com/lirongzzuin/receipt-recap) | 콘텐츠 소비 기록을 영수증 형태로 시각화 | Next.js 15, Prisma, Neon DB, Toss Payments |
| [Crypto Auto Trade](https://github.com/lirongzzuin/Crypto_Auto_Trade_for_Upbit_and_Binance) | Upbit·Binance 시세 모니터링과 자동매매 | Python |
| [TrendHive](https://github.com/lirongzzuin/TrendHive) | 트렌드 공유·댓글 플랫폼 (JWT 인증, Docker) | Java, Spring Boot, MySQL |
| [voucher-booking-server](https://github.com/lirongzzuin/voucher-booking-server) | 바우처 관리·회의실 예약 서버 | Java, Spring Boot |
| [FastChat](https://github.com/lirongzzuin/FastChat) | WebSocket 실시간 채팅 | Java, Spring Boot |
| [FlashPay](https://github.com/lirongzzuin/FlashPay) | 결제 트랜잭션 처리 구조 설계 | Java, Spring Boot |
| [MoodPress](https://github.com/lirongzzuin/moodpress) | 감정 기반 문장 생성·공유 | TypeScript, Next.js |
| [BlameDetector](https://github.com/lirongzzuin/blame-detector) | 대화 스크린샷 기반 과실 분석 | JavaScript |

</details>

---

## Skills

| 분류 | 내용 |
|---|---|
| 기술지원 · 운영 | 이슈 재현·분석, 로그 확인, API 테스트(Postman, Swagger), Jira 이슈 관리, 기술 문서 작성 |
| Backend | Java, Spring Boot, JPA, REST API, JWT, Node.js, TypeScript |
| Database | MySQL, MariaDB, PostgreSQL, SQLite, Supabase, Cloudflare D1 |
| Infra | Linux, Shell, Docker, Nginx, GitHub Actions, AWS (EC2/S3), Cloudflare (Workers/Pages/KV/R2), Vercel, Fly.io |
| Frontend | Next.js, React, Astro, Cordova |
| Automation · AI | Python, Claude Code, Claude API, Discord/Slack 봇, 외부 API 연동 |

---

## Study & Notes

- [What_I_Learned](https://github.com/lirongzzuin/What_I_Learned) · 실무에서 만난 이슈와 해결 과정 기록
- [cs-study](https://github.com/lirongzzuin/cs-study) · OS, DB, Network 정리
- [coding-test-prep](https://github.com/lirongzzuin/coding-test-prep) · 알고리즘·자료구조 풀이

---

경기도 안양 · younggyun12@hotmail.com · [LinkedIn](https://www.linkedin.com/in/younggyunlee)
