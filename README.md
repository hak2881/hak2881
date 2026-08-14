# hak2881

Backend engineer. I build the systems that sit behind hosted commerce platforms — the part that handles money, identity, and integration with whatever the business already runs on.

Most of my work is under NDA, so what is here is **written up rather than published**: architecture, the problems that actually cost time, the decisions and their tradeoffs. No client code, no credentials, no infrastructure identifiers.

## Case studies

| Repository | What it covers |
|---|---|
| **[commerce-backend-msa](https://github.com/hak2881/commerce-backend-msa)** | Backend microservices behind Shopify Plus storefronts — Go and Python, service boundaries, webhook idempotency, when to consolidate six services into one deployable |
| **[loyalty-ledger-systems](https://github.com/hak2881/loyalty-ledger-systems)** | Points, tiers, and rewards — append-only ledgers, integer money, reserve-and-confirm redemption, simulating a tier change before it ships |
| **[erp-integration-patterns](https://github.com/hak2881/erp-integration-patterns)** | Putting a B2B storefront in front of an ERP — order sync, ocean freight quoting, scheduled inventory reconciliation |
| **[storefront-engineering](https://github.com/hak2881/storefront-engineering)** | A 1,067-brand marketplace theme — breaking up shared files, AJAX filter state, and three documented failures at platform-native offloading |
| **[ai-experience-platform](https://github.com/hak2881/ai-experience-platform)** | An AI photo kiosk — a job queue for paid non-idempotent work, serving media without storage credentials, camera control from a desktop app |
| **[platform-tooling](https://github.com/hak2881/platform-tooling)** | Internal infrastructure — a document design system, an agent pipeline with an approval gate, a repeatable shape for small services |

## What I work with

**Languages** — Go, Python, TypeScript, C#
**Backend** — chi · pgx · sqlc · goose · FastAPI · Django REST · Remix
**Data** — PostgreSQL, Aurora Serverless, Redis, S3
**Infra** — Kubernetes (EKS), Docker, AWS Lambda, GitHub Actions
**Commerce** — Shopify Plus: Admin & Storefront APIs, webhooks, app proxy, checkout extensions, edge functions, themes

## How I think about this work

**Money is stored as integers.** Every value system here uses an append-only ledger with amounts in the smallest unit. Balance is derived, never a column.

**Idempotency belongs in the database.** A unique constraint on an idempotency key is correct under concurrency. An application-level "have we seen this?" check is correct until two webhook deliveries race — which is exactly what happens during a retry storm.

**Boundaries and deployments are separate decisions.** One system here keeps six service boundaries in a single binary. Another deliberately refuses to split at all. Both were right for their traffic.

**Negative results are deliverables.** Three documented failed attempts at moving load onto a platform were worth more to the client than a fourth attempt would have been.

**Handover is part of the work.** Documentation with account IDs baked into it is documentation you can't hand to anyone.

---

## 한국어

커머스 플랫폼 뒤에 서는 백엔드를 만듭니다 — **돈, 신원, 그리고 이미 회사가 돌리고 있는 시스템과의 연동**을 다루는 부분입니다.

대부분의 작업이 NDA 하에 있어서, 여기 있는 것은 공개가 아니라 **기록**입니다 — 아키텍처, 실제로 시간을 잡아먹은 문제, 내린 결정과 그 트레이드오프. 클라이언트 코드·인증정보·인프라 식별자는 없습니다.

| 레포 | 내용 |
|---|---|
| **[commerce-backend-msa](https://github.com/hak2881/commerce-backend-msa)** | 커머스 플랫폼 뒤의 백엔드 마이크로서비스 — Go·Python, 서비스 경계, 웹훅 멱등성, 서비스 6개를 배포 1개로 합치는 판단 |
| **[loyalty-ledger-systems](https://github.com/hak2881/loyalty-ledger-systems)** | 포인트·등급·리워드 — append-only 원장, 정수 금액, 예약-확정 차감, 등급 개편 사전 시뮬레이션 |
| **[erp-integration-patterns](https://github.com/hak2881/erp-integration-patterns)** | ERP 앞에 B2B 스토어프론트 붙이기 — 주문 동기화, 해상 운임 견적, 스케줄 재고 대사 |
| **[storefront-engineering](https://github.com/hak2881/storefront-engineering)** | 브랜드 1,067개 마켓플레이스 테마 — 공유 파일 분해, AJAX 필터 상태, 네이티브 전환 3회 실패 기록 |
| **[ai-experience-platform](https://github.com/hak2881/ai-experience-platform)** | AI 포토 키오스크 — 유료·비멱등 작업용 잡 큐, 자격증명 없이 미디어 서빙, 데스크톱 앱의 카메라 제어 |
| **[platform-tooling](https://github.com/hak2881/platform-tooling)** | 내부 인프라 — 문서 디자인 시스템, 승인 게이트가 있는 에이전트 파이프라인, 소규모 서비스 표준 형태 |

**작업 원칙**

- **돈은 정수로 저장합니다.** 모든 값 시스템이 최소 단위 정수 금액의 append-only 원장을 씁니다. 잔액은 파생되지, 컬럼이 아닙니다.
- **멱등성은 DB에 있어야 합니다.** 멱등 키의 unique 제약은 동시성 하에서 옳습니다. 애플리케이션 레벨 "이거 본 적 있나?" 체크는 웹훅 두 건이 경합하기 전까지만 옳고, 그 경합은 정확히 재시도 폭주 때 일어납니다.
- **경계와 배포는 별개의 결정입니다.** 여기 한 시스템은 서비스 경계 6개를 단일 바이너리에 유지합니다. 다른 하나는 의도적으로 쪼개기를 거부합니다. 각자의 트래픽에서 둘 다 맞았습니다.
- **부정적 결과도 결과물입니다.** 플랫폼으로 부하를 옮기려다 실패한 3번의 기록이, 4번째 시도보다 고객사에 더 값어치 있었습니다.
- **인계도 일의 일부입니다.** 계정 ID가 박힌 문서는 누구에게도 건넬 수 없는 문서입니다.
