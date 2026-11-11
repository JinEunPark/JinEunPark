<h2 align="center">안녕하세요, 백엔드 개발자 박진은입니다 👋</h2>
<p align="center">문제의 원인을 끝까지 추적해 구조로 해결하고, 장애에 강하고 운영하기 쉬운 서버를 만듭니다.</p>

<p align="center">
  <a href="https://rekit.co.kr"><img src="https://img.shields.io/badge/rekit-rekit.co.kr-0e75b6?style=flat-square" alt="rekit"/></a>
  <!-- Velog 주소로 바꿔 주세요 -->
  <a href="https://velog.io/@VELOG_ID"><img src="https://img.shields.io/badge/Blog-Velog-20C997?style=flat-square&logo=velog&logoColor=white" alt="velog"/></a>
  <a href="mailto:wlsdmsrnfl@naver.com"><img src="https://img.shields.io/badge/Email-wlsdmsrnfl@naver.com-03C75A?style=flat-square&logo=naver&logoColor=white" alt="email"/></a>
</p>

---

### 👨‍💻 About

- **헬스케어 IT 기업 백엔드 엔지니어** (2024.06 ~ 2026.04, 1년 11개월)
  - 일 최대 3천만 건의 로그가 쌓이는 해외 대규모 레거시 시스템의 운영과 장애 대응
  - 헬스케어 서비스 백엔드와 외부 기관 표준 API 연동 (Spring Boot 3, Redis, NCP)
- **rekit 1인 개발** (2026.05 ~ 현재) · 🔗 **https://rekit.co.kr**
  - 업소용 중고 가전 거래 플랫폼. 기획부터 백엔드, 인프라, 배포, 모니터링까지 혼자 맡고 있습니다.

### 🏆 Key Achievements

| | 성과 | 어떻게 |
| :---: | --- | --- |
| **1시간** | 해외 서비스 전면 장애 복구 | 이슬람력 날짜(1449년)로 멈춘 WAS의 원인을 로그로 단계별 추적 |
| **3배+** | 로그 적재 처리 속도 개선 | 파일 중복 읽기 4회→1회, 재귀를 반복문으로 바꿔 서버 다운과 일일 수작업 제거 |
| **4개월** | 외부 API 지연에도 일정 준수 | 표준 스펙 기반 WireMock 서버로 먼저 개발해 연동 코드를 거의 그대로 재사용 |
| **1,440회/일** | 알림용 DB 폴링 조회 제거 | `@Scheduled` 폴링을 커밋 후 예약 + 비동기 발송 구조로 바꿔 실서비스에 반영 |

### 🚀 Featured Project

#### rekit · 업소용 중고 가전 거래 플랫폼

🔗 **서비스 주소: [https://rekit.co.kr](https://rekit.co.kr)**
<!-- 저장소가 공개라면 링크를 추가하세요: [GitHub](https://github.com/jineunpark/REPO) -->

폐업 매장에서 나온 업소용 가전을 상태 등급과 동작 보증 정보로 표준화해 거래하는 서비스입니다.
**API 약 100개 · 테스트 코드 560개+**

- **결제 정합성**: 토스페이먼츠 웹훅은 믿지 않고 조회 API로 재확인, `FOR UPDATE` 잠금 순서 통일로 이중 판매 경합 차단, Idempotency-Key, `SKIP LOCKED` 정리 작업
- **관측성**: Prometheus + Grafana로 p95·5xx 비율·결제 실패율까지 실시간 확인, 멀티 워커 환경의 지표 불일치 해결
- **배포**: git 태그로 Jenkins 빌드, 배포 후 자동 헬스체크, 이전 버전 재배포만으로 롤백
- **트러블슈팅**: 일부 사용자만 소셜 로그인에 실패하던 문제를 OAuth state와 DNS 설정에서 찾아 해결

<!-- 2단계(W3~W9) 완료 후 추가
#### [rekit-order](https://github.com/jineunpark/rekit-order) · 주문·결제 도메인 Spring Boot 재구현
Java 21 · Spring Boot 3 · JPA · AWS(EC2, RDS, SQS) · k6
- 주문 API p95 ○○ms → ○○ms
-->

### 🛠 Tech Stack

**Backend**<br/>
<img src="https://img.shields.io/badge/Java_21-007396?style=flat-square&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white"/>
<!-- W4 이후: <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square&logo=hibernate&logoColor=white"/> -->

**Data**<br/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
<img src="https://img.shields.io/badge/MS_SQL-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white"/>

**Infra & DevOps**<br/>
<img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
<img src="https://img.shields.io/badge/nginx-009639?style=flat-square&logo=nginx&logoColor=white"/>
<img src="https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white"/>
<img src="https://img.shields.io/badge/NCP-03C75A?style=flat-square&logo=naver&logoColor=white"/>
<!-- W6 이후: <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white"/> <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/> -->

**Monitoring & Test**<br/>
<img src="https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white"/>
<img src="https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white"/>
<img src="https://img.shields.io/badge/Sentry-362D59?style=flat-square&logo=sentry&logoColor=white"/>
<img src="https://img.shields.io/badge/WireMock-1E6BB8?style=flat-square"/>

### ✍️ Writing
<!-- 블로그 글을 발행할 때마다 위에서부터 추가하세요 -->
- 이슬람력 1449년이 WAS를 멈춘 이야기 *(작성 예정)*

### 🎓 Education · Awards · Certificate

- 상명대학교 컴퓨터과학과 졸업 (2024.08)
- 창업경진대회 대상 (2023.01)
- 데이터청년캠퍼스 최우수상 (2022.08)
- SQLD

<details>
<summary>이전 프로젝트</summary>

- [AI_WEBTOONER](https://github.com/new-Capstone/WEBTOONER_Backend) · 학부 캡스톤 백엔드

</details>
