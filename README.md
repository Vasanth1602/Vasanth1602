<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a5f,100:0ea5e9&height=200&section=header&text=Vasanth%20A&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=DevOps%20%7C%20Cloud%20Infrastructure%20%7C%20MLOps&descSize=18&descAlignY=58&descColor=94d2ff&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=800&color=0EA5E9&center=true&vCenter=true&width=700&lines=Building+production-grade+cloud+infrastructure;Evolving+one+platform+through+real+DevOps+phases;Terraform+%7C+Docker+%7C+AWS+%7C+CI%2FCD;Documenting+real+incidents%2C+not+just+checkmarks)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-vasanth1602-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vasanth1602)
[![GitHub](https://img.shields.io/badge/GitHub-Vasanth1602-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vasanth1602)
[![Email](https://img.shields.io/badge/Email-kumarajith85666%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kumarajith85666@gmail.com)

</div>

---

## About Me

I'm an early-career DevOps/Cloud Engineer (M.Sc. Data Science, Periyar University) with hands-on AWS, Terraform, and CI/CD experience — validated through a 3-month cloud infrastructure internship at Codec Technologies and three self-built, production-style projects. I build platforms and pipelines that turn manual, error-prone deployment work into automated, observable systems.

My current focus is **VoteSecure** — a voting platform evolving phase by phase (containerization → reverse proxy → CI/CD → cloud deployment → monitoring → Kubernetes), with real incidents documented along the way instead of just green checkmarks. My work sits at the intersection of **infrastructure as code**, **CI/CD automation**, and **cloud-native architecture** — with a growing focus on **observability** and incident-driven learning.

```text
🏗️  Currently building     →  VoteSecure (Phase 3 complete → AWS deployment next)
☁️  Cloud focus             →  AWS (EC2, ECS Fargate, ALB, RDS, Secrets Manager, ECR)
🔧  Automation passion      →  Replacing manual workflows with repeatable, observable pipelines
🎓  Certified               →  CI/CD (IBM · Coursera)
📚  Learning next           →  Monitoring (Prometheus + Grafana), Kubernetes
📍  Based in                →  Tamil Nadu, India
```

---

## Tech Stack

<div align="center">

### Cloud & Infrastructure
[![AWS](https://img.shields.io/badge/AWS-EC2%20%7C%20ECS%20Fargate%20%7C%20ALB%20%7C%20RDS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://aws.amazon.com)
[![Terraform](https://img.shields.io/badge/Terraform-IaC-7B42BC?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io)
[![Docker](https://img.shields.io/badge/Docker-Containerisation-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)

### CI/CD & Automation
[![Jenkins](https://img.shields.io/badge/Jenkins-Pipelines-D24939?style=flat-square&logo=jenkins&logoColor=white)](https://www.jenkins.io)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-Workflows-2088FF?style=flat-square&logo=github-actions&logoColor=white)](https://github.com/features/actions)

### Backend & Databases
[![Python](https://img.shields.io/badge/Python-3.12-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Flask](https://img.shields.io/badge/Flask-3.0-000000?style=flat-square&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-336791?style=flat-square&logo=postgresql&logoColor=white)](https://www.postgresql.org)
[![Redis](https://img.shields.io/badge/Redis-7-DC382D?style=flat-square&logo=redis&logoColor=white)](https://redis.io)

### Frontend & Tools
[![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactjs.org)
[![NGINX](https://img.shields.io/badge/NGINX-Reverse%20Proxy-009639?style=flat-square&logo=nginx&logoColor=white)](https://nginx.org)
[![Linux](https://img.shields.io/badge/Linux-Ubuntu-FCC624?style=flat-square&logo=linux&logoColor=black)](https://ubuntu.com)

</div>

---

## Featured Projects

<table>
<tr>
<td width="100%" valign="top">

### 🚀 ML Deployment Platform
**One-click ML model deployment from GitHub URL to live AWS infrastructure**

A self-service MLOps platform that eliminates manual server configuration. Enter a GitHub repo URL — the platform provisions an EC2 instance, installs Docker, configures NGINX as a reverse proxy, builds the Docker image, and streams real-time deployment progress to a React dashboard via WebSocket.

**Platform Infrastructure (Terraform IaC — 10 modules):**
- **Networking** — Custom VPC · Multi-AZ public/private/DB subnets · NAT Gateway
- **Compute** — ECS Fargate (Flask backend, serverless) · ECR (private container registry) · EC2 (ML app deployment target)
- **Frontend** — React SPA on S3 + CloudFront (global CDN, free HTTPS)
- **Traffic** — ALB with path-based routing (/api/* and /socket.io/* → ECS backend) + session stickiness for WebSocket continuity
- **Data** — RDS PostgreSQL 16 in isolated DB subnets
- **Security** — Layered security groups · IAM least-privilege · CloudFront origin restriction on ALB · no static credentials anywhere
- **Secrets** — AWS Secrets Manager for DB credentials, JWT secrets, and SSH keys — injected at ECS runtime via task definition

**Application Pipeline (boto3 + Paramiko):**
- 13-step automated pipeline: EC2 provisioning → SSH → Docker install → git clone → image build → container run → NGINX config → health check
- Real-time WebSocket deployment logs streamed to React dashboard
- JWT-secured REST API · SQLAlchemy + Alembic migrations · automatic EC2 cleanup on pipeline failure

> ⚡ Reduces a 30-minute manual EC2 setup to under 5 minutes — fully automated end to end

[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=for-the-badge&logo=github)](https://github.com/Vasanth1602/ML-Deployment-Platform)
[![Python](https://img.shields.io/badge/Python-blue?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://aws.amazon.com)
[![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactjs.org)

</td>
</tr>
</table>

<table>
<tr>
<td width="100%" valign="top">

### ☁️ AWS DevOps Platform
**Production-grade Flask API on AWS — 100% Infrastructure as Code, from provisioning to observability**

An end-to-end cloud engineering build: a Flask API on EC2 with every AWS resource — VPC, security groups, IAM roles, S3, CloudWatch — provisioned entirely through Terraform. Every push to `main` triggers a fully automated GitHub Actions pipeline: test → Docker build → push to GHCR → deploy to EC2 → health-check gate.

**Highlights:**
- **Infrastructure as Code** — Terraform-managed VPC, EC2, least-privilege IAM, S3, CloudWatch dashboard & alarms — zero manual console changes
- **CI/CD** — GitHub Actions, 2 jobs / 8 stages, tests gate every deployment, images published to GitHub Container Registry
- **Security by default** — non-root Docker container, NGINX security headers, encrypted + versioned S3, scoped IAM policies, no hardcoded credentials anywhere
- **Observability** — CloudWatch dashboard (4 widgets), 3 metric alarms, 4 log streams (bootstrap, NGINX access/error, application)
- **Load tested** — k6 at 20 concurrent VUs: **0.00% error rate**, 100% checks passed (3,546 / 3,546), p95 latency 417ms

> ⚙️ Documented trade-offs (SSH open for CI/CD, no HTTPS yet, single-instance) with the production fix for each — because a portfolio project should show what you'd change for real production, not pretend it's already there.

[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=for-the-badge&logo=github)](https://github.com/Vasanth1602/aws-devops-platform)
[![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)](https://www.terraform.io)
[![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://aws.amazon.com)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)](https://github.com/features/actions)

</td>
</tr>
</table>

<table>
<tr>
<td width="100%" valign="top">

### 🗳️ VoteSecure — DevOps Portfolio Journey 🚧 *Active Build*
**One application, evolved phase by phase — the same system growing the way real production infrastructure does**

Instead of building disconnected mini-projects, VoteSecure takes a single full-stack voting platform (FastAPI + React + PostgreSQL + Redis) and evolves it through progressive infrastructure phases — each one built, intentionally broken, documented, and shared.

**Completed phases:**
- **Phase 1 — Containerization** ✅ — Dockerized frontend + backend, Compose orchestration, health-check-gated startup, persistent volumes
- **Phase 2 — Reverse Proxy** ✅ — NGINX as the single public entry point, WebSocket-aware routing for Socket.io, backend never exposed to the host
- **Phase 3 — CI** ✅ — GitHub Actions, 5-stage fail-fast pipeline (lint → frontend validation → backend build → frontend build → smoke test), PR-gated merges to `main`

**Real incidents, documented like production postmortems:**
- `INC-001` — PostgreSQL container outage (Docker DNS vs. TCP connectivity)
- `INC-002` — Service discovery failure (`localhost` vs. Docker internal DNS)
- `INC-003` — NGINX WebSocket upgrade failure (silent fallback to long-polling)

> 💡 The learning driving this project: **availability doesn't guarantee functionality.** All three incidents passed basic health checks while the actual feature underneath was broken — that gap is what the incident reports exist to close.

**Up next:** CI failure simulations → AWS deployment → monitoring & observability (Prometheus/Grafana) → container registry & CD → Kubernetes.

Following the build-in-public series on [LinkedIn](https://linkedin.com/in/vasanth1602).

[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=for-the-badge&logo=github)](https://github.com/Vasanth1602/votesecure-devops-journey)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=flat-square&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactjs.org)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://www.docker.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)](https://www.postgresql.org)
[![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)](https://redis.io)

</td>
</tr>
</table>

---

## GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Vasanth1602&show_icons=true&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=0ea5e9&icon_color=0ea5e9&text_color=94a3b8&rank_icon=github" height="165"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Vasanth1602&layout=compact&theme=github_dark&hide_border=true&bg_color=0d1117&title_color=0ea5e9&text_color=94a3b8&langs_count=6" height="165"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Vasanth1602&theme=github-dark-blue&hide_border=true&background=0d1117&stroke=0ea5e9&ring=0ea5e9&fire=f97316&currStreakLabel=94a3b8&sideLabels=94a3b8&dates=475569" height="165"/>

</div>

---

## What I'm Building Toward

```python
goals = {
    "short_term":  ["AWS deployment for VoteSecure (Phase 4)", "Monitoring with Prometheus + Grafana (Phase 5)", "Container Registry + CD (Phase 6-7)"],
    "medium_term": ["Kubernetes migration for VoteSecure (Phase 8)", "AWS Solutions Architect Associate cert", "Helm charts"],
    "long_term":   ["Platform engineering", "Internal developer platforms", "Production-grade SRE practices"]
}
```

---

<div align="center">

*Open to DevOps / Cloud / MLOps internships and full-time entry-level roles*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:0f172a&height=100&section=footer" width="100%"/>

</div>
