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

> Cách tính: với mỗi repo chạy `git log --no-merges --numstat --pretty=format:'@%aN'`, cộng dồn *added/removed* theo tác giả (không gộp alias), sắp xếp theo Net LoC.

<details><summary><b>s360-backend</b> — 22 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| khoapda | 126453 | 17862 | 108591 |
| mainhatnam219 | 37012 | 2167 | 34845 |
| notDuyLam | 53200 | 27513 | 25687 |
| Võ Hoàng Nguyên | 31914 | 7436 | 24478 |
| TNMonster | 14558 | 2897 | 11661 |
| 22120157 | 10837 | 1506 | 9331 |
| eNKay | 30697 | 23864 | 6833 |
| PhamGiaKhiem | 5909 | 1168 | 4741 |
| Pham Dao Anh Khoa | 7594 | 2938 | 4656 |
| khiempham123 | 2742 | 162 | 2580 |
| BrianTrac | 3109 | 544 | 2565 |
| Huynh Tan Loc | 5428 | 2899 | 2529 |
| copilot-swe-agent[bot] | 2370 | 1 | 2369 |
| 22120197 | 2234 | 208 | 2026 |
| phatnguyen1906 | 2064 | 275 | 1789 |
| NKhank11 | 700 | 32 | 668 |
| kiin21 | 134 | 123 | 11 |
| Anwirismee | 1 | 12 | -11 |
| Nguyen Phan Duc Khai | 12 | 178 | -166 |
| Huỳnh Tấn Lộc | 2634 | 6192 | -3558 |
| 22120186 | 11884 | 16053 | -4169 |
| Nguyễn Anh Hào | 63560 | 79049 | -15489 |

</details>

<details><summary><b>s360-frontend</b> — 20 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| Nguyễn Anh Hào | 151132 | 78639 | 72493 |
| phatnguyen1906 | 48267 | 13291 | 34976 |
| Võ Hoàng Nguyên | 32340 | 10419 | 21921 |
| BrianTrac | 29403 | 16002 | 13401 |
| Huynh Cong Minh | 22724 | 10731 | 11993 |
| 22120157 | 29011 | 17745 | 11266 |
| mainhatnam219 | 12785 | 2270 | 10515 |
| notDuyLam | 7935 | 1299 | 6636 |
| 22120197 | 9205 | 4839 | 4366 |
| Huỳnh Công Minh | 9094 | 6197 | 2897 |
| khiempham123 | 3159 | 648 | 2511 |
| 22120209 | 3949 | 2280 | 1669 |
| eNKay | 509 | 24 | 485 |
| Phạm Gia Khiêm | 292 | 31 | 261 |
| khoapda | 154 | 12 | 142 |
| TPL | 1275 | 1182 | 93 |
| Pham Dao Anh Khoa | 11 | 0 | 11 |
| NKhank11 | 1 | 1 | 0 |
| Nguyễn Vĩnh Lương | 1089 | 3349 | -2260 |
| PhamGiaKhiem | 42378 | 48072 | -5694 |

</details>

<details><summary><b>s360-web-admin</b> — 14 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| Nguyễn Anh Hào | 95259 | 39826 | 55433 |
| 22120157 | 20174 | 7652 | 12522 |
| 22120197 | 11033 | 450 | 10583 |
| phatnguyen1906 | 23481 | 17575 | 5906 |
| eNKay | 3952 | 157 | 3795 |
| mainhatnam219 | 2747 | 432 | 2315 |
| NKhank11 | 1154 | 315 | 839 |
| BrianTrac | 468 | 6 | 462 |
| 22120186 | 405 | 30 | 375 |
| Pham Dao Anh Khoa | 34 | 1 | 33 |
| kiin21 | 19 | 0 | 19 |
| khoapda | 38148 | 38734 | -586 |
| PhamGiaKhiem | 18954 | 20780 | -1826 |
| khiempham123 | 6390 | 9823 | -3433 |

</details>

<details><summary><b>s360-career-ai</b> — 4 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| khoapda | 54807 | 13863 | 40944 |
| copilot-swe-agent[bot] | 64 | 1 | 63 |
| kiin21 | 35 | 0 | 35 |
| Pham Dao Anh Khoa | 577 | 671 | -94 |

</details>

<details><summary><b>s360-ai</b> — 9 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| Võ Hoàng Nguyên | 26380 | 4977 | 21403 |
| notDuyLam | 6307 | 976 | 5331 |
| Nguyễn Anh Hào | 5147 | 508 | 4639 |
| TNMonster | 3340 | 467 | 2873 |
| Huỳnh Công Minh | 1564 | 319 | 1245 |
| eNKay | 390 | 9 | 381 |
| minh huynh | 229 | 31 | 198 |
| BrianTrac | 151 | 1 | 150 |
| khoapda | 20 | 0 | 20 |

</details>

<details><summary><b>s360-gitops</b> — 5 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| kiin21 | 461 | 135 | 326 |
| khoapda | 115 | 1 | 114 |
| Nguyễn Anh Hào | 17 | 0 | 17 |
| Pham Dao Anh Khoa | 11 | 0 | 11 |
| s360-cicd | 2 | 2 | 0 |

</details>

<details><summary><b>s360-devops</b> — 3 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| khoapda | 649 | 226 | 423 |
| kiin21 | 118 | 86 | 32 |
| Pham Dao Anh Khoa | 11 | 0 | 11 |

</details>

<details><summary><b>s360-iac</b> — 3 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| khoapda | 382 | 43 | 339 |
| kiin21 | 177 | 1 | 176 |
| Pham Dao Anh Khoa | 11 | 0 | 11 |

</details>

<!-- STATS:END -->
