<h1 align="center">Syed Mohammad Saad</h1>

<p align="center">
  <b>Software Engineer</b> &nbsp;·&nbsp; Secure, scalable distributed systems in Java and Python
</p>

<p align="center">
  <a href="https://syedmdsaad.github.io/Portfolio/"><img src="https://img.shields.io/badge/Portfolio-6366F1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/syed-mohammad-saad-640144213/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:mdsaadsyed29@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

2026 Information Technology graduate from **Pune Institute of Computer Technology** (CGPA **8.94/10**).
I build backends that hold up under load — and the schemas, deployment pipelines and test suites
around them. Two published research papers, and merged contributions to
**Elasticsearch** and **Apache Lucene**.

Currently looking for a full-time software engineering role starting **mid-2026**.

---

## Flagship — FinTwin.ai

An AI-powered personal finance platform with bank-account aggregation via Setu AA, plus budget,
goal, investment and net-worth engines featuring real EMI &amp; DTI computation and a water-fill
savings-allocation algorithm. **Architected and shipped end to end, solo.**

| | |
|---|---|
| **Architecture** | Production-grade **4-service distributed system** — React + Vite frontend, Spring Boot (Java 21) core API, a separate identity service, and a Python/FastAPI AI service over PostgreSQL with 14 Flyway migrations |
| **Security** | JWT auth with refresh-token rotation and theft detection, TOTP 2FA, Google OAuth, RBAC via a custom Spring Security permission evaluator, and AES-256-GCM field-level encryption of financial data |
| **AI** | Self-hosted LLM copilot on **Ollama** (qwen2.5 / phi3) driven by an OpenAI-style tool-calling loop — the model fetches user data through a secured internal API instead of being prompt-stuffed, with no paid API dependency |
| **Performance** | Eliminated N+1 query hotspots via Redis-backed distributed rate limiting, Caffeine caching, HikariCP tuning, paginated batch jobs replacing full-table scans, and parallel market-data fetching |
| **Delivery** | Docker + **Kubernetes** (HPA 2 → 10 replicas, zero-downtime rolling deploys), Prometheus/Grafana monitoring, 5 CI/CD workflows, **~180 automated tests** (48 Testcontainers, 129 pytest) |

---

## Tech Stack

**Languages**

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)

**Backend &amp; APIs**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socketdotio&logoColor=white)

**Data &amp; Storage**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white)

**Cloud &amp; DevOps**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

**Frontend &amp; ML**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

---

## Open Source

Merged contributions to large distributed-systems and search codebases:

| Project | Contribution |
|---|---|
| [elastic/elasticsearch](https://github.com/elastic/elasticsearch/pull/142940) | Documented the `http_schema` field in AlibabaCloudSearchService configuration |
| [apache/lucene](https://github.com/apache/lucene/pull/15719) | Improved JavaDocs for the `org.apache.lucene.util` package |
| [TheAlgorithms/Java](https://github.com/TheAlgorithms/Java/pull/7275) | Added `RemoveStars` and `ComplexNumberMultiply` string algorithms |

Beyond those, I've opened 30+ pull requests against Elasticsearch and Lucene — chasing flaky
tests, resource leaks in the chunked fetch phase, ESQL planner bugs and memory exhaustion in
lookup joins. Reading a codebase that large is its own skill, and it's where most of what I know
about distributed systems actually came from.

---

## Research &amp; Publications

**Yoga Pose Detection and Correction Using Machine Learning Approaches**
*ICCCNT 2025, IIT Indore — IEEE*
Real-time posture correction model using CNN, XGBoost and MediaPipe, achieving **92% pose accuracy**.

**Machine Learning Techniques for Detecting DoS and DDoS Attacks: Methods, Attacks and Datasets**
*Indian Journal of Technical Education (ISTE), 2026*
Intrusion detection system using MLP and LSTM, achieving **>99% accuracy** on CIC-IDS benchmarks.

---

## Experience

**Google AI/ML Virtual Internship** — Eduskills · *Jan 2025 – Apr 2025*
Implemented ML pipelines for classification and NLP using CNN and XGBoost across 50,000+ records,
improving accuracy 15–20%. Designed RESTful APIs for secure inter-service transmission, improving
transfer efficiency by 30%.

**Yoga Pose Detection Internship** — Pune Institute of Computer Technology · *Feb 2025 – Apr 2025*
Built a real-time posture analysis system with MediaPipe, CNN, XGBoost and SVM — 20% accuracy gain,
35% better error detection, 25% faster processing. Led a 3-member team across design, deployment,
testing, performance tuning and UX.

---

## Selected Projects

| Project | What it does | Stack |
|---|---|---|
| [Real-Time Chat Platform](https://github.com/SYEDMDSAAD/Chat-S.io) | One-to-one and group messaging with delivery-status tracking; JWT + bcrypt sessions, <50 ms delivery across concurrent sessions | MERN, Socket.io |
| [Hybrid Cryptography over TLS](https://github.com/SYEDMDSAAD/Cryptography) | Client–server channel on TLS 1.2 with ECDHE-RSA and AES-256-GCM, X.509 auth via Java KeyStore | Java, JSSE/JCA |
| [Hospital Management System](https://github.com/SYEDMDSAAD/HMS) | Patient booking, provider messaging and an admin panel, with scheduling conflicts caught before they hit the database | MERN |
| [Emotion-Driven Music Recommender](https://github.com/SYEDMDSAAD/EmotionalDrivenMusicRecommender) | Reads facial expression in real time to infer mood, then curates a matching Spotify queue | Python, OpenCV |
| [Food Reservation System](https://github.com/SYEDMDSAAD/RestBackend) | Table booking and pre-ordering with validation that prevents double-booking | Node.js, Express, MongoDB |

More on the [portfolio →](https://syedmdsaad.github.io/Portfolio/)

---

<p align="center">
  <i>Open to software engineering roles starting mid-2026 · Pune, India</i>
</p>
