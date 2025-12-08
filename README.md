# 이영균 (Younggyun Lee) 
| Backend Developer · Product Manager Candidate

---

## 소개

저는 Java와 Spring Boot를 중심으로 **실시간 처리 시스템**을 설계·구현해 온 백엔드 개발자입니다. Kafka, Redis, WebSocket, JWT 인증, Docker 기반 배포 자동화 등 실무 전반을 다루며, 사용자의 문제를 **정의하고 운영에 강한 서비스**로 연결하는 데 집중하도록 노력해 왔습니다. 
최근에는 제품 관점에서 **지표·실험·운영 프로세스**까지 책임지는 **PM 역할**을 준비하고 있습니다.

저의 핵심 역량은 다음과 같다고 생각합니다.

- **실시간 시스템 설계**: Kafka/Redis, WebSocket
- **운영 친화적 백엔드**: Swagger 명세, 로깅·모니터링, 구성 표준화, 배포 자동화(SH 스크립트)
- **하이브리드 앱 연동**: Cordova 기반 iOS/Android 클라이언트와 Spring Boot 서버 연동
- **프로덕트 마인드셋**: 요구 수집 → 정의 → 설계/개발 → 검수/배포 → 지표/피드백 기반 개선의 전 사이클 경험

현재는 개발자 경험을 바탕으로 **PM/PO 트랙**으로 역할을 확장하고 있으며, **데이터와 사용자 가치**를 중심에 둔 제품 운영을 지향합니다.

---

## 주요 경력 하이라이트

- **GNTEL 연구소 개발1팀 (2022 ~ 현재)**  
  - 교환기 연결을 통한 사내전화와 내 휴대전화를 연결하여 사생활을 보호할 수 있는 하이브리드 앱(mCaller, CallBanner, MobileOffice 등), Spring Boot 백엔드 개발 및 연동
  - OTP/FCM Push 로그인, 조직도/주소록, 버전 컨트롤, 원격 배포 자동화(SH) 등 기능 개발·운영
  - 서버 배포 파이프라인과 하이브리드 컨텐츠 배포 자동화(타임스탬프 버전, 백업·이력 관리) 설계
  - iOS FCM Push OTP 초기화 오류 분석 및 onDeviceReady() 재구성 등 플랫폼 이슈 해결

- **실시간 메시징/거래 자동화 사이드 프로젝트**  
  - 한국투자증권(KIS)·Upbit API 기반 **자동 잔고 브리핑/체결 알림/자동매매** 시스템 개발
  - Slack/Telegram/Discord 연동, 브리핑 포맷, 실패 종목 스킵 및 재시도, 레이트 리밋 제어
  - RSI/MACD/ADX/Supertrend, ICT 지표 조합, 트레일링 스탑 등 매매 전략 연구 및 운용 자동화

---

## 대표 사이드 프로젝트

| 프로젝트 | 요약 | 역할 | 링크 |
|---|---|---|---|
| TrendHive | Spring Boot + JWT 기반 트렌드 공유 플랫폼. 트렌드/댓글 도메인, Swagger, Docker+MySQL | 설계·백엔드·배포 | https://github.com/lirongzzuin/TrendHive |
| FastChat | WebSocket + Redis 캐시 기반 실시간 채팅. JWT, Swagger, ChatMessageDTO, Kafka/Redis 연동 | 서버 아키텍처·백엔드 | https://github.com/lirongzzuin/FastChat |
| FlashPay | Kafka + Redis로 멱등·분산 락 기반 결제 트랜잭션 처리. 장애/유실 대비 구조 | 백엔드·메시징 설계 | https://github.com/lirongzzuin/FlashPay |
| MoodPress | 감정 선택형 문장 생성/공유 웹. 모바일 중심 UX, 광고 수익화(쿠팡 파트너스) | 기획·FE/BE·분석 | https://github.com/lirongzzuin/moodpress |
| BlameDetector | 대화 스크린샷 기반 과실 비율 분석 Web. 공유 중심 UX, 무료 AI API 우선 | 기획·FE/BE | https://github.com/lirongzzuin/BlameDetector |

> 추가: 자동매매/알림 봇, 버전·배포 자동화 도구, Cordova 플러그인 연동 샘플 등은 비공개 저장소 또는 사내 레포지토리로 운영했습니다.

---

## 제품(PO/PM) 관점의 강점

- **문제 정의**: 현업/운영의 언어로 요구를 정리하고 개발 태스크로 변환합니다.
- **지표 운영**: GA/로그 기반으로 전환·잔존·오류율을 추적하고, A/B 또는 단계적 롤아웃으로 개선합니다.
- **프로세스 설계**: 체크리스트/표준 템플릿, 재현 가능한 배포 스크립트로 누락·재작업을 줄입니다.
- **기술 커뮤니케이션**: 설계 배경·트레이드오프·대안까지 문서화하며, 개발/디자인/운영과 합의합니다.

---

## 기술 스택

**Backend**: Java, Spring Boot, JPA, REST, JWT 
**Real-time/Messaging**: Kafka, Redis, WebSocket 
**Infra/DevOps**: Docker, Shell(SH), Nginx, GitHub Actions, AWS(EC2/S3)  
**DB**: MySQL, MariaDB  
**Frontend/Client**: Javascript, Cordova  
**Tools**: Swagger, Postman, Slack

---

## 공개 학습/정리

- coding-test-prep: 알고리즘/자료구조 풀이 정리 – https://github.com/lirongzzuin/coding-test-prep  
- cs-study: OS/DB/Network 등 CS 이론 – https://github.com/lirongzzuin/cs-study  
- What_I_Learned: 이슈·해결·설계 의도 기록 – https://github.com/lirongzzuin/What_I_Learned

---

## 연락처·포트폴리오

- 위치: 인천, 대한민국  
- 이메일: younggyun12@hotmail.com  
- LinkedIn: https://www.linkedin.com/in/%EC%98%81%EA%B7%A0-%EC%9D%B4-b2b4532b6  
- Notion 포트폴리오: https://swamp-force-6e6.notion.site/Developer-YG-s-289e71bb7258468fb045b6d70b54eb10?pvs=4
