# Student360 (S360)

Nền tảng career & student-lifecycle — đồ án tốt nghiệp (HCMUS).
Kết nối sinh viên với việc làm bằng AI matching, quản lý hồ sơ, và cổng tuyển dụng cho HR.

## Services

| Repo | Vai trò | Stack |
|------|---------|-------|
| **s360-backend** | REST API core | NestJS · TypeORM · PostgreSQL · BullMQ/Redis |
| **s360-ai** | AI gateway & chatbot | FastAPI |
| **s360-career-ai** | AI matching job ↔ candidate | Embeddings · Knowledge Graph (Neo4j) · pgvector |
| **s360-web-admin** | Cổng HR / admin | React · Cloudflare Pages |
| **s360-gitops** · **s360-devops** · **s360-iac** | GitOps · CI/CD · Infrastructure | ArgoCD · GitHub Actions · Terraform |

## Hạ tầng

- **Kubernetes (k3s) + ArgoCD** — GitOps, deploy prod/staging tách nhánh
- **CI/CD** — GitHub Actions reusable workflows (build → semver → auto-deploy)
- **AWS** — EC2 (k3s), RDS PostgreSQL · **RunPod** — GPU cho AI matching

📊 **Service health:** https://status.api-backend.me

## Contributors (LoC by author, auto-updated)

<!-- STATS:START -->

_updating…_

<!-- STATS:END -->
