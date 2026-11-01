<h1>JaeYoon Sim <sub><sub>심재윤</sub></sub></h1>

**Backend Engineer · Java / Spring**

원인을 데이터로 확인하고, 같은 문제가 반복되지 않게 구조와 기록을 남기는 백엔드 개발자입니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-111111?style=flat-square&logo=notion&logoColor=white)](https://shy-repair-a36.notion.site/40abf7756f8180f783ccd14ce1fa3c6c)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-111111?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/%EC%9E%AC%EC%9C%A4-%EC%8B%AC-732427448/)
[![Claude Skills](https://img.shields.io/badge/Claude_Skills-111111?style=flat-square&logo=anthropic&logoColor=white)](https://github.com/smjae96/claude-skills)

&nbsp;

### About

- 결제 · 예약처럼 정확해야 하는 기능을 설계부터 운영까지 맡아 왔습니다.
- 문제가 생기면 짐작으로 고치지 않고, 실행 계획 · 로그 · 데이터로 원인부터 확인합니다.
- 고친 뒤에는 원인과 해결 과정을 회고로 남겨, 팀이 같은 실수를 반복하지 않게 합니다.
- 반복되는 절차는 Claude Code 스킬로 만들어 팀이 함께 쓰도록 정리합니다.

&nbsp;

### Troubleshooting

운영 중에 겪은 문제를 어떻게 확인하고 해결했는지 정리했습니다.

| | 문제 | 어떻게 풀었나 |
| :-- | :-- | :-- |
| 01 | [상품 목록 조회가 최대 20초까지 느려진 문제](https://shy-repair-a36.notion.site/40abf7756f818010a0f2dfa11abd214f) | 구버전 복원 비교로 가설을 버리고, `EXPLAIN ANALYZE`로 원인 확정 |
| 02 | [AWS RDS MySQL 8.0 → 8.4 메이저 업그레이드](https://shy-repair-a36.notion.site/AWS-RDS-40abf7756f81807aacd2f8f23ac4fb00) | Blue/Green · 런북 · 복제본 검증 후 전환 |
| 03 | [동시 요청에도 견적 · 결제가 어긋나지 않게 만든 잠금 설계](https://shy-repair-a36.notion.site/DB-40bbf7756f8180878f3fc2e895e7b7e9) | 잠금 순서 통일, `REPEATABLE READ` 스냅샷 문제 분석 |
| 04 | [JWT 서명 · 만료 검증 강화와 자동로그인 장애 해결](https://shy-repair-a36.notion.site/JWT-40bbf7756f8180ecbe40e8bd49d25d30) | int 오버플로로 만료 시각이 과거로 찍힌 원인 확정 |
| 05 | [외부 PG사 셀러 계좌 수정 API의 명의 검증 누락 대응](https://shy-repair-a36.notion.site/PG-API-40bbf7756f81807fa3f7ec1c70f7329e) | PG사에 피드백하고, 우리 서버에서 먼저 차단 |
| 06 | [웹소켓 단계별 인가 추가와 순환 의존 해결](https://shy-repair-a36.notion.site/40bbf7756f81809eb0cdc0c27877f4f6) | 순환 의존의 원인을 구분한 뒤 `@Lazy`로 최소 변경 |
| 07 | [이용 제한의 서버 적용과 강제 로그아웃 도구 구현](https://shy-repair-a36.notion.site/40bbf7756f8180b0acf9f3e209c81555) | 판정을 서버 한 곳으로 모으고, 무효화 기준 시각으로 강제 로그아웃 |
| 08 | [SMS 인증을 Redis로 다시 설계](https://shy-repair-a36.notion.site/sms-Redis-40bbf7756f8180d59369f073529a7c5b) | TTL · 원자적 증가로 삭제 배치 · 만료 비교 · 잠금 코드 제거 |

&nbsp;

### Experience

| 기간 | 회사 · 역할 | 한 일 |
| :-- | :-- | :-- |
| 2026.02 – 현재 | **스페이스점프** · 백엔드 개발자 | 중고 거래 · 창업 견적 플랫폼의 Spring 서버 개발 · 운영 |
| 2025.12 – 2026.02 | **굿소프트** · 웹 개발자 | KB차차차 웹/앱 운영, 어드민 기능 FE · BE 개발 |
| 2025.08 – 2025.11 | **메타빌드** · SW 개발자 | 연계 미들웨어(ESB · API 게이트웨이) 설치 · 개발, 이중화 구성 |
| 2024.07 – 2025.07 | **에이디앤스타일** · 백엔드 개발자 | 사내 그룹웨어 구축, 에러 로그 수집 자동화 |

&nbsp;

### Projects

**[claude-skills](https://github.com/smjae96/claude-skills)** — Open Source  
실무에서 AI가 같은 실수를 반복하거나 같은 설명을 매번 하게 될 때, 그 절차를 정리해 만든 Claude Code 스킬 모음. 코드 변경 절차, 프로젝트 간 원인 추적, API 변경 명세, 흐름 기반 QA, 회고 등 11종.

**Funxtion** — 경매형 중고거래 플랫폼 · 팀 프로젝트 · [backend](https://github.com/TeamFunxtion/fx-backend) · [frontend](https://github.com/TeamFunxtion/fx-frontend)  
관심 상품 · 판매자 팔로우 API, WebSocket 1:1 실시간 채팅, 채팅방 안 포인트 기반 안전거래를 개발했습니다.

&nbsp;

### Stack

![Java](https://img.shields.io/badge/Java-111111?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-111111?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-111111?style=flat-square&logo=springsecurity&logoColor=white)
![JPA](https://img.shields.io/badge/JPA_·_QueryDSL-111111?style=flat-square&logo=hibernate&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-111111?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-111111?style=flat-square&logo=redis&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-111111?style=flat-square&logo=amazonwebservices&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-111111?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-111111?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-111111?style=flat-square&logo=linux&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-111111?style=flat-square&logo=anthropic&logoColor=white)

&nbsp;

### Certificate · Education

- **SQL개발자 (SQLD)** · 한국데이터베이스진흥센터 · 2024.12
- **KH정보교육원** · 자바 개발자 과정 · 2023.12 – 2024.06

&nbsp;

<sub>tlawodbs0528@naver.com</sub>
