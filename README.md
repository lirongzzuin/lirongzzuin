# 이영균 (Younggyun Lee)
Backend Engineer · IT Manager/Tech Support · Product & Operations

---

## 소개

안녕하세요. 저는 Java와 Spring Boot를 중심으로 백엔드 개발과 운영 업무를 함께 경험해 왔습니다.  
업무에서는 하이브리드 앱(Cordova)과 서버를 연동하는 기능 개발, 인증/로그인 흐름(OTP 포함) 구성, 조직도·주소록 같은 사내 기능 운영, 그리고 배포/버전 관리와 같은 반복 작업을 자동화하는 일을 주로 맡아왔습니다.

제가 지향하는 방식은 “개발만 잘하는 사람”보다는, 운영에서 실제로 문제가 덜 생기고 문제가 생기면 빨리 원인을 좁혀 해결할 수 있는 구조를 만드는 쪽에 가깝습니다.  
그래서 Backend뿐 아니라 IT Manager, Technical Support처럼 운영과 커뮤니케이션 비중이 큰 역할도 자연스럽게 관심을 갖게 되었습니다.

---

## 제가 일하는 방식

- 요구사항을 받을 때 먼저 “원하는 결과”와 “운영 제약(환경, 권한, 일정 등)”을 분리해서 정리합니다.
- 이슈가 생기면 재현 조건(환경/단계/기대값/실제값)을 먼저 고정하고, 원인 후보를 좁혀가며 해결합니다.
- 반복 작업은 체크리스트나 스크립트로 표준화해서, 누락과 재작업을 줄이려고 합니다.
- 개발/운영/현업 등 관점이 다른 사람들과도 같은 목표를 보게 만드는 커뮤니케이션을 중요하게 생각합니다.

---

## 경력 하이라이트

### GNTEL 연구소 개발1팀 (2022 ~ 현재)

- 교환기 연동 기반 하이브리드 앱(mCaller, CallBanner, MobileOffice 등)과 Spring Boot 백엔드 기능 개발 및 운영
- OTP 기반 로그인(SMS/FCM Push), 조직도/주소록, 사용자/권한 관련 기능 개발 및 유지보수
- 하이브리드 컨텐츠 배포 및 버전 관리 흐름 개선(배포 이력 관리, 백업 파일 관리 등)
- iOS 환경에서 발생한 FCM Push OTP 관련 초기화 이슈 분석 및 로그인 초기 구동 로직 개선

---

## IT Manager / Tech Support 관점에서 해온 일

- 장애/이슈 대응 시, 재현 가능한 정보(환경, 단계, 로그, 기대값/실제값)를 먼저 정리하고 해결 방향을 좁혀왔습니다.
- 배포/운영 과정에서 반복되거나 실수하기 쉬운 작업을 스크립트와 체크리스트로 정리해 누락을 줄였습니다.
- 하이브리드 앱 특성상 iOS/Android에서 다르게 발생하는 이슈를 분리해 추적하고, 원인을 좁혀 해결했습니다.
- 기술적인 내용을 기획/운영 관점에서도 이해할 수 있도록 설명하고, 선택지와 트레이드오프를 정리해 공유했습니다.

---

## Backend 관점에서 해온 일

- Spring Boot 기반 REST API 개발 및 유지보수
- 로그인/인증 흐름 구성(OTP 포함) 및 운영 이슈 대응
- API 문서화(Swagger), 공통 응답/에러 처리 등 협업을 위한 기본 품질 정리
- 운영에 필요한 로그/설정 정리와 배포 자동화 흐름 개선(Shell 기반)

---

## 사이드 프로젝트

업무에서의 기술 경험을 넓히기 위해, 아래 프로젝트들을 개인적으로 설계하고 구현했습니다.  
다만 Kafka/Redis 같은 기술은 실무에서 깊게 사용한 경험이라기보다는, 사이드 프로젝트에서 필요한 범위로 적용하며 익혔습니다.

| 프로젝트 | 요약 | 역할 | 링크 |
|---|---|---|---|
| TrendHive | 트렌드 공유/댓글 중심의 간단한 플랫폼. JWT 인증, Docker + MySQL 구성 | 설계·백엔드·배포 | https://github.com/lirongzzuin/TrendHive |
| FastChat | WebSocket 기반 실시간 채팅 실험 프로젝트. 캐시/메시징 요소를 일부 적용하며 구조를 학습 | 설계·백엔드 | https://github.com/lirongzzuin/FastChat |
| FlashPay | 결제 트랜잭션 처리 구조를 학습하기 위한 프로젝트. 장애/유실 케이스를 가정하고 설계 연습 | 설계·백엔드 | https://github.com/lirongzzuin/FlashPay |
| MoodPress | 감정 선택 기반 문장 생성/공유 웹. 모바일 중심 UX 구성 | 기획·FE/BE | https://github.com/lirongzzuin/moodpress |
| BlameDetector | 대화 스크린샷 기반 과실 분석 서비스 기획/구현 프로젝트 | 기획·FE/BE | https://github.com/lirongzzuin/BlameDetector |

---

## 기술 스택

**Backend**: Java, Spring Boot, JPA, REST, JWT  
**DB**: MySQL, MariaDB  
**Client/Frontend**: JavaScript, Cordova  
**Infra/DevOps**: Docker, Shell(SH), Nginx, GitHub Actions, AWS(EC2/S3)  
**Tools**: Swagger, Postman, Slack  

*Kafka/Redis 등은 사이드 프로젝트에서 필요한 범위로 적용해본 경험이 있습니다.*

---

## 공개 학습/정리

- coding-test-prep: 알고리즘/자료구조 풀이 정리 – https://github.com/lirongzzuin/coding-test-prep  
- cs-study: OS/DB/Network 등 CS 이론 – https://github.com/lirongzzuin/cs-study  
- What_I_Learned: 이슈·해결·설계 의도 기록 – https://github.com/lirongzzuin/What_I_Learned  

---

## 연락처·포트폴리오

- 위치: 경기도, 대한민국  
- 이메일: younggyun12@hotmail.com  
- LinkedIn: https://www.linkedin.com/in/%EC%98%81%EA%B7%A0-%EC%9D%B4-b2b4532b6  
- Notion 포트폴리오: https://swamp-force-6e6.notion.site/Developer-YG-s-289e71bb7258468fb045b6d70b54eb10?pvs=4  
