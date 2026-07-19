# Student360 (S360)

Career & student-lifecycle platform — capstone project (HCMUS).
Connects students with jobs via AI matching, profile management, and an HR recruitment portal.

## Services

| Repo | Role | Stack |
|------|------|-------|
| **s360-backend** | Core REST API | NestJS · TypeORM · PostgreSQL · BullMQ/Redis |
| **s360-ai** | AI gateway & chatbot | FastAPI |
| **s360-career-ai** | AI job ↔ candidate matching | Embeddings · Knowledge Graph (Neo4j) · pgvector |
| **s360-web-admin** | HR / admin portal | React · Cloudflare Pages |
| **s360-gitops** · **s360-devops** · **s360-iac** | GitOps · CI/CD · Infrastructure | ArgoCD · GitHub Actions · Terraform |

## Infrastructure

- **Kubernetes (k3s) + ArgoCD** — GitOps, branch-per-env prod/staging deploys
- **CI/CD** — GitHub Actions reusable workflows (build → semver → auto-deploy)
- **AWS** — EC2 (k3s), RDS PostgreSQL · **RunPod** — GPU for AI matching

📊 **Service health:** https://status.api-backend.me

## Contributors (LoC by author, auto-updated)

<!-- STATS:START -->

> Method: per repo run `git log --all --no-merges --numstat --pretty=format:'@%aN'` (all branches, incl. unmerged), sum added/removed per author (no alias merge), sorted by Net LoC.

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
| phatnguyen1906 | 51488 | 14042 | 37446 |
| Võ Hoàng Nguyên | 32770 | 10651 | 22119 |
| BrianTrac | 29403 | 16002 | 13401 |
| Huynh Cong Minh | 25367 | 12381 | 12986 |
| mainhatnam219 | 14948 | 2271 | 12677 |
| notDuyLam | 14834 | 2174 | 12660 |
| 22120157 | 29348 | 17786 | 11562 |
| 22120197 | 13984 | 5232 | 8752 |
| khiempham123 | 5961 | 2390 | 3571 |
| Huỳnh Công Minh | 11579 | 9688 | 1891 |
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
| 22120157 | 20471 | 7703 | 12768 |
| 22120197 | 12462 | 452 | 12010 |
| phatnguyen1906 | 23481 | 17575 | 5906 |
| eNKay | 3952 | 157 | 3795 |
| mainhatnam219 | 2747 | 432 | 2315 |
| NKhank11 | 1154 | 315 | 839 |
| BrianTrac | 468 | 6 | 462 |
| 22120186 | 405 | 30 | 375 |
| Pham Dao Anh Khoa | 34 | 1 | 33 |
| kiin21 | 19 | 0 | 19 |
| PhamGiaKhiem | 20436 | 21329 | -893 |
| khoapda | 41017 | 42460 | -1443 |
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

<details><summary><b>s360-ai</b> — 10 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| Võ Hoàng Nguyên | 38538 | 8011 | 30527 |
| notDuyLam | 6307 | 976 | 5331 |
| Nguyễn Anh Hào | 5147 | 508 | 4639 |
| TNMonster | 3340 | 467 | 2873 |
| Huỳnh Công Minh | 1564 | 319 | 1245 |
| eNKay | 390 | 9 | 381 |
| minh huynh | 229 | 31 | 198 |
| BrianTrac | 151 | 1 | 150 |
| khoapda | 20 | 0 | 20 |
| kiin21 | 0 | 51 | -51 |

</details>

<details><summary><b>s360-gitops</b> — 5 authors</summary>

| Author | Added | Removed | Net LoC |
|---|--:|--:|--:|
| kiin21 | 519 | 192 | 327 |
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
