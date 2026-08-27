<img width="100%" src="./assets/header.svg" alt="ByungHak Kim — Backend &amp; Cloud Engineer · Go · Python · AWS" />

<div align="center">

### 프로덕션 백엔드와 클라우드 인프라를 설계하고 운영합니다

**커머스는 제가 깊이 이해하는 도메인이지, 제가 만들 수 있는 시스템의 경계가 아닙니다.**

Go·Python 서비스의 설계부터 AWS 배포, 운영 안정화, 인계까지 맡아 왔습니다.

<br/>

<img src="https://img.shields.io/badge/Backend-Go_·_Python_·_TypeScript-0D1117?style=flat-square" />
<img src="https://img.shields.io/badge/AWS-EKS_·_Lambda_·_Aurora_·_S3-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" />
<img src="https://img.shields.io/badge/Focus-Reliability_·_Integration_·_Operations-1F6FEB?style=flat-square" />
<img src="https://img.shields.io/badge/Open_to-Backend_·_Platform_·_Cloud_roles-238636?style=flat-square" />

</div>

## What I build

- **Reliable backends** — integer ledgers, idempotent webhooks, transactional outbox, job queues, and APIs that can explain their state
- **AWS production systems** — EKS, Lambda, ECR, ALB, Aurora/RDS, S3, SQS, IAM, CloudWatch, Kubernetes, and CI/CD
- **Integration-heavy products** — ERP identity and inventory, carrier APIs, payment and payout flows, camera hardware, and AI generation providers
- **Operable software** — load-test follow-up, rollback paths, log retention, secrets boundaries, deployment contracts, and handover packages

## Featured engineering work

### [AWS Production Operations](https://github.com/hak2881/aws-production-operations)

EKS 서비스 운영, Lambda/EKS 런타임 경계, ECR·ALB·IAM·SQS 배선, CloudWatch 로그와 부하 대응을 정리했습니다. 잘못된 AWS identity나 Kubernetes context로도 명령은 성공할 수 있다는 문제에서 출발해, 배포 대상을 코드 리뷰와 실행 시점에 드러내는 방식을 사용했습니다.

`EKS` · `Lambda` · `Aurora/RDS` · `S3` · `SQS` · `IAM` · `CloudWatch`

### [Reliable Backend Patterns](https://github.com/hak2881/reliable-backend-patterns)

고객사 코드가 아닌 **실행 가능한 Go 샘플**입니다. 정수 금액, unique 멱등 키, append-only 원장, transactional outbox를 작은 인터페이스와 PostgreSQL 스키마로 보여줍니다. race test와 vet를 GitHub Actions에서 실행합니다.

`Go` · `PostgreSQL` · `TDD` · `GitHub Actions`

### [AI Experience Platform](https://github.com/hak2881/ai-experience-platform)

무인 키오스크 촬영부터 유료 AI 생성, S3 정규화, QR 결과 페이지까지 이어지는 시스템입니다. 공개 웹 계층에는 스토리지 자격증명을 두지 않았고, 재시도마다 비용이 발생하는 비멱등 작업은 Postgres 잡 큐와 운영자 승인 경계로 다뤘습니다.

`FastAPI` · `PostgreSQL` · `S3` · `Next.js` · `C# / WPF` · `C++ camera SDK`

### [Commerce Backend Microservices](https://github.com/hak2881/commerce-backend-msa)

호스팅형 플랫폼 뒤에서 직접 운영한 회원·리워드·주문·ERP·배송 백엔드의 사례입니다. 서비스 경계와 배포 경계를 분리하고, 웹훅 멱등성·outbox·자체 인증·인계 가능한 설정을 중심으로 기록했습니다.

`Go` · `Python` · `PostgreSQL` · `Kubernetes` · `AWS Lambda`

## Selected production work

> 대부분 NDA 프로젝트이므로 고객 상표와 인프라 식별자는 표기하지 않습니다. 아래 수치는 익명화된 시스템 규모와 결과입니다.

| 시스템 | 담당한 문제 | 결과 |
|---|---|---|
| 멀티브랜드 패션 마켓플레이스 | 대규모 커스텀 스토어프론트와 백엔드 10종, 검색·필터·회원 상태 | 브랜드 1,067개, 상품 메타필드 235,848건 백필, 실패율 0.04% |
| 미국 B2B+B2C 리워드 플랫폼 | 다단계 추천 보상, 현금 인출 원장, 임베드 관리자 앱 | Go 서비스 경계 유지 후 단일 배포, 원장 통합, 적립 3중 멱등성 |
| 글로벌 제조사 D2C | 백엔드 3종, 국제 배송 견적, 레거시 이관과 인계 | Lambda+EKS 혼합 런타임, Aurora Serverless, 체크섬 포함 인계 |
| 스포츠 브랜드 멤버십 | 등급·등급별 가격, 구매 게이트, 체크아웃 포인트 | Shopify Functions 3종, UI Extension 4종, 실데이터 시뮬레이션 후 배포 |
| B2B 원료 공급 | ERP 주문·재고·운임·샘플 제한 | 트리거별 FastAPI 4서비스, 택배·항공·해상 운임, 멱등 재고 대사 |
| AI 포토 키오스크 | 카메라 제어, 유료 생성 잡, 모바일 결과 전달 | FastAPI+Postgres 큐, scoped presigned URL, Windows/C++ 촬영 클라이언트 |

## More case studies

- [Loyalty and Ledger Systems](https://github.com/hak2881/loyalty-ledger-systems) — 현금성 리워드 원장, 등급 개편 시뮬레이션, 체크아웃 예약·확정 차감
- [ERP Integration Patterns](https://github.com/hak2881/erp-integration-patterns) — 주문 동기화, 중량별 운임, 샘플 제한, 스케줄 재고 대사
- [Storefront Engineering at Scale](https://github.com/hak2881/storefront-engineering) — 대형 테마 분해, AJAX 상태, 플랫폼 네이티브 전환 실패 기록
- [Platform Tooling](https://github.com/hak2881/platform-tooling) — 문서 디자인 시스템, 승인 게이트 에이전트 파이프라인, 소규모 서비스 표준

## How I work

**문제의 맥락부터 이해합니다.** 요구사항만 구현하지 않고 사용자 흐름, 데이터, 운영 제약을 함께 살펴 실제로 해결해야 할 문제를 정의합니다.

**복잡도에는 근거가 있어야 합니다.** 책임은 명확히 분리하되, 서비스와 인프라는 트래픽·장애 격리·운영 비용을 기준으로 설계합니다.

**배포 이후까지 책임집니다.** 로그와 지표, 실패 복구와 롤백 경로를 준비하고 운영에서 발견한 문제를 다음 개선으로 연결합니다.

**결정이 이어지게 만듭니다.** 기술적 선택과 트레이드오프, 환경 계약과 운영 절차를 기록해 다른 개발자가 안전하게 이어갈 수 있게 합니다.

## Stack

`Go` · `Python` · `TypeScript` · `C#` · `FastAPI` · `Django` · `PostgreSQL` · `Redis` · `EKS` · `Lambda` · `Aurora/RDS` · `S3` · `SQS` · `IAM` · `CloudWatch` · `Kubernetes` · `Docker` · `GitHub Actions`

---

## In English

Backend and cloud engineer building production services in Go and Python and operating them on AWS. I work across service design, data integrity, external integrations, deployment, incident follow-up, and handover.

Commerce is the domain in which I have the deepest production experience, not the limit of the systems I build. Recent work also includes an AI photo kiosk spanning camera control, paid generation jobs, S3 delivery, and a public mobile result experience.

The client systems are private, so the repositories above are sanitized case studies and independently written executable examples. They contain no client source, credentials, account IDs, or infrastructure identifiers.

<img width="100%" src="./assets/footer.svg" alt="" />
