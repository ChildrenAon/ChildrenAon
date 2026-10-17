## 권오철 (Gwon O Cheol)

원광대학교 컴퓨터소프트웨어공학과 재학 중 · **백엔드 개발** 실무형 프로젝트 경험을 쌓아가고 있습니다.

기능을 구현하는 데 그치지 않고, 문제가 발생했을 때 원인을 코드와 문서로 끝까지 추적해 근본 원인을 규명하는 것을 중요하게 생각합니다.

---

## 🛠 Tech Stack

**주력**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

**사용 경험**

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Jest](https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge&logo=claude&logoColor=white)

---

## 🚀 Projects

### **[ONE Student](https://github.com/ONE-Student-WKU/web)** — 원광대 학생 학사 정보 서비스 (팀 프로젝트, **리더**) · [onestudent.io.kr](https://onestudent.io.kr)

학생이 입력한 학사정보와 원광대 실제 학칙·교육과정을 근거로 **"졸업까지 무엇이 남았는지"** 알려주고, 학칙 질문에 근거를 들어 답하는 서비스입니다. 실제 운영 중입니다.

- **규정 판단 엔진** — 학칙·학칙시행규칙 원문과 교육과정 책자 10개년(2017~2026, 학번별 이수기준표)을 근거로, 학과(126개)·학번·입학 유형(일반·편입·전과)·다전공·교직·휴학에 맞는 졸업요건을 계산하고, 근거가 불확실하면 "추정"과 그 이유를 함께 표시
- **학칙 기반 AI 챗봇 (RAG)** — Voyage 임베딩 검색 + Claude. 규정 판단 결과와 학생의 이수 현황을 근거 우선순위대로 넘기고, 근거에 없는 내용은 단정하지 않도록 답변 가드를 적용
- **성적표 PDF 자동 입력** — 웹정보서비스 성적표 PDF를 AI로 읽어 과목·학점·성적을 한 번에 등록하고, 문서의 합계와 대조해 차이를 알림
- **학교와 직접 소통해 기준 확정** — 교육혁신과·학과에 문의·면담해 받은 답을 기록하고 데이터와 엔진에 반영. 학교의 자동 수집 불허 방침에 맞춰 사람이 검증하는 자료 갱신 절차를 설계
- **운영 인프라** — Vercel·Railway 배포, GitHub Actions CI(서버·클라이언트 자동 테스트 1,200여 개), 승인 게이트가 있는 DB 재시딩 워크플로, Sentry 에러 추적, 요청 제한·세션 보안
- 학사 관리·진로 탐색·커뮤니티(모집·신고·제재)·관리자 페이지·한국어/영어 화면까지 하나의 서비스로 통합 — React(Vite) + Node.js/Express + MySQL 모노레포
