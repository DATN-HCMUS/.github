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

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| khoapda | 220728 | 70741 | 149987 |
| Nguyễn Anh Hào | 315115 | 198022 | 117093 |
| Võ Hoàng Nguyên | 90634 | 22832 | 67802 |
| mainhatnam219 | 52544 | 4869 | 47675 |
| phatnguyen1906 | 73812 | 31141 | 42671 |
| notDuyLam | 67442 | 29788 | 37654 |
| 22120157 | 60022 | 26903 | 33119 |
| 22120197 | 22472 | 5497 | 16975 |
| BrianTrac | 33131 | 16553 | 16578 |
| TNMonster | 17898 | 3364 | 14534 |
| Huynh Cong Minh | 22724 | 10731 | 11993 |
| eNKay | 35548 | 24054 | 11494 |
| Pham Dao Anh Khoa | 8183 | 3610 | 4573 |
| Huỳnh Công Minh | 10658 | 6516 | 4142 |
| Huynh Tan Loc | 5428 | 2899 | 2529 |
| copilot-swe-agent[bot] | 2434 | 2 | 2432 |
| 22120209 | 3949 | 2280 | 1669 |
| khiempham123 | 12291 | 10633 | 1658 |
| NKhank11 | 1855 | 348 | 1507 |
| kiin21 | 934 | 345 | 589 |
| Phạm Gia Khiêm | 292 | 31 | 261 |
| minh huynh | 229 | 31 | 198 |
| TPL | 1275 | 1182 | 93 |
| s360-cicd | 1 | 1 | 0 |
| Anwirismee | 1 | 12 | -11 |
| Nguyen Phan Duc Khai | 12 | 178 | -166 |
| Nguyễn Vĩnh Lương | 1089 | 3349 | -2260 |
| PhamGiaKhiem | 67241 | 70020 | -2779 |
| Huỳnh Tấn Lộc | 2634 | 6192 | -3558 |
| 22120186 | 12289 | 16083 | -3794 |

<!-- STATS:END -->
