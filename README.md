### 👩‍💻 About me

**Cloud/Infra Engineer · SRE · Data Engineer · Platform Engineer**

제약 안에서 돌아가는 구조를 설계하고 운영하는 엔지니어입니다.<br>
AWS 인프라와 데이터 파이프라인을 설계하고, 모니터링과 알림을 붙여 실서비스로 운영해 왔습니다.<br>
만든 뒤에도 장애와 오탐의 원인을 운영 데이터로 다시 확인하고, 고친 방법을 코드와 문서로 남깁니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-seoyeon83.github.io-1F5FD1?style=flat-square&logo=githubpages&logoColor=white)](https://seoyeon83.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Seoyeon_Kim-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/seoyeon-kim-b7369a305/)
[![Email](https://img.shields.io/badge/Email-seannn283@gmail.com-24292F?style=flat-square&logo=gmail&logoColor=white)](mailto:seannn283@gmail.com)

---

### 📂 Projects

**[KG-RAG 기반 화장품 추천 시스템](https://seoyeon83.github.io/projects/kg-rag.html)** · `2026.01 – 2026.11` · BOAZ 25기 Team 4EVR0 (4인) · [GitHub](https://github.com/4EVR0)<br>
데이터 전처리 파이프라인, AWS 인프라, 통합 모니터링 담당
- Iceberg 메달리온 전처리 파이프라인과 Airflow DAG 설계, Aho-Corasick 성분 매칭으로 완전탐색 대비 약 200배, 매칭률 99%대
- 5개 이기종 환경의 메트릭과 로그를 Grafana로 통합하고 실측값 기반 알림 14종 설계
- 품질 경고 오탐의 원인을 4개 층위로 추적해 수정, 입력 품질 게이트 도입 (과거 재생 기준 데이터 나이 SLO 달성률 96.1%)
- 재실행 시 두 벌 쌓이던 적재를 멱등화하고 누락 배치 7개를 백필로 복구
- GitHub OIDC와 SSM으로 키 없는 배포를 저장소 4개에 통일, 배포 결과 회수와 재시작 승인 분리
- 저트래픽 베타 서비스에 알림 6종 설계, GPU 정지 3회 모두 3분 내 감지, 배포 오탐 0건

**[BOAZ 공식 웹사이트](https://seoyeon83.github.io/projects/boaz-web.html)** · `2026.02 – 현재` · 백엔드 팀장, 이후 백엔드 PM · [Service](https://www.bigdataboaz.com) · [Backend](https://github.com/BOAZ-website/backend)<br>
운영 중인 동아리 공식 웹 서비스, AWS 인프라 설계와 운영 담당
- k6 부하 테스트로 단일 서버가 충분함을 확인하고 3개 구성 중 CloudFront + 퍼블릭 EC2 선택 (월 예상 비용 $70대 → $40대)
- 모집 기간에만 이중화(ALB, EC2 2대, RDS Multi-AZ)하고 전환을 스크립트로 자동화, 상시 이중화 대비 연 40% 이상 절감
- 평가 기간 시간당 최대 9,208건의 API 요청을 서버 1대로 처리, CloudWatch 대시보드 2종과 알람 12종 구성
- 로그인 장애를 남은 지표로 재분석해 처음 세운 캐시 가설을 기각하고 WAF 요청 수 제한으로 원인 재정의
- 명세 저장소 backend-docs 구축(기능 명세 68개, TC 864개 이전), 운영 인프라 Terraform 마이그레이션 (네트워크 완료)

> 문제 정의와 설계 근거, 검증 결과는 [포트폴리오](https://seoyeon83.github.io)에 정리되어 있습니다.

### 🌱 Activities & Education

- **빅데이터 연합 동아리 BOAZ** 25기 데이터 엔지니어링 · `2025.07 – 2026.07`
- **4차 산업혁명 연합 동아리 TAVE** 14기 백엔드 · `2024.08 – 2025.01` — 후반기 프로젝트 최우수상
- **프로그래머스 데브코스** 데이터 엔지니어링 3기 · `2024.03 – 2024.08`
- **서울여자대학교** 데이터사이언스학과 · 소프트웨어융합학과 · `2021.03 – 2027.02 졸업 예정`

### 🏅 Certifications

<a href="https://www.credly.com/badges/eb1910e8-b429-4177-903e-74b7783c8b85/public_url"><img src="https://images.credly.com/size/340x340/images/0e284c3f-5164-4b21-8660-0d84737941bc/image.png" width="80" alt="AWS Certified Solutions Architect – Associate"></a>
<a href="https://www.credly.com/badges/17777786-a370-4989-9652-1994f24574a1/public_url"><img src="https://images.credly.com/size/340x340/images/00634f82-b07f-4bbd-a6bb-53de397fc3a6/image.png" width="80" alt="AWS Certified Cloud Practitioner"></a>

### 🧰 Tech Stack

<img src="assets/tech-stack.svg" height="48" alt="AWS, Terraform, Docker, GitHub Actions, Prometheus, Grafana, Grafana Loki, Python, Apache Airflow, Apache Iceberg, Java, Spring">
