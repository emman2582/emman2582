## Hi there 👋

# Emmanuel "Emman" Comia — DevOps | Cloud | SRE

Canadian DevOps/SRE with 19 years in software + 5 years in platform automation. I build secure, observable, reliable delivery platforms on AWS/Kubernetes with Terraform, Ansible, and GitHub Actions.

**Focus:** EKS • IaC (Terraform/Ansible) • CI/CD (Actions/Jenkins) • Observability (Prometheus/Grafana/Loki) • Security (CodeQL/OWASP/Burp) • Cost-aware architectures

**Certs:** AWS SAA-C03, PMI-ACP, PSM I — Based in North York, ON, Canada

---

### Portfolio

| Project | Stack | What it does |
|---|---|---|
| [**LinkShort**](https://github.com/emman2582/linkshortenerproject) | Next.js 16 · TypeScript · Clerk · Drizzle ORM · Neon PostgreSQL · Tailwind CSS v4 | Full-stack authenticated URL shortener with per-user link ownership, custom slugs, CSRF-protected Server Actions, and defence-in-depth security headers. |
| [**vprofile-action**](https://github.com/emman2582/vprofile-action) | GitHub Actions · SonarQube · Maven · Docker · AWS ECR · EKS · Helm | 3-stage GitHub Actions pipeline: quality gate (SonarQube) → immutable Docker artifact (ECR) → Helm deploy to EKS. Quality gate hard-blocks on security findings. |
| [**iac-vprofile**](https://github.com/emman2582/iac-vprofile) | Terraform · AWS VPC · EKS · GitHub Actions | GitOps IaC: plan-on-PR, apply-on-merge. Provisions full AWS landing zone (VPC, public/private subnets, NAT, EKS) with remote S3 state + locking. |
| [**devops4sure**](https://github.com/emman2582/devops4sure) | GitHub Actions · Terraform · AWS ECR · EKS · SonarQube · Nexus | Monorepo combining app pipeline and IaC into a single 3-layer DevOps platform: source+pipeline → artifact registry → infrastructure. |
| [**resilience4j-sample**](https://github.com/emman2582/resilience4j-sample) | Spring Boot 3 · Resilience4j · Prometheus · Grafana · Docker · Kubernetes · AWS Lambda | All five Resilience4j fault tolerance patterns (Circuit Breaker, Retry, Rate Limiter, Bulkhead, Time Limiter) with live Prometheus/Grafana observability. Deployable to K8s and Lambda. |
| [**vprokube**](https://github.com/emman2582/vprokube) | Kubernetes · Spring Boot · MySQL · Memcached · RabbitMQ · ElasticSearch · Ansible · Jenkins | Multi-tier K8s deployment with cache-aside (Memcached), async messaging (RabbitMQ), and full-text search (ElasticSearch). Jenkins pipeline for image build + deploy. |
| [**proton**](https://github.com/emman2582/proton) | Vagrant · Ansible · Tomcat · MySQL · Memcached · RabbitMQ · ElasticSearch | 5-VM local multi-tier stack provisioned with Ansible. Mirrors production topology for realistic network simulation — stepping stone from local to AWS. |
| [**Grafana Observability Lab**](https://github.com/emman2582/grafana) | Grafana 11.2.0 · MySQL · Loki · Prometheus · Grafana Alloy · Vagrant · Ubuntu 24.04 | Reproducible Vagrant lab for Grafana + MySQL. Covers dashboards, LogQL, alerting, Nginx/TLS, Grafana Cloud, and Alloy migration from Promtail. |
| [**devops**](https://github.com/emman2582/devops) | Bash · Python · Docker · Kubernetes · Jenkins · Maven | Curated command runbook and working examples for Docker, Kubernetes, Git, Jenkins pipelines, Maven, Linux, and Bash — built up over years of platform work. |
| [**terraform-provider-aws**](https://github.com/emman2582/terraform-provider-aws) | Go · Terraform Plugin SDK · AWS APIs | Reference fork of hashicorp/terraform-provider-aws for studying provider internals: CRUD lifecycle, eventual consistency waiters, and state reconciliation patterns. |

---

### Systems Design Patterns I Apply

| Pattern | Where |
|---|---|
| **Pipeline-as-Code** | vprofile-action, devops4sure — delivery workflow version-controlled, reviewable, auditable |
| **Immutable Infrastructure** | vprofile-action — ECR images tagged by run number; rollback = tag change, no rebuild |
| **GitOps** | iac-vprofile, devops4sure — PR triggers plan; merge triggers apply; Git history = audit log |
| **Declarative IaC** | iac-vprofile — desired-state model with remote state locking and drift detection |
| **Circuit Breaker / Bulkhead** | resilience4j-sample — application-layer fault isolation, cascading failure prevention |
| **Cache-Aside** | vprokube, proton — Memcached reduces DB read load with TTL-based invalidation |
| **Async Decoupling** | vprokube, proton — RabbitMQ offloads long-running ops from HTTP threads |
| **Multi-Tier Architecture** | vprokube, proton — stateless app tier + stateful backing services with PVC |
| **Shift-Left Quality** | devops4sure, vprofile-action — SonarQube gate runs before artifact creation |
| **Network Isolation** | iac-vprofile — public/private subnet split, NAT Gateway, least-exposure principle |

---

### Work with me

I'm available for freelance DevOps/SRE engagements:
- GitHub Actions / Jenkins CI/CD pipeline design (test → build → deploy)
- AWS infrastructure design and provisioning (VPC, EKS, RDS, IAM)
- Terraform codebase reviews and GitOps pipeline setup
- Kubernetes platform hardening and observability (Prometheus/Grafana)
- SonarQube quality gate and OWASP security integration

[LinkedIn](https://www.linkedin.com/in/emmanuelcomia/) · [Email](mailto:emman_job@yahoo.com)

---

![GitHub stats](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-informational)
![IaC](https://img.shields.io/badge/IaC-Terraform%20%7C%20Ansible-informational)
![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-informational)
![AWS](https://img.shields.io/badge/AWS-SAA--C03-orange)
