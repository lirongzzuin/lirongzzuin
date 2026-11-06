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
- 개인 서비스를 직접 운영하면서 배포, 모니터링, 장애 대응, API 비용 관리까지 맡고 있습니다. 대표적으로 쿠팡 위탁판매를 사람 없이 돌리는 [무인 운영 시스템](https://github.com/lirongzzuin/coupang-dropship-engine-public)을 홈서버에서 운영 중입니다 (테스트 357개, CI 통과 커밋만 받는 자동 배포·롤백, 감사 로그)

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
저장소마다 README 에 해결한 문제, 설계 이유, 한계와 현재 상태를 솔직하게 적어 두었습니다.

### 운영 중

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [쿠팡 위탁판매 무인 운영 시스템](https://github.com/lirongzzuin/coupang-dropship-engine-public) | 상품 선정 → 등록 → 주문 수집 → 공급처 발주 → 송장 → 정산 대사까지 자동 처리하고 사람은 예외 알림만 처리. 실주문을 지키는 안전 플래그, 상태머신·멱등 처리, 이상 감지 시 자동 판매중지, CI 통과 커밋만 받는 자동 업데이트와 롤백, 개인정보 암호화·감사 로그 | TypeScript, Fastify, PostgreSQL, React, Vitest, GitHub Actions |
| [BeautyPost](https://github.com/lirongzzuin/beautypost-public) | 1인 뷰티샵이 시술 사진을 올리면 인스타·블로그 게시글, 게시용 사진, 릴스 영상을 만들어 주는 서비스 ([beautypost.shop](https://beautypost.shop)). 영상 렌더링 150초 → 4초, Postgres 기반 작업 큐, 무료 AI 한도 안에서 운영 | TypeScript, Hono, React PWA, Neon Postgres, Gemini·Claude API, ffmpeg |
| [소확잼](https://github.com/lirongzzuin/fortune-hub) | 운세·테스트·퀴즈 콘텐츠 웹 서비스 ([sohwakzem.xyz](https://sohwakzem.xyz)). 콘텐츠 33종을 레지스트리 하나로 관리, DB 없이 결정론적 개인화, AdSense 정책에 맞춘 광고 배치 | Next.js 14, Supabase, AdSense, Vercel |
| [육아 영상 자동 편집 파이프라인](https://github.com/lirongzzuin/filmcraft-shorts-pipeline) | 직접 촬영한 가족 영상을 넣으면 편집 기획(plan.json) 검증 → 편집기(FilmCraft)를 MCP 로 원격 조작해 쇼츠·롱폼 빌드 → 규격·음량·자막 겹침 QA → 업로드 일정·배포 → 성과 수집까지 처리하는 개인 채널용 파이프라인 (단위 테스트 122개, 열람 전용 공개 사본) | Python, MCP, Swift(macOS Vision), YouTube API |
| [storage keeper](https://github.com/lirongzzuin/storage-keeper) | 256GB Mac 의 오래된 작업 파일을 외장 SSD 로 해시 검증 후 옮기고 링크로 대체하는 운영 자동화. SSD 연결 감시·자동 재마운트, 복사 중 연결이 끊겨도 원본 보존 | Python, launchd, macOS 시스템 도구 |

### 현장·업무 문제를 푼 프로젝트

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [오피스텔 방문차량 관리](https://github.com/lirongzzuin/officetel-visitor-parking) | 입주민이 휴대폰으로 방문차량을 등록하면 관리사무소 PC 의 에이전트가 기존 주차관제 프로그램 DB 에 반영. 현장 방문이 1~2회뿐이라 진단 도구로 DB 형식을 원격 확인하고, dry-run·자동 업데이트·롤백으로 원격 운영하도록 설계 (실제 건물 적용용, 공개 사본) | Next.js, Supabase, Python, MS Access(ODBC), GitHub Actions |
| [BabyGoGo](https://github.com/lirongzzuin/babygogo) | 내 주변 유아 동반 가능 장소 위치 기반 검색. 카카오·구글·네이버 API 교차 활용, API 비용 제어 설계 | Next.js 14, Supabase, PostGIS, PWA |
| [Bybit 선물 자동매매 v2](https://github.com/lirongzzuin/bybit-futures-bot-v2) | 1시간봉 추세 + 5분봉 진입, 1초 주기 포지션 관리. 실거래·페이퍼 데이터를 분석해 v6 → v17.5 까지 개선 (테스트 105개) | Python, Bybit API, Docker, Fly.io |
| [KIS Trading Alert Bot](https://github.com/lirongzzuin/KIS_Discord_Alert_Bot) | 한국투자증권 OpenAPI 로 체결·자산 변동, ETF 브리핑을 Discord·Telegram 으로 알림 (Fly.io 에 배포해 운영, 현재 중지) | Python, KIS OpenAPI, Discord API |

<details>
<summary>그 외 프로젝트 (프로토타입·학습)</summary>

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [짠내왕](https://github.com/lirongzzuin/jjannaewang) | 생활용품 최저가 추적·특가 알림 토스 앱인토스 미니앱. HMAC 세션 토큰, 가격 이력 통계, 인앱 결제 멱등 처리 | React, Vercel Functions, Supabase, Upstash Redis |
| [KindHeart](https://github.com/lirongzzuin/kindheart) | 후원금 사용 내역을 증빙과 함께 공개하는 후원 플랫폼 프로토타입. 본인확인 CI 해시 저장, DB 제약·트리거로 규칙 강제 | Next.js, Supabase (RLS·트리거) |
| [DROPLY](https://github.com/lirongzzuin/droply) | 한정 수량 아트 드롭·경매 플랫폼 프로토타입. 동시 입찰·오버셀 방지, 결제 서버 검증 | Next.js, Prisma, Upstash Redis, PortOne |
| [AutoPilot](https://github.com/lirongzzuin/autopilot) | AI 업무 보조 SaaS 프로토타입. 멀티 AI 모델 라우터(BYOK·폴백·비용 기록), API 키 암호화 보관 | Next.js 14, Supabase, Prisma |
| [YiwuGo Korea](https://github.com/lirongzzuin/yiwugo-korea) | 중국 이우 도매시장 상품을 한국어로 탐색하는 크로스보더 쇼핑몰 프로토타입 (외부 Open API 연동) | Next.js, NestJS, Expo |
| [World Leaders Missile Volley](https://github.com/lirongzzuin/world-leaders-missile-volley) | 피카츄 배구 오마주 2D 풍자 대전 게임. 클라이언트·서버 공용 물리 모듈, 고정 타임스텝 | Next.js, Canvas, Socket.io |
| [Upbit Bot](https://github.com/lirongzzuin/upbit-bot) · [Bybit v1](https://github.com/lirongzzuin/bybit-futures-bot) · [Binance](https://github.com/lirongzzuin/binance-futures-bot) | 현물·선물 자동매매. 거래소 계층 분리, 단계적 손실 차단, 백테스트 | TypeScript, Python |
| [취향영수증](https://github.com/lirongzzuin/receipt-recap) | 콘텐츠 소비 기록을 영수증 형태로 시각화 | Next.js 15, Prisma, Neon DB, Toss Payments |
| [Job Recommend Bot](https://github.com/lirongzzuin/job-recommend-bot) | 채용 공고를 매일 수집해 조건에 맞는 공고만 추려서 알림 | JavaScript |
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
| Infra | Linux, Shell, Docker, Nginx, GitHub Actions, AWS (EC2/S3), Cloudflare (Workers/Pages/KV/R2), Vercel, Fly.io, macOS launchd |
| Frontend | Next.js, React, Astro, Cordova |
| Automation · AI | Python, Claude Code, Claude API, Discord/Slack 봇, 외부 API 연동 |

---

## Study & Notes

- [What_I_Learned](https://github.com/lirongzzuin/What_I_Learned) · 실무에서 만난 이슈와 해결 과정 기록
- [cs-study](https://github.com/lirongzzuin/cs-study) · OS, DB, Network 정리
- [coding-test-prep](https://github.com/lirongzzuin/coding-test-prep) · 알고리즘·자료구조 풀이

---

경기도 안양 · younggyun12@hotmail.com · [LinkedIn](https://www.linkedin.com/in/younggyunlee)
