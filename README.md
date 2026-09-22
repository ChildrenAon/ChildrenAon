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
![Claude API](https://img.shields.io/badge/Claude_API-D97757?style=for-the-badge)

---

## 🚀 Projects

### **[wku-iksan-store-BE](https://github.com/adapterz/wku-iksan-store-BE)** — 익산 상권 기프티콘 서비스 (팀 프로젝트, **BE 담당 + 리뷰 담당**)
- API 명세서·ERD 설계부터 인증/세션, 주문, 선물함·바코드 사용까지 핵심 플로우 전 구간 구현
- 카테고리·상품 검색 API 설계 및 구현 (마이그레이션 스크립트 작성 포함)
- 관리자 인증/권한, 상품·카테고리 관리, 대시보드, 리뷰 신고·문의·회원 제재까지 관리자 페이지 API 전 구간 구현
- PR 리뷰 시 `git diff` 기반으로 설명과 실제 변경 파일을 대조하는 리뷰 방법론을 직접 정립해 팀에 적용
- 운영 배포 중 발생한 상품 이미지 404 장애를 BE/FE/인프라에 걸쳐 원인 진단하고 크로스팀 대응 주도

### **[ONE Student](https://github.com/ONE-Student-WKU/web)** — 원광대생 대학생활 통합 플랫폼 (학사관리·진로탐색·커뮤니티·AI 챗봇, 팀 프로젝트, **리더**)
- React(Vite) + Node.js/Express + MySQL 모노레포 구조
- 학사 관리(수강·성적 입력, 성적표 PDF 자동 인식·입력, 졸업요건 진단, 재수강 안내), 학칙 기반 AI 챗봇(RAG), 진로 탐색, 커뮤니티 모집 게시판(신청·승인·신고)까지 네 기능을 하나의 서비스로 통합 설계·구현
- 관리자 승인 검수 플로우, 관리자 대시보드까지 구현 완료
- 테스트 인프라(Vitest, node:test) 도입, Sentry 에러 추적 연동 등 백엔드 안정성·관측성 개선 주도
