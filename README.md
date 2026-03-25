<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:1e3a5f,100:0ea5e9&height=200&section=header&text=Vasanth%20A&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=DevOps%20%7C%20Cloud%20Infrastructure%20%7C%20MLOps&descSize=18&descAlignY=58&descColor=94d2ff&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=800&color=0EA5E9&center=true&vCenter=true&width=700&lines=Building+production-grade+cloud+infrastructure;Automating+EC2+%E2%86%92+ECS+Fargate+deployments;Terraform+%7C+Docker+%7C+AWS+%7C+CI%2FCD;Turning+30-min+manual+setups+into+5-min+pipelines)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-vasanth1602-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/vasanth1602)
[![GitHub](https://img.shields.io/badge/GitHub-Vasanth1602-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Vasanth1602)
[![Email](https://img.shields.io/badge/Email-kumarajith85666%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kumarajith85666@gmail.com)

</div>

---

## About Me

I'm a DevOps-focused engineer and M.Sc. Data Science student (Periyar University, 2024–2026) with a strong interest in cloud infrastructure, automation, and MLOps. I build platforms that take ML applications from a GitHub URL to a live, production-ready deployment — fully automated, containerised, and observable.

My work sits at the intersection of **infrastructure as code**, **CI/CD automation**, and **cloud-native architecture**. I don't just deploy apps — I build the platforms that deploy them.

```text
🏗️  Currently working on   →  ECS Fargate + Terraform IaC for ML Deployment Platform
☁️  Cloud focus             →  AWS (EC2, ECS Fargate, ALB, RDS, Secrets Manager, ECR)
🔧  Automation passion      →  Replacing manual workflows with repeatable pipelines
📚  Learning                →  Terraform modules, GitHub Actions
📍  Based in               →  Tamil Nadu, India
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
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-336791?style=flat-square&logo=postgresql&logoColor=white)](https://www.postgresql.org)

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
**One-click ML deployment from GitHub URL to production AWS infrastructure**

A self-service MLOps platform that eliminates manual server configuration. Enter a GitHub repo URL — the platform provisions EC2, installs Docker, configures NGINX, builds your image, and streams real-time deployment logs to a React dashboard via WebSocket.

**Architecture highlights:**
- **Dual deployment targets** — EC2 (SSH-based) + ECS Fargate (serverless containers)
- **Infrastructure as Code** — full Terraform modules for VPC, ALB, ECS cluster, RDS, ECR, Cloud Map
- **Production networking** — Multi-AZ VPC · Public/private subnets · ALB with path-based routing
- **Secure by design** — Secrets Manager, IAM least-privilege, no static credentials
- **Full stack** — Flask/Gunicorn · React 19/Vite · PostgreSQL 16 · SQLAlchemy + Alembic
- **Observability** — Real-time WebSocket deployment logs · JWT-secured API · Rate limiting

> ⚡ Reduces a 30-minute manual EC2 setup to a single API call in **3–5 minutes**

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
<td width="50%" valign="top">

### 🔁 Jenkins CI/CD Automation Pipeline
**Pipeline-as-code with automated testing, PR gating, and deployment**

Declarative Jenkins pipeline that automates the full build-test-merge-deploy lifecycle for a Flask application. Integrates with the GitHub API to enforce test-gated PR merges — only passing builds reach `main`.

**Key features:**
- Declarative `Jenkinsfile` pipeline (build → test → merge → deploy)
- GitHub API integration for automated PR management
- Unit-test gating: failing tests block merges to `main`
- Virtual environment isolation and dependency management
- Consistent, repeatable builds on every code push

[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=flat-square&logo=github)](https://github.com/Vasanth1602/jenkins_workflow)
[![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)](https://www.jenkins.io)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)

</td>
<td width="50%" valign="top">

### 📡 Wi-Fi IP Switcher
**Windows automation tool for automatic static IP / DHCP switching**

A background Windows service that detects the active Wi-Fi SSID and automatically switches between static IP and DHCP configurations — no manual network changes needed when moving between networks.

**Key features:**
- SSID-aware background monitor (Python threading)
- System tray integration with live status
- Flask-based web UI for configuration management
- Automated startup via Windows Task Scheduler (elevated)
- JSON-based config persistence + structured logging
- Packaged as a standalone `.exe` (PyInstaller + Inno Setup)

[![Repo](https://img.shields.io/badge/View%20Repo-181717?style=flat-square&logo=github)](https://github.com/Vasanth1602/wifi_switcher)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Windows](https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white)](https://www.microsoft.com/windows)

</td>
</tr>
</table>

---

## AWS Architecture — ML Deployment Platform (ECS Fargate)

```
                        Internet
                            │ HTTP :80
              ┌─────────────▼──────────────┐
              │   Application Load Balancer │   internet-facing · public subnets · 2 AZs
              │   Rule 1:  /api/*      ───► btg (backend :5000)
              │   Rule 2:  /socket.io/*───► btg (backend :5000)
              │   Default: /          ───► ftg (frontend :80)
              └──────────┬─────────────────┘
                         │             private subnets
          ┌──────────────┘──────────────────────┐
          ▼                                      ▼
  ┌───────────────┐   Cloud Map / Service    ┌──────────────────┐
  │  Frontend ECS │   Connect                │   Backend ECS    │
  │  Nginx :80    │◄─ backend.local:5000 ───►│  Flask/Gunicorn  │
  │  (ftg)        │                          │  :5000  (btg)    │
  └───────────────┘                          └────────┬─────────┘
                                                      │ :5432
                                             ┌────────▼─────────┐
                                             │  RDS PostgreSQL   │
                                             │  DB subnet group  │
                                             └──────────────────┘
```

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
    "short_term":  ["Kubernetes (EKS)", "GitHub Actions advanced workflows", "Monitoring (Prometheus + Grafana)"],
    "medium_term": ["AWS Solutions Architect Associate cert", "Helm charts", "Service mesh (Istio)"],
    "long_term":   ["Platform engineering", "Internal developer platforms", "MLOps at scale"]
}
```

---

<div align="center">

*Open to DevOps / Cloud / MLOps internships and entry-level roles*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:0f172a&height=100&section=footer" width="100%"/>

</div>
