<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:8B0000,50:B22222,100:1a1a2e&height=230&section=header&text=Tushar%20Mishra&fontSize=58&fontColor=ffffff&fontAlignY=38&desc=Your%20Friendly%20Neighborhood%20Engineer&descAlignY=60&descSize=18&animation=fadeIn" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&pause=1000&color=E23636&center=true&vCenter=true&width=800&lines=With+great+scale+comes+great+responsibility.;Kubernetes%2C+Kafka%2C+GCP%2C+Observability.;Distributed+systems+%2B+applied+AI+agents.;Swinging+between+backend+and+platform+engineering.)](https://git.io/typing-svg)

<a href="https://www.linkedin.com/in/tushar-mishra-7960b722b"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
<a href="https://www.tushar25.com"><img src="https://img.shields.io/badge/Portfolio-8B0000?style=for-the-badge&logo=firefox&logoColor=white" /></a>
<a href="https://discord.com/users/Menace25"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" /></a>

<br/>

![Location](https://img.shields.io/badge/Georgia%2C%20USA-1a1a2e?style=flat-square&logo=googlemaps&logoColor=E23636)
![Focus](https://img.shields.io/badge/Focus-Backend%20%7C%20Platform%20%7C%20Applied%20AI-8B0000?style=flat-square)
![Degree](https://img.shields.io/badge/B.S.%20CS%20(AI)-University%20of%20Georgia-B22222?style=flat-square)

</div>

---

### 🕷️ Radioactive Origin

I was bitten by backend engineering somewhere around a computer science degree (AI emphasis) at the University of Georgia, and I never quite recovered. Most of my work lives where fast, reliable systems meet an ML-aware layer swinging on top.

The unglamorous parts are half the appeal: chasing a flaky service through a stack trace at midnight, writing a Terraform module boring enough that nobody has to think about it again, catching a timezone bug before it catches me. If a system is observable, reproducible, and operable by someone who is not me, that is the kind of web I want to build.

---

### 🦸 Currently Swinging

| | |
|---|---|
| 🎓 **IT Professional Assistant** @ UGA Franklin College OIT | Keeping a university's worth of systems running |
| 🔬 **Building** | **RaftKV**, a Raft-based distributed key-value store, from scratch in Go |
| 📜 **Studying** | AWS Solutions Architect Professional |

---

### 🧪 The Serum: InferGrid

Every hero has an origin experiment. Mine is **InferGrid**, a production-grade distributed ML inference platform on GCP, and the project where backend engineering and applied AI fuse into one working system.

```mermaid
flowchart LR
    C([Client]) --> R{A/B Router<br/>hash-based}
    R -->|variant A| D[DistilBERT<br/>ONNX Runtime]
    R -->|variant B| S[scikit-learn<br/>baseline]
    C -.async.-> K[(Kafka Queue)]
    K --> D
    D --> W[WebSocket<br/>delivery]
    R --> P[(PostgreSQL<br/>experiment tracker)]
    D --> M[Prometheus + Grafana]
    D --> X[KS-test<br/>drift detector]
```

- ⚡ Sub-100ms p95 latency at 500+ requests per minute
- ☸️ Kubernetes autoscaling for inference workloads
- 🔀 Deterministic A/B model routing between DistilBERT and a scikit-learn baseline
- 📨 Kafka-backed async inference queue with WebSocket result delivery
- 📉 Drift detection on live traffic (KS-test) and Prometheus/Grafana observability
- 🖥️ React dashboard on Vercel for watching routing, latency, and drift

---

### 🌃 Patrols Across the City

<table>
<tr>
<td width="50%" valign="top">

#### 🚨 Sentra
**AI incident-triage copilot.** A tool-calling LLM agent investigates simulated production incidents using read-only diagnostics (logs, metrics, deploys, runbooks) and returns root-cause hypotheses with cited evidence, streamed to a Next.js evidence viewer.

- Human approval for restarts/rollbacks enforced in **orchestration code, not the prompt**, with an append-only audit trail
- **100% root-cause accuracy and valid citations** across 12 live-LLM runs on 6 seeded failure scenarios; 0 approval-gate bypasses
- 135 automated tests, CI across three services

`Next.js` `FastAPI` `pgvector` `Gemini` `Docker`

</td>
<td width="50%" valign="top">

#### 🧩 RaftKV *(in progress)*
**Distributed key-value store implementing Raft from scratch** in Go/gRPC: leader election, log replication, snapshotting, and a write-ahead log with torn-tail repair.

- Fault-injecting filesystem and crash-recovery tests
- Next up: a chaos-testing harness with a **linearizability verifier**
- Suite green and clean under Go's `-race` detector

`Go` `gRPC` `Raft` `WAL`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🤖 Job Agent *(in design)*
**Local-first, CLI-driven multi-agent assistant** that detects job postings, researches sponsorship evidence, and tailors resumes truthfully. Human stays in the loop: no auto-submit, no pay-per-token APIs.

`Multi-agent` `CLI` `Codex` `Claude Code`

</td>
<td width="50%" valign="top">

#### 🌊 Clickstream Lake *(in progress)*
**Serverless AWS data lake** for simulated e-commerce events: S3 tiered storage, Glue ETL to partitioned Parquet, Athena analytics, QuickSight dashboards, with cost guardrails and IaC via CDK.

`S3` `Glue` `Athena` `QuickSight` `CDK`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🔭 Nexus & VectorForge
**Distributed observability.** Nexus traces requests and monitors service health across a cluster, the kind of tool you build so the next 2am page is shorter. VectorForge extends the observability thread.

`Tracing` `Metrics` `Distributed Systems`

</td>
<td width="50%" valign="top">

#### 🏆 Procuroid
**Multi-agent procurement system.** Honorable Mention at **AI ATL 2025**, Google Cloud track.

`Multi-agent` `Google Cloud`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 📬 AtlasFlow
**Event-driven backend** on DynamoDB and SQS, built for decoupled, asynchronous processing instead of one long synchronous chain.

`DynamoDB` `SQS` `AWS`

</td>
<td width="50%" valign="top">

#### 📸 PixelVault
**Zero-cost photo archival pipeline.** iPhone photos route through a Vercel relay to an old Pixel XL for free, unlimited Google Photos backup. A fun systems-automation heist.

`Next.js` `Kotlin` `iOS Shortcuts`

</td>
</tr>
<tr>
<td width="50%" valign="top">

#### 🕸️ FraudSense
**Fraud detection with graph-structured models**, built to catch the patterns flat tabular data quietly misses.

`Graph ML` `Python`

</td>
<td width="50%" valign="top">

#### 🧪 Mini ML Platform
A smaller-scale run at the ideas behind InferGrid, the proving ground before the real thing got built.

`MLOps` `Python`

</td>
</tr>
</table>

---

### 🧰 Utility Belt

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=java,py,ts,js,go,kotlin,swift,cpp,bash&perline=9" />

**Backend, Cloud & Infra**

<img src="https://skillicons.dev/icons?i=spring,nodejs,fastapi,react,nextjs,graphql,docker,kubernetes,terraform,gcp,aws,azure&perline=12" />

**Data, Messaging & Observability**

<img src="https://skillicons.dev/icons?i=postgres,mongodb,cassandra,mysql,redis,kafka,rabbitmq,prometheus,grafana&perline=9" />

</div>

---

### 🎖️ Certifications

![AWS SAA](https://img.shields.io/badge/AWS-Solutions%20Architect%20Associate-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![AWS CCP](https://img.shields.io/badge/AWS-Cloud%20Practitioner-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-AZ--900-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AWS SAP](https://img.shields.io/badge/AWS%20SAP-In%20Progress-8B0000?style=for-the-badge&logo=amazonaws&logoColor=white)

---

### 🕸️ Spider Sense (Live Activity)

<p align="center">
  <img width="49%" src="https://github-readme-stats-eight-wheat-41.vercel.app/api?username=MenaceHecker&show_icons=true&theme=dracula&hide_border=true&count_private=true&include_all_commits=true" />
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=MenaceHecker&theme=dracula" />
</p>

---

### 📖 The Code I Swing By

> With great scale comes great responsibility, for uptime, for logs, and for whoever is on call when things break at 2am.
>
> Build systems that are observable.
>
> Build systems that fail gracefully instead of embarrassingly.
>
> Build systems someone else can swing through without needing a map.

---

<details>
<summary><b>🎭 Unmasked</b></summary>

<br>

- I have strong opinions about logging and monitoring, and I will share them whether you ask or not.
- Most of my side projects start small and quietly turn into full infrastructure projects.
- Debugging almost always starts in the code and ends in the logs.
- I once spent an embarrassing number of hours tracking down a single timezone bug.
- The Kafka cluster is probably fine.

</details>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:B22222,100:8B0000&height=120&section=footer" />

</div>
