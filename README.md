<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=220&text=Samuel%20Nahas&fontAlign=50&fontAlignY=40&color=0:0F2027,50:203A43,100:2C5364&fontColor=ffffff&desc=Software%20Engineer%20%7C%20AI%20and%20Backend%20Engineering&descAlign=50&descAlignY=60" />
</p>

<p align="center">
  Building <b>backend systems, full-stack applications, data pipelines and AI-powered products.</b>
</p>

<p align="center">
  Computer Science student at <b>Universidade Federal de Mato Grosso do Sul (UFMS)</b><br>
  with international academic experience at <b>Leuphana University Lüneburg, Germany 🇩🇪</b>
</p>

<br>

<div align="center">

### 🌐 Connect with me

<a href="https://www.linkedin.com/in/samuel-nahas-23b809281">
  <img src="https://img.shields.io/badge/LinkedIn-203A43?style=for-the-badge&logo=linkedin&logoColor=white">
</a>
<a href="https://github.com/SamuelNahas">
  <img src="https://img.shields.io/badge/GitHub-203A43?style=for-the-badge&logo=github&logoColor=white">
</a>

</div>

<br>

<div align="center">

### 💻 Technologies & Tools

<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/spring/spring-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg">
<img height="38" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg">

<br><br>

<img src="https://img.shields.io/badge/REST_APIs-203A43?style=flat-square">
<img src="https://img.shields.io/badge/LLM_Integration-203A43?style=flat-square">
<img src="https://img.shields.io/badge/RAG-203A43?style=flat-square">
<img src="https://img.shields.io/badge/Vector_Search-203A43?style=flat-square">
<img src="https://img.shields.io/badge/WebSockets-203A43?style=flat-square">
<img src="https://img.shields.io/badge/CI/CD-203A43?style=flat-square">

</div>

<br>

## 💼 Professional Experience

### 🤖 ClickTI — AI Pre-Sales Automation (RAG)

I work at **ClickTI** on an AI product that **automates the pre-sales process**, built around a **Retrieval-Augmented Generation (RAG) pipeline** that turns documents into grounded, LLM-generated answers for the pre-sales team.

**Document ingestion → Embeddings → Vector Search → Context Retrieval → LLM → Structured output**

My work involves:

- building the RAG pipeline end to end, from document ingestion and processing to retrieval and generation
- embeddings and semantic/vector search over the ingested documents
- LLM integration and prompt design for reliable, grounded outputs
- backend APIs with FastAPI and PostgreSQL persistence
- containerized services, testing and deployment
- running accelerated/local AI workloads on **NVIDIA DGX Spark**

> Active commercial project — client information, datasets, business rules and model configuration are intentionally not disclosed.

**Tech:** `Python` · `FastAPI` · `PostgreSQL` · `Embeddings` · `Vector Search` · `RAG` · `LLMs` · `Docker` · `NVIDIA DGX Spark`

<br>

## 🚀 Featured Projects

### 🌹 Rote Rosen — AI Audience Analytics Platform

Large-scale AI and data engineering project developed at **Leuphana University Lüneburg** in collaboration with the German television production **Rote Rosen**.

The platform automatically collects audience discussions and transforms them into structured analytics through a multi-service pipeline involving **web crawling, PostgreSQL, FastAPI and Large Language Models**.

Key features include:

- automated weekly forum data collection
- sentiment analysis with positive, neutral and negative classification
- LLM-generated contextual explanations
- evidence-based sentiment analysis linked to original audience posts
- engagement and discussion metrics
- character mention analysis
- AI-generated character discussion summaries
- historical weekly analytics
- PostgreSQL caching to avoid unnecessary LLM recomputation
- React/TypeScript analytical dashboard

I worked primarily on the **backend and analytical architecture**, including FastAPI services, sentiment pipelines, LLM integration, PostgreSQL persistence, caching, webhook processing and Dockerized services.

**Tech:** `Python` · `FastAPI` · `PostgreSQL` · `Pandas` · `LLMs` · `React` · `TypeScript` · `Docker`

[View organization →](https://github.com/orgs/AIProjectRoteRosen/repositories)

<br>

### 🔢 SVHN Digit Classification — Deep Learning

Neural network study on the **Street View House Numbers** dataset, progressing from a linear classifier to MLPs, CNNs and ensembles, with every decision made on validation data only.

Highlights:

- 30 controlled experiments (optimizers, regularization, augmentation, cutout, label smoothing, depth vs. width)
- **119 training runs on two NVIDIA DGX Spark** machines, with a pre-registered experiment plan
- test-time augmentation and a final **ensemble of 20 CNNs: 97.89% test accuracy**
- reproducible pipeline with cached results/weights and CI that runs the notebook on every PR
- LaTeX report with tables and figures generated from the results

**Tech:** `Python` · `PyTorch` · `Jupyter` · `NVIDIA DGX Spark` · `LaTeX` · `GitHub Actions`

[Repository →](https://github.com/SamuelNahas/svhn-classificacao)

<br>

### 🏨 HospedaBem — Hotel Management Desktop System

Desktop system for hotel front desks covering **reservations, room availability, check-in, consumption and check-out with payment**, built for the Object-Oriented Analysis and Design course at UFMS.

Highlights:

- layered MVC architecture (`view → controller → service → DAO`) with GRASP patterns
- Spring Boot as a DI and transaction container, without a web server
- concurrency-safe rules enforced in PostgreSQL (row locks, partial unique indexes, `CHECK`)
- atomic check-in/check-out transactions, verified with injected failures
- **207 automated tests** (unit, integration with real PostgreSQL, JavaFX E2E)
- **mutation testing (PIT) at 96%**
- CI on every Pull Request: Checkstyle, build, tests on headless JavaFX and mutation

**Tech:** `Java 17` · `JavaFX` · `Spring Boot` · `Spring JDBC` · `PostgreSQL` · `JUnit 5` · `PIT` · `GitHub Actions`

[Repository →](https://github.com/SamuelNahas/hospedabem)

<br>

### 😂 ComedyHub — Meme & Comedy Social Platform

**[ComedyHub](https://thecomedyhub.com.br/)** is a real, live social platform for **sharing and interacting with memes and comedy content**. I was part of the team that built it, working on the platform's backend and API.

ComedyHub is a complete multi-client ecosystem rather than a simple CRUD application:

- Java / Spring Boot backend with PostgreSQL and Redis for caching and queues
- versioned REST API (v2) plus secure WebSocket connections for real-time events
- React + Vite web application and React Native mobile app
- JWT authentication, roles and rate limiting
- posts, comments, likes, sharing, private collections and chat
- real-time notifications (email and push)
- media uploads with dedicated compression and moderation microservices
- standardized validation and API error handling

**Tech:** `Java` · `Spring Boot` · `Spring Security` · `PostgreSQL` · `Redis` · `React` · `React Native` · `JWT` · `WebSockets` · `Microservices`

[Live Platform →](https://thecomedyhub.com.br/) · [Developer Docs & Dev Diary →](https://comedyblog.omeninotech.com) · [GitHub Organization →](https://github.com/ComedyHub)

> I'm no longer part of the organization; the code lives in its private repositories.

<br>

### 📊 SH Meta Games

Competitive **Pokémon TCG metagame analytics platform** built from public tournament data.

The application processes tournament results to generate:

- metagame representation
- deck performance statistics
- BO1 and BO3 matchup analysis
- representative decklists
- tournament history
- personal Battle Journal
- automated tournament collection
- scheduled data updates
- optional Supabase synchronization

**Tech:** `Next.js` · `React` · `TypeScript` · `Python` · `Supabase` · `GitHub Actions`

[Repository →](https://github.com/SamuelNahas/Limitless-stats) · [Live Application →](https://samuelnahas.github.io/Limitless-stats/)

<br>

### 🏆 TCG Tournament Check

Full-stack tournament operations platform developed for use by **Pokémon TCG judges and tournament organizers during real competitive events**.

Features include:

- tournament management
- player and judge accounts
- digital decklist submission
- Pokémon TCG Live imports
- automatic deck validation
- physical deck-check workflow
- tournament occurrences and penalties
- PDF reports
- responsive desktop, mobile and iPad interface
- automated deployment using a self-hosted GitHub Actions runner

**Tech:** `TypeScript` · `Node.js` · `SQLite` · `Docker` · `Nginx` · `GitHub Actions`

> Private repository — developed for real tournament operations.

<br>

### 🖥️ HVComp

Educational computing project based on the **Hypothetical Computer (HV)** model.

The platform helps students understand fundamental concepts including:

- CPU execution
- memory
- machine instructions
- machine language
- program execution
- computer architecture

The project is also connected to academic research involving **Computer Science Education and Design Science Research**.

[hvcomp.io →](https://hvcomp.io)

<br>

### 🃏 Pokémon TCG Master Set

Collection management application combining several Pokémon TCG data sources to build a unified catalog of Brazilian, international and Japanese card releases.

Includes:

- collection tracking
- variants and rarity filtering
- card image resolution
- completion statistics
- JSON backups
- automatically generated visual checklists

**Tech:** `JavaScript` · `HTML` · `CSS` · `REST APIs` · `GitHub Actions`

[Repository →](https://github.com/SamuelNahas/my-master-set)

<br>

## 🎓 Education

**B.Sc. Computer Science**  
Universidade Federal de Mato Grosso do Sul — UFMS 🇧🇷

**International Exchange Studies**  
Leuphana University Lüneburg 🇩🇪

**Technical Diploma in Informatics (Integrated High School)**  
Universidade Federal de Mato Grosso do Sul — UFMS 🇧🇷

## 🌍 Languages

**English — B2 (Upper-Intermediate)**  
Cambridge English proficiency exam

<br>

<div align="center">

### Currently interested in

**Backend Engineering · Software Architecture · RAG · AI Applications · Data Engineering · Full-Stack Development**

<br>

<a href="https://www.linkedin.com/in/samuel-nahas-23b809281">
  <img src="https://img.shields.io/badge/Let's_connect-203A43?style=for-the-badge&logo=linkedin&logoColor=white">
</a>

</div>
