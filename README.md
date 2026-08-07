## Garv Aggarwal

**Backend engineer — I design and operate distributed systems in production.**
Java &amp; Spring at scale, Go for systems projects, exploring LLMs &amp; AI infrastructure.

[![Portfolio](https://img.shields.io/badge/Portfolio-F59E0B?style=for-the-badge&logo=astro&logoColor=white)](https://garv2003.github.io)
[![System Designs](https://img.shields.io/badge/System_Designs-18181B?style=for-the-badge&logo=diagramsdotnet&logoColor=F59E0B)](https://garv2003.github.io/systems)
[![Blog](https://img.shields.io/badge/Blog-18181B?style=for-the-badge&logo=readthedocs&logoColor=F59E0B)](https://garv2003.github.io/blog/)
[![Résumé](https://img.shields.io/badge/Résumé-18181B?style=for-the-badge&logo=readdotcv&logoColor=white)](https://garv2003.github.io/resume.pdf)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/garvaggarwal05/)

---

## 🧭 System Design — explore it, don't just read it

Interactive case studies of systems I designed and shipped at Octro. **Trace a request through
the architecture, break it, and watch how it recovers** — with the tradeoff behind every decision:

| Case study | What it shows | Stack |
|---|---|---|
| **[Async Notification Pipeline →](https://garv2003.github.io/systems#notification)** | Decoupling push delivery from the request path so a slow third party can't stall the app; scaling it to 100M users | Amazon SQS · Redis · DLQ |
| **[Account Migration &amp; Merge →](https://garv2003.github.io/systems#merge)** | Merging guest → registered accounts — safe under partial failure, idempotent under retries, auditable end-to-end | 3 services · MongoDB · Redis |
| **[Real-time Leaderboard →](https://garv2003.github.io/systems#leaderboard)** | Live ranks with O(log N) updates, one push per interval, and recovery when the cache dies | Redis ZSET · WebSockets |

▶ **[Open the interactive case studies →](https://garv2003.github.io/systems)**

---

Backend engineer at **Octro Inc** (Best Performer), building distributed Java/Spring microservices
across a 54-service platform on AWS — WebSockets, RabbitMQ, Redis, MongoDB, ZooKeeper, and async
Amazon SQS pipelines, plus a polyglot Java ↔ TypeScript Lambda compute layer. I ship features
end-to-end and carry on-call.

## ⚙️ Systems & AI infrastructure I've built

Self-authored side projects — real code with tests, metrics, and design docs. Grouped by theme.

**Distributed systems**

| Project | What it demonstrates | Stack |
|---|---|---|
| **[wal-kv-store](https://github.com/Garv2003/wal-kv-store)** | Durable key-value store: write-ahead log → crash recovery → compaction → **Raft replication** (3-node), with fault-injection crash tests + a design doc | Go · hashicorp/raft |
| **[code-execution-engine](https://github.com/Garv2003/code-execution-engine)** | Runs untrusted code in hardened Docker sandboxes (drop-caps · no network · PID/mem limits), Redis job queue + worker pool, SSE result streaming, Prometheus metrics + threat model | Go · Docker · Redis |
| **[distributed-rate-limiter](https://github.com/Garv2003/distributed-rate-limiter)** | Pluggable strategies (token-bucket / sliding-window / Redis+Lua for cross-instance limits), HTTP + gRPC APIs, Prometheus, Docker Compose | Go · Redis · gRPC |
| **[payments-ledger](https://github.com/Garv2003/payments-ledger)** | Double-entry accounting service: idempotent transfers + transactional outbox — no double-spend, no dual-write races | Go · Postgres |
| **[cdc-pipeline](https://github.com/Garv2003/cdc-pipeline)** | Change-data-capture: DB change stream → Kafka → idempotent sink, with a dead-letter path + replication-lag metrics | Go · Mongo · Kafka |

**AI infrastructure & products**

| Project | What it demonstrates | Stack |
|---|---|---|
| **[llm-gateway](https://github.com/Garv2003/llm-gateway)** | OpenAI-compatible gateway that routes each request to the cheapest capable model + a semantic response cache + per-key rate limiting + cost metrics | Go · Redis |
| **[vidbite](https://github.com/Garv2003/vidbite)** | AI YouTube-video summarizer — full-stack, JWT auth, Dockerized and deploy-ready | React · Flask · Gemini |
| **[livepolls](https://github.com/Garv2003/livepolls)** | Real-time audience polling with a live word cloud (Slido-style) over WebSockets | socket.io · Redis pub/sub |

**Also:** [go-load-balancer](https://github.com/Garv2003/go-load-balancer) (HTTP LB · health checks · hot config reload via fsnotify) · [EnvBox](https://github.com/Garv2003/EnvBox) (env manager with client-side AES-GCM encryption) · [ssh-server](https://github.com/Garv2003/ssh-server) · [go-cli-tool](https://github.com/Garv2003/go-cli-tool)

## 🧰 Tech

**Languages**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**Backend &amp; Infrastructure**

![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-FF4438?style=for-the-badge&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Amazon SQS](https://img.shields.io/badge/Amazon%20SQS-FF4F8B?style=for-the-badge&logo=amazonsqs&logoColor=white)
![ZooKeeper](https://img.shields.io/badge/ZooKeeper-D22128?style=for-the-badge&logo=apache&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

## 🤝 Connect

[![Stack Overflow](https://img.shields.io/badge/Stack%20Overflow-F58025?style=for-the-badge&logo=stackoverflow&logoColor=white)](https://stackoverflow.com/users/22573280/garv-aggarwal?tab=profile)
[![Gmail](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aggarwalgarv0505@gmail.com)
![Followers](https://img.shields.io/github/followers/Garv2003?style=for-the-badge&logo=github&logoColor=white&label=Follow&color=18181B)
