## 권오철 (Gwon O Cheol)

근거를 확인하고 만들고, 배포한 뒤에도 사용자 반응을 보고 고쳐 나가는 **백엔드 개발자**입니다.

원광대학교 컴퓨터소프트웨어공학과에 재학 중이고, 기획한 서비스를 실제 학생들에게 공개해 운영하고 있습니다.

---

## 🛠 Tech Stack

**주력**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**사용 경험**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=claude&logoColor=white)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=for-the-badge&logo=railway&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Sentry](https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white)

---

## 🚀 Projects

### 🎓 [ONE Student](https://github.com/ONE-Student-WKU/web) — 원광대생의 졸업요건을 학칙 근거로 진단해 주는 서비스

`2026.07 ~ 운영 중` · 팀 3명 · 기획부터 개발·운영까지 대부분 담당 · [onestudent.io.kr](https://onestudent.io.kr)

들은 과목을 넣으면 졸업까지 무엇이 남았는지 계산하고, 학칙이 궁금하면 근거 조문을 인용해 답하는 챗봇을 제공합니다.

**구조에서 정한 것**

- **판정은 코드, 설명은 AI** — 졸업 학점과 요건 충족 여부는 규정 엔진이 계산하고, AI는 그 결과와 학칙 원문을 근거로 설명만 합니다. 숫자를 AI가 계산하지 않게 했습니다.
- **찾는 방법을 자료마다 나눔** — 학칙처럼 정해진 모양이 없는 문서는 RAG(임베딩 유사도 검색)로 찾고, 과목 목록처럼 하나도 빠지면 안 되는 자료는 SQL로 조회합니다.
- **규정 문서 반영 파이프라인** — 규정 문서를 고쳐 `main`에 반영하면 승인 뒤 자동으로 다시 임베딩됩니다. 임베딩을 모두 받은 뒤 트랜잭션으로 바꿔 넣어, 중간에 실패해도 옛 문서가 검색에 남습니다.

**개발하며 풀어 간 문제**

| 문제 | 해결 | 근거 |
|---|---|---|
| 성적표 PDF를 올렸는데 과목이 빠지거나 등록이 안 됨 `AI 결과 검증` | 과목 읽기는 AI에 맡기고, AI와 상관없이 문서에 적힌 학기별 합계로 검산 | [#57](https://github.com/ONE-Student-WKU/web/pull/57) · [#61](https://github.com/ONE-Student-WKU/web/pull/61) · [#123](https://github.com/ONE-Student-WKU/web/pull/123) |
| 인증 코드를 한꺼번에 보내면 5번 제한이 뚫림 `동시 요청` | "5번 미만일 때만 1 올리기"를 조건부 UPDATE 한 문장으로 처리 | [#347](https://github.com/ONE-Student-WKU/web/pull/347) |
| 학교 기준이 바뀌어 결과가 달라져도 학생이 모름 `변경 감지` | 진단 입력을 해시로 함께 저장해, 입력은 같은데 결과만 달라질 때만 알림 | [#481](https://github.com/ONE-Student-WKU/web/pull/481) |

### 🎁 [익산 스토어](https://github.com/adapterz/wku-iksan-store-BE) — 익산 지역 상권의 기프티콘 선물 쇼핑몰

`2026.06 ~ 11` · 부트캠프 팀 프로젝트(4명) · 백엔드 담당 · [iksan.store](https://iksan.store)

인증·공통 구조와 관리자 기능(상품 관리, 리뷰 신고, 회원 제재·이의제기, 운영 대시보드 API)을 맡았습니다.

| 문제 | 해결 | 근거 |
|---|---|---|
| 장바구니 결제가 담은 상품 수만큼 DB를 오감 `N+1` | 조회는 `IN` 한 번, 저장은 여러 행을 한 문장으로 넣어 쿼리 수를 고정 (30개 기준 75.7ms → 16.5ms) | [#133](https://github.com/adapterz/wku-iksan-store-BE/pull/133) |
| 보낸 사람이 탈퇴하면 받은 선물이 사라짐 `주문 시점 기록` | 주문할 때 닉네임을 함께 저장하고, 선물 조회는 회원 정보 대신 그 기록을 사용 | [#76](https://github.com/adapterz/wku-iksan-store-BE/pull/76) |

### 그 밖에

- [winforms-calendar](https://github.com/ChildrenAon/winforms-calendar) — 윈도우 프로그래밍 수업 팀 프로젝트 (C# WinForms 달력·일정 관리 앱)

---

## 📝 기록

- [TIL](https://github.com/ChildrenAon/TIL) — 개발하며 새로 알게 된 것을 날짜별로 기록합니다. 지금은 운영 중인 ONE Student 코드를 기능 하나씩 화면에서 DB까지 따라가며 다시 읽고 있습니다.
