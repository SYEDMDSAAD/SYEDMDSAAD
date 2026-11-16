<p align="center">
  <img src="assets/header.svg" width="100%" alt="Syed Mohammad Saad · Software Engineer · Building FinTwin AI, an AI money copilot for India" />
</p>

<p align="center">
  <a href="https://fintwin-web.azurewebsites.net"><img src="https://img.shields.io/badge/FinTwin_AI-Live_demo-7C3AED?style=for-the-badge&logo=googlechrome&logoColor=white" alt="FinTwin AI live demo" /></a>
  <a href="https://syedmdsaad.github.io/Portfolio/"><img src="https://img.shields.io/badge/Portfolio-6366F1?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/syedmdsaad/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:mdsaadsyed29@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

2026 Information Technology graduate from **Pune Institute of Computer Technology** (CGPA **8.94/10**).
I build backend systems in Java and Python that are secure, tested and made to keep running, and I'm
building **FinTwin AI**, an AI money copilot for young Indian earners, now live in public beta.
Merged contributions to **Elasticsearch** and **Apache Lucene**, and two published research papers.

**Open to backend / software engineer roles.** I write about backend engineering, security and
applied AI on [LinkedIn](https://www.linkedin.com/in/syedmdsaad/).

---

## FinTwin AI

An AI money copilot for young Indian earners. It reads bank and UPI statements, categorizes every
transaction, and answers money questions from the user's own numbers. Designed, built and run end to end.

**[Live demo: one click, no sign-up](https://fintwin-web.azurewebsites.net)** &nbsp;·&nbsp; [Source on GitHub](https://github.com/SYEDMDSAAD/FinTwin.ai)

<p align="center">
  <img src="assets/fintwin-architecture.svg" width="100%" alt="FinTwin AI architecture: browser, React web app, identity service, Java core API, Python AI service, LLM and PostgreSQL" />
</p>

| | |
|---|---|
| **Architecture** | 4 services: a React 19 + Vite frontend, a Spring Boot 3.5 (Java 21) core API, a separate identity service, and a Python FastAPI AI service, over PostgreSQL with 26 Flyway migrations |
| **Data in** | Bank statements as CSV, PDF or Excel and DKIM-verified bank alert emails, with Account Aggregator linking in testing. The categorizer learns from user corrections, and transfers between a user's own accounts are excluded |
| **AI** | Self-hosted LLM copilot (qwen2.5 on Ollama, on a GPU) with a tool-calling loop. The tools have no user-ID parameter and every question carries a short-lived token signed by the core API, so the model can't read another user's data. Code does the maths, and an eval suite of real questions, graded by code, measures every prompt or model change |
| **Security** | JWT with refresh-token rotation and reuse detection, TOTP 2FA, Google OAuth, RBAC via a custom Spring Security permission evaluator, and AES-256-GCM field-level encryption with an HMAC blind index |
| **Reliability** | Resilience4j circuit breakers with statistical fallbacks when the AI is down, rate limiting per IP and per user, Caffeine caching, HikariCP tuning, N+1 fixes and paginated batch jobs. Real EMI and debt-to-income maths, and a water-fill allocator for goal savings |
| **Delivery** | Docker, Azure App Service, Grafana monitoring with 8 alert rules, 6 GitHub Actions workflows, and **1,100+ automated tests** (Testcontainers on real PostgreSQL, pytest, Vitest) |

---

## Open Source

Merged contributions to large distributed-systems and search codebases:

| Project | Contribution |
|---|---|
| [elastic/elasticsearch](https://github.com/elastic/elasticsearch/pull/142940) | Documented the `http_schema` field in AlibabaCloudSearchService configuration |
| [apache/lucene](https://github.com/apache/lucene/pull/15719) | Improved JavaDocs for the `org.apache.lucene.util` package |
| [TheAlgorithms/Java](https://github.com/TheAlgorithms/Java/pull/7275) | Added `RemoveStars` and `ComplexNumberMultiply` string algorithms |

Beyond those, I've opened 30+ pull requests against Elasticsearch and Lucene, chasing flaky
tests, resource leaks in the chunked fetch phase, ESQL planner bugs and memory exhaustion in
lookup joins. Reading a codebase that large is its own skill, and it's where most of what I know
about distributed systems actually came from.

---

## Selected Projects

| Project | What it does | Stack |
|---|---|---|
| [Forge](https://github.com/SYEDMDSAAD/forge) | An Alexa+ MCP server that learns new skills while you talk to it: it writes, sandbox-tests and installs its own tools | TypeScript, MCP (Streamable HTTP) |
| [Bluewren](https://github.com/SYEDMDSAAD/bluewren) | A self-hosted MCP server for Alexa+ that rebooks, refunds and helps travelers by voice when a flight goes wrong | TypeScript, MCP (Streamable HTTP) |
| [Real-Time Chat Platform](https://github.com/SYEDMDSAAD/Chat-S.io) | One-to-one and group messaging with delivery-status tracking; JWT + bcrypt sessions, <50 ms delivery across concurrent sessions | MERN, Socket.io |
| [Hybrid Cryptography over TLS](https://github.com/SYEDMDSAAD/Cryptography) | Client–server channel on TLS 1.2 with ECDHE-RSA and AES-256-GCM, X.509 auth via Java KeyStore | Java, JSSE/JCA |
| [Hospital Management System](https://github.com/SYEDMDSAAD/HMS) | Patient booking, provider messaging and an admin panel, with scheduling conflicts caught before they hit the database | MERN |
| [Emotion-Driven Music Recommender](https://github.com/SYEDMDSAAD/EmotionalDrivenMusicRecommender) | Reads facial expression in real time to infer mood, then curates a matching Spotify queue | Python, OpenCV |

More on the [portfolio →](https://syedmdsaad.github.io/Portfolio/)

---

## Research &amp; Publications

**Yoga Pose Detection and Correction Using Machine Learning Approaches**<br>
*ICCCNT 2025, IIT Indore — IEEE*<br>
Real-time posture correction model using CNN, XGBoost and MediaPipe, achieving **92% pose accuracy**.

**Machine Learning Techniques for Detecting DoS and DDoS Attacks: Methods, Attacks and Datasets**<br>
*Indian Journal of Technical Education (ISTE), 2026*<br>
Intrusion detection system using MLP and LSTM, achieving **>99% accuracy** on CIC-IDS benchmarks.

---

## Experience

**Machine Learning Intern (Google AI/ML Virtual Internship)** — EduSkills Foundation · *Jan 2025 – Apr 2025*<br>
Implemented ML pipelines for classification and NLP using CNN and XGBoost across 50,000+ records,
improving accuracy 15–20%. Designed RESTful APIs for secure inter-service transmission, improving
transfer efficiency by 30%.

**Machine Learning Intern | Team Lead** — Pune Institute of Computer Technology · *Feb 2025 – Apr 2025*<br>
Built a real-time posture analysis system with MediaPipe, CNN, XGBoost and SVM: 20% accuracy gain,
35% better error detection, 25% faster processing. Led a 3-member team across design, deployment,
testing, performance tuning and UX. Published at IEEE ICCCNT 2025.

---

## Tech Stack

**Languages**

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)

**Backend &amp; APIs**

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-404040?style=for-the-badge&logo=express&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-404040?style=for-the-badge&logo=socketdotio&logoColor=white)

**AI**

![Ollama](https://img.shields.io/badge/LLMs_·_Ollama-404040?style=for-the-badge&logo=ollama&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-404040?style=for-the-badge&logo=modelcontextprotocol&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)

**Data &amp; Storage**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=for-the-badge&logo=flyway&logoColor=white)

**Cloud, DevOps &amp; Testing**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=black)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI%2FCD-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?style=for-the-badge&logo=junit5&logoColor=white)
![Testcontainers](https://img.shields.io/badge/Testcontainers-404040?style=for-the-badge&logo=testcontainers&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)

---

<p align="center">
  <i>Open to backend / software engineer roles · Pune, India</i>
</p>
