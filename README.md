# 🧾 StockTrading-Web (주식 웹 트레이딩 플랫폼)

실시간 시세, 종목 검색, 트레이딩, 자산 관리, 정보 공유 기능을 제공하는 종합 주식 웹 트레이딩 서비스입니다.  
[🔗 배포 링크](https://your-deployment-url.com)

---

## 📆 프로젝트 개요

| 항목 | 내용 |
| ---- | ---- |
| 🧪 프로젝트명 | StockTrading-Web |
| ⏰ 개발 기간 | 2025.07.01 ~ (진행 중) |
| 👨‍💻 개발 인원 | 1명 (개인 프로젝트) |
| 🧩 담당 역할 | 전체 기획, 설계, 개발, 배포 |

---

## 🧰 기술 스택

### ✅ Backend
- Java 17, Spring Boot 3
- JPA (Hibernate), QueryDSL
- Spring Security + JWT
- Redis (캐싱, 세션)
- Kafka (이벤트 기반 주문 처리)
- MySQL
- Spring REST Docs (API 문서화)

### ✅ Frontend
- React.js (Vite + TypeScript)
- Tailwind CSS
- Chart.js / d3.js
- WebSocket

### ✅ DevOps
- Docker, Docker Compose
- Nginx
- GitHub Actions (CI/CD)
- AWS EC2, S3, Route53

---

## 🧩 시스템 아키텍처 (구상도)

![architecture](https://your-architecture-image-url.com)

- 모놀리식 → 점진적 마이크로서비스 구조
- 주문 시스템, 사용자 시스템, 종목 정보 시스템 분리 가능성 고려

---

## 🔑 주요 기능

### 📊 종목
- 종목 검색, 테마별 분류
- 종목별 뉴스, 재무제표 제공
- 최근 본 종목 목록 (삭제 가능)

### 💹 트레이딩
- 실시간 호가/차트
- 매수/매도/정정/취소 기능
- 체결/미체결 내역 확인 (WebSocket 실시간 처리)

### 💼 자산관리
- 계좌 개설
- 잔고 및 주문 내역 조회
- 관심 종목 관리
- 입출금 처리 (모의 기능)

### 🗣 정보 공유 게시판
- 글 등록/수정/삭제
- 댓글 기능

### 🧑‍💼 마이페이지
- 회원정보 수정
- 알림 설정
- 로그아웃

---

## 📈 홈 화면 구성

| 위치 | 내용 |
|------|------|
| 상단 | 네비바 + 드롭다운 (반응형) |
| 중단 | 코스피/코스닥/나스닥 지수, 상승/하락 TOP5 |
| 하단 | 거래량 상위 종목 리스트 |

---

## ⚙ 기술 설계 및 성능 최적화

| 분야 | 적용 내용 |
|------|-----------|
| 고성능 아키텍처 | CQRS, Kafka 기반 주문 분리, 비동기 이벤트 처리 |
| 데이터 최적화 | Redis 캐싱, ElasticSearch 종목 검색 |
| 인증/보안 | JWT + 리프레시 토큰 구조, OAuth2 로그인 |
| 배포 자동화 | Docker + GitHub Actions + Nginx 무중단 배포 |

---

## 🧪 API 명세서

Swagger 또는 Spring REST Docs를 통해 문서화  
👉 추후 링크 추가 예정

---

## 🧱 ERD

<details>
<summary>ERD 보기</summary>

![ERD](https://your-erd-image-url.com)

</details>

---

## 📝 문제 해결 사례

### ✅ 실시간 트레이딩 화면에서 동시성 문제

- **문제**: 동시에 여러 주문/체결/호가 데이터가 들어와 렌더링이 꼬임
- **해결**: WebSocket 메시지 큐 + 상태 기반 업데이트 처리
- **결과**: 실시간 트레이딩 화면 안정성 확보, flicker 현상 제거

---

## 🧠 회고 및 기록

- 프로젝트 전체 흐름, 기술 스택 선택 이유, 아키텍처 고민
- 구현 중 마주한 문제와 해결 과정을 정리한 노션 문서  
👉 [회고 링크 예정]

---

## 📦 기타 문서

- [기능 명세서](https://notion.so/your-function-doc)
- [기획서](https://notion.so/your-planning-doc)
- [기술 구조 설명](https://notion.so/your-structure-doc)

---

## 📌 참고 사이트

- [TradingView](https://www.tradingview.com/)
- [Robinhood](https://robinhood.com/)
- [Investing.com](https://www.investing.com/)

---

> 이 프로젝트는 포트폴리오 목적으로 개인이 설계·구현한 종합 주식 트레이딩 웹 애플리케이션입니다.
