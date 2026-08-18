<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:1F6FEB,100:58A6FF&height=200&section=header&text=ByungHak%20Kim&fontSize=54&fontColor=FFFFFF&fontAlignY=36&desc=Backend%20Engineer%20·%20Commerce%20Platforms&descAlignY=58&descSize=18" />

<div align="center">

### 커머스 플랫폼 뒤에 서는 백엔드를 만듭니다

**돈** · **신원** · **회사가 이미 돌리고 있는 시스템과의 연동**

<br/>

<img src="https://img.shields.io/badge/Shopify_Plus-7AB55C?style=flat-square&logo=shopify&logoColor=white" />
<img src="https://img.shields.io/badge/9_production_systems-1F6FEB?style=flat-square" />
<img src="https://img.shields.io/badge/Go_·_Python_·_TypeScript-0D1117?style=flat-square" />
<img src="https://img.shields.io/badge/EKS_·_Lambda_·_Aurora-FF9900?style=flat-square" />

</div>

<br/>

## 이런 걸 만듭니다

- **결제·정산이 걸린 백엔드** — 현금으로 인출되는 리워드 원장, 체크아웃 포인트 차감, ERP로 들어가는 매출 기록. 틀리면 회계 차액이 되는 코드
- **플랫폼이 못 하는 것** — 호스팅형 커머스에 등급별 가격, 다단계 추천 트리, 구매자별 상한처럼 **플랫폼에 개념 자체가 없는 규칙**을 얹는 일
- **레거시와의 연결** — 스토어프론트보다 오래됐고 앞으로도 더 오래 갈 ERP를 신원·재고의 원본으로 두고 그 앞에 커머스를 세우는 일
- **인수받고, 넘겨주는 일** — 중간에 받아서 확장하고, 계정 식별자까지 전부 파라미터화한 인계 패키지로 고객사 팀에 넘기는 것까지

<br/>

## Selected Work

> 클라이언트 상표는 표기하지 않습니다. 도메인·규모로만 기술합니다.

<table>
<tr><th align="left">도메인</th><th align="left">작업</th><th align="left">규모 · 결과</th></tr>

<tr><td>

**멀티브랜드 럭셔리 패션 마켓플레이스**
<sub>국내 · 대규모 카탈로그</sub>

</td><td>

대규모 커스텀 스토어프론트 + 백엔드 10종 앞단.
필터·검색·큐레이션·위시리스트·쿠폰

</td><td>

브랜드 **1,067개** · 상위 브랜드 상품 5,000+개<br/>
상품 메타필드 **235,848건 백필** (실패율 0.04%)<br/>
섹션 147 · 스니펫 121 · 템플릿 48 · CSS 172 · JS 74<br/>
플랫폼 네이티브 전환 3회 시도 → **실패 원인 문서화**

</td></tr>

<tr><td>

**글로벌 대시캠 제조사**
<sub>국내 제조 · 딜러 + 소비자 이중 채널</sub>

</td><td>

백엔드 3종, 레거시 CMS 무중단 이관,
국제 배송비 실시간 견적, 인계

</td><td>

스토어프론트 2개 · **Lambda + EKS 하이브리드** 런타임<br/>
Aurora Serverless v2 · 읽기/쓰기 분리<br/>
인프라 문서 · DB 스키마 · 체크섬 번들 **인계 완료**

</td></tr>

<tr><td>

**미국 뷰티 디바이스 브랜드**
<sub>B2B + B2C 단일 Plus 스토어</sub>

</td><td>

다단계 추천 보상 원장,
파트너 현금 인출, 임베드 관리자 앱

</td><td>

Go 서비스 **6개 → 단일 바이너리** (경계 유지)<br/>
원장 **2개 → 1개 통합**, 과거 잔액 이관<br/>
적립 **3중 멱등성** · 부동소수 연산 0

</td></tr>

<tr><td>

**라켓스포츠 · 알파인 아웃도어 브랜드**
<sub>국내 D2C · 2개 브랜드 병행</sub>

</td><td>

멤버십 등급·등급별 가격,
런칭/래플 구매 게이트, 알림

</td><td>

**Shopify Functions 3종** · UI Extension 4종<br/>
네트워크 없는 체크아웃 샌드박스에서 등급가 적용<br/>
등급 개편 **실데이터 시뮬레이션 수십 회 후** 배포

</td></tr>

<tr><td>

**B2B 화장품 원료 공급사**
<sub>제조사 대상 · 드럼 단위 거래</sub>

</td><td>

ERP 연동 4서비스.
주문·운임·샘플 제한·재고

</td><td>

**트리거별로 분리한 4서비스** (웹훅/요청/스케줄)<br/>
중량 구간별 **택배 · 항공 · 해상** 운임 견적<br/>
ERP→스토어 재고 대사 1일 2회, 멱등 설계

</td></tr>

<tr><td>

**아웃도어 기어 리테일러**
<sub>국내 · 오프라인 멤버십 선행</sub>

</td><td>

레거시 ERP 기반 통합회원,
마이페이지, 체크아웃 포인트

</td><td>

문자인증 → ERP 매칭 → **메타필드 투영**<br/>
스토어프론트 핫패스에 ERP 호출 0<br/>
Go 단일 서비스, 기능은 패키지로 추가

</td></tr>

<tr><td>

**AI 포토 키오스크 플랫폼**
<sub>무인 현장 설치 · 유료 AI 생성</sub>

</td><td>

촬영 → 생성 → QR 결과 전 구간.
백엔드 · 웹 · 데스크톱 앱

</td><td>

FastAPI + **Postgres 잡 큐** · 벤더 중립 어댑터<br/>
웹 계층 **스토리지 자격증명 0** · 세션별 presigned<br/>
Windows 키오스크 앱 + **C++ 카메라 SDK 사이드카**

</td></tr>
</table>

<br/>

## Stack

<p>
<img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/C%23-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
</p>

<p>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
<img src="https://img.shields.io/badge/Remix-000000?style=for-the-badge&logo=remix&logoColor=white" />
<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
<img src="https://img.shields.io/badge/chi_·_pgx_·_sqlc-00ADD8?style=for-the-badge" />
</p>

<p>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/Amazon%20S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" />
<img src="https://img.shields.io/badge/Aurora_Serverless-527FFF?style=for-the-badge&logo=amazonrds&logoColor=white" />
</p>

<p>
<img src="https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/AWS_Lambda-FF9900?style=for-the-badge&logo=awslambda&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" />
<img src="https://img.shields.io/badge/Shopify_Plus-7AB55C?style=for-the-badge&logo=shopify&logoColor=white" />
</p>

<br/>

## Case Studies

대부분의 작업이 NDA 하에 있어서, 여기 있는 것은 공개가 아니라 **기록**입니다 —
아키텍처, 실제로 시간을 잡아먹은 문제, 내린 결정과 그 트레이드오프.
클라이언트 코드·인증정보·인프라 식별자는 없습니다.

<table>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/commerce-backend-msa"><img src="https://img.shields.io/badge/commerce--backend--msa-0D1117?style=for-the-badge&logo=go&logoColor=00ADD8" /></a>

커머스 플랫폼 뒤의 **백엔드 마이크로서비스**.
서비스 경계, 웹훅 멱등성, 서비스 6개를 배포 1개로 합치는 판단.

<img src="https://img.shields.io/badge/-3_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-Go-00ADD8?style=flat-square" /> <img src="https://img.shields.io/badge/-FastAPI-009688?style=flat-square" /> <img src="https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square" />

</td>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/loyalty-ledger-systems"><img src="https://img.shields.io/badge/loyalty--ledger--systems-0D1117?style=for-the-badge&logo=databricks&logoColor=4493F8" /></a>

포인트·등급·리워드의 **원장 설계**.
정수 금액, 예약-확정 차감, 등급 개편 사전 시뮬레이션.

<img src="https://img.shields.io/badge/-4_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square" /> <img src="https://img.shields.io/badge/-Go-00ADD8?style=flat-square" /> <img src="https://img.shields.io/badge/-Idempotency-8957E5?style=flat-square" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/erp-integration-patterns"><img src="https://img.shields.io/badge/erp--integration--patterns-0D1117?style=for-the-badge&logo=databricks&logoColor=BF8700" /></a>

**ERP 앞에 B2B 스토어프론트** 붙이기.
주문 동기화, 해상 운임 견적, 스케줄 재고 대사.

<img src="https://img.shields.io/badge/-4_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-FastAPI-009688?style=flat-square" /> <img src="https://img.shields.io/badge/-Webhooks-1F6FEB?style=flat-square" /> <img src="https://img.shields.io/badge/-B2B-BF8700?style=flat-square" />

</td>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/storefront-engineering"><img src="https://img.shields.io/badge/storefront--engineering-0D1117?style=for-the-badge&logo=shopify&logoColor=7AB55C" /></a>

**브랜드 1,067개** 마켓플레이스 테마.
공유 파일 분해, AJAX 필터 상태, 네이티브 전환 3회 실패 기록.

<img src="https://img.shields.io/badge/-4_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-Liquid-7AB55C?style=flat-square" /> <img src="https://img.shields.io/badge/-Vanilla_JS-F7DF1E?style=flat-square" /> <img src="https://img.shields.io/badge/-Performance-DA3633?style=flat-square" />

</td>
</tr>
<tr>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/ai-experience-platform"><img src="https://img.shields.io/badge/ai--experience--platform-0D1117?style=for-the-badge&logo=openaigym&logoColor=58A6FF" /></a>

**AI 포토 키오스크** 전 구간.
유료·비멱등 작업용 잡 큐, 자격증명 없는 미디어 서빙, 카메라 제어.

<img src="https://img.shields.io/badge/-3_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-FastAPI-009688?style=flat-square" /> <img src="https://img.shields.io/badge/-Amazon_S3-569A31?style=flat-square" /> <img src="https://img.shields.io/badge/-C%23-512BD4?style=flat-square" />

</td>
<td width="50%" valign="top">

<a href="https://github.com/hak2881/platform-tooling"><img src="https://img.shields.io/badge/platform--tooling-0D1117?style=for-the-badge&logo=gnometerminal&logoColor=768390" /></a>

**내부 인프라**.
문서 디자인 시스템, 승인 게이트 에이전트 파이프라인, 소규모 서비스 표준 형태.

<img src="https://img.shields.io/badge/-3_cases-30363D?style=flat-square" /> <img src="https://img.shields.io/badge/-Design_System-EC4899?style=flat-square" /> <img src="https://img.shields.io/badge/-AI_Agents-8957E5?style=flat-square" /> <img src="https://img.shields.io/badge/-Docker-2496ED?style=flat-square" />

</td>
</tr>
</table>

<br/>

## 일하는 방식

**돈은 정수로만 다룹니다.**
금액은 센트, 포인트는 100을 곱해서 정수로 저장합니다. 십진수로 바꾸는 건 화면에 뿌릴 때뿐입니다. 잔액도 컬럼에 들고 있지 않고 원장을 더해서 구합니다. 그래야 "이 잔액이 왜 이 숫자인가"를 항목 단위로 설명할 수 있고, 환불이 들어와도 이력을 지우지 않고 반대 부호 한 줄을 더하면 됩니다.

**중복은 DB가 막게 합니다.**
웹훅은 반드시 두 번 옵니다. 코드에서 "이미 처리했나?"를 조회해서 거르는 방식은 두 건이 동시에 들어오면 뚫리고, 그 동시 유입은 하필 재시도가 몰릴 때 일어납니다. 멱등 키에 unique 제약을 걸어두면 재전송이 그냥 거절된 insert가 됩니다.

**쪼갤지 말지는 트래픽이 정합니다.**
한 프로젝트는 서비스 경계 6개를 그대로 둔 채 배포만 하나로 합쳤고, 다른 프로젝트는 끝까지 쪼개지 않았습니다. 경계를 나누는 것과 따로 배포하는 것은 별개의 문제입니다. 파드 6개와 커넥션 풀 6벌이 필요 없는 트래픽에서 굳이 나눠 띄울 이유는 없습니다.

**남는 건 코드보다 기록입니다.**
플랫폼으로 부하를 되돌리려다 세 번 실패했습니다. 그 실패 원인을 정리한 문서가 네 번째 시도보다 고객사에 도움이 됐습니다. 같은 논의가 반년마다 다시 올라오는 걸 막아줬으니까요. 인계도 비슷합니다. 계정 ID가 박혀 있으면 애초에 넘길 수 없는 문서라, 식별자를 전부 분리해서 정리했습니다.

<br/>

---

## In English

Backend engineer working on the systems behind hosted commerce platforms — money, identity, and integration with whatever the business already runs on.

Recent work includes:

- a **1,067-brand fashion marketplace** storefront and the ten services behind it
- **dual-channel D2C** for a global dashcam manufacturer, serving dealers and consumers
- a **multi-level referral reward ledger** whose balance is withdrawable as cash
- **membership programs for two sports brands** on a platform with no native tier support
- **ERP integration** for a B2B ingredient supplier, from order sync to ocean freight quoting
- an **AI photo kiosk platform**, from camera control to the public result page

Most of it is under NDA, so these repositories are write-ups rather than published source: the architecture, the problems that actually cost time, and the reasoning behind each tradeoff. No client code, credentials, or infrastructure identifiers.

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:58A6FF,50:1F6FEB,100:0D1117&height=120&section=footer" />
