<div align="center">

# Samuel Nahas

### Software Developer · Computer Science @ UFMS

Building **backend systems, full-stack applications, data pipelines and AI-powered products**.

Computer Science student at **Universidade Federal de Mato Grosso do Sul (UFMS)** with international academic experience at **Leuphana University Lüneburg, Germany**.

</div>

---

<div align="center">

### 🌐 Connect with me

<a href="https://www.linkedin.com/in/samuel-nahas-23b809281/" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-ff0043?style=for-the-badge&logo=linkedin&logoColor=white">
</a>
<a href="https://github.com/SamuelNahas" target="_blank">
  <img src="https://img.shields.io/badge/GitHub-ff0043?style=for-the-badge&logo=github&logoColor=white">
</a>

</div>

---

<div align="center">

### 💻 Technologies & Tools

<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nextjs/nextjs-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nodejs/nodejs-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/spring/spring-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/fastapi/fastapi-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/postgresql/postgresql-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/redis/redis-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/git/git-original.svg">
<img align="center" height="35" width="45" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg">

<br><br>

![REST APIs](https://img.shields.io/badge/REST_APIs-ff0043?style=flat-square)
![LLM](https://img.shields.io/badge/LLM_Integration-ff0043?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-ff0043?style=flat-square)
![Vector Search](https://img.shields.io/badge/Vector_Search-ff0043?style=flat-square)
![WebSockets](https://img.shields.io/badge/WebSockets-ff0043?style=flat-square)
![CI/CD](https://img.shields.io/badge/CI%2FCD-ff0043?style=flat-square)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-ff0043?style=flat-square&logo=githubactions&logoColor=white)

</div>

---

# 🚀 Featured Projects

## 🌹 Rote Rosen — AI Audience Analytics Platform

Large-scale academic software project developed at **Leuphana University Lüneburg** in collaboration with the German television production **Rote Rosen**.

The goal was to transform large volumes of audience discussion into **structured, explainable and continuously updated insights** using data engineering, natural-language processing and Large Language Models.

Rather than building a standalone sentiment-analysis script, the team designed a complete multi-service system:

```text
Rote Rosen Community Discussions
              ↓
       Automated Crawler
              ↓
          PostgreSQL
              ↓
     FastAPI Analytics API
              ↓
   Statistical + LLM Analysis
              ↓
 React / TypeScript Dashboard
```

### 🕷️ Automated data pipeline

A dedicated crawler collects weekly discussions about the show from the **Wunschliste Rote Rosen forum**.

The ingestion pipeline extracts and enriches:

- posts and replies
- discussion hierarchy
- timestamps and users
- reply counts
- thread structure
- posting activity
- textual characteristics
- character mentions

New information is stored in the central PostgreSQL database and the analytical backend is automatically notified that a new period is available for processing.

### 🧠 AI & analytics backend

The analytical service was built with **Python and FastAPI** and combines deterministic metrics with LLM-powered analysis.

It generates:

- positive, neutral and negative audience sentiment
- contextual explanations for sentiment
- evidence posts supporting classifications
- engagement metrics
- posting frequency
- reply and thread-depth statistics
- recurring discussion topics
- character mention statistics
- audience summaries for individual characters

Character summaries are grounded in actual discussion excerpts rather than generic model-generated descriptions.

### 🔎 Explainable AI

A central architectural goal was **data provenance**.

Analytical results can be connected back to the actual audience posts that contributed to them.

Instead of only reporting:

> "Audience sentiment was negative."

the system can expose the discussions that support the result.

### ⚡ Compute once, cache and reuse

For each analytical period:

1. PostgreSQL is checked for existing results;
2. available analytics are returned immediately;
3. only missing analyses are computed;
4. required LLM calls are performed;
5. results are persisted;
6. future requests reuse the stored analysis.

This reduces unnecessary model execution while keeping historical analytics quickly accessible.

### 👨‍💻 My contribution

I worked heavily on the **backend and analytical architecture**, including development of the first substantial backend prototype and its evolution into the multi-service architecture.

My work included:

- FastAPI REST API development
- sentiment-analysis pipelines
- LLM integration
- engagement analytics
- character analysis
- PostgreSQL persistence
- analytical caching
- weekly processing logic
- API contracts
- webhook-based processing
- Dockerized services

**Stack:** `Python` · `FastAPI` · `PostgreSQL` · `Pandas` · `LLMs` · `React` · `TypeScript` · `Docker`

🔗 [AIProjectRoteRosen](https://github.com/orgs/AIProjectRoteRosen/repositories)

---

## 😂 ComedyHub — Full-Stack Social Media Platform

One of my largest early full-stack projects: a **social network built around comedy content and communities**.

ComedyHub went beyond a basic CRUD application and was designed as a multi-client platform with a web application, mobile application, backend API, asynchronous infrastructure and real-time communication.

```text
       React Web App
             │
 React Native Mobile App
             │
             ▼
      REST API + WebSocket
             │
             ▼
      Java / Spring Boot
        ↙          ↘
 PostgreSQL        Redis
             │
             ▼
 Notifications / Media / External Services
```

### 👥 Social platform

The platform included concepts such as:

- user accounts and profiles
- content publishing
- posts
- comments
- likes and interactions
- content sharing
- notifications
- media handling
- real-time events

### ☕ Backend architecture

The backend was developed primarily using **Java and Spring Boot**, incorporating:

- Spring Boot
- Spring MVC
- Spring Data JPA
- PostgreSQL
- Redis
- Spring Security
- JWT authentication
- REST APIs
- WebSocket communication
- Swagger / OpenAPI
- DTO and service layers
- API versioning
- structured error responses

### 🔐 API & authentication

The API was designed around **JWT bearer authentication** and evolved into a versioned interface capable of serving both web and mobile clients.

The architecture also considered:

- validation
- standardized errors
- authorization
- file uploads
- media handling
- rate limiting
- persistent real-time connections

### ⚡ Real-time infrastructure

In addition to traditional HTTPS REST endpoints, ComedyHub incorporated **WebSockets for real-time events** and Redis for caching and asynchronous communication patterns.

### 🖥️ Multiple clients

**Web:** `React` · `Vite`  
**Mobile:** `React Native`  
**Backend:** `Java` · `Spring Boot`  
**Infrastructure:** `PostgreSQL` · `Redis`

🔗 [ComedyHub API](https://github.com/SamuelNahas/comedyhubApi)  
🔗 [ComedyHub Documentation](https://github.com/lucaserm/my-docs-comedyhub)

**Stack:** `Java` · `Spring Boot` · `Spring Security` · `PostgreSQL` · `Redis` · `React` · `React Native` · `JWT` · `WebSockets` · `OpenAPI`

---

## 📊 [SH Meta Games](https://github.com/SamuelNahas/Limitless-stats)

Competitive **Pokémon TCG metagame analytics platform** built from public tournament data.

The application transforms tournament results into structured competitive analytics, including:

- metagame representation
- tournament performance
- deck rankings
- BO1 and BO3 matchup statistics
- representative decklists
- tournament history
- personal match tracking

```text
Limitless TCG
     ↓
Python Collector
     ↓
Data Processing
     ↓
Versioned Dataset
     ↓
Next.js Application
     ↓
GitHub Pages
```

The project also includes automated collection, scheduled updates, configurable competitive eras, GitHub Actions CI/CD, Supabase authentication and a personal Battle Journal.

**Stack:** `Next.js` · `React` · `TypeScript` · `Python` · `Supabase` · `GitHub Actions`

🌐 [Live Application](https://samuelnahas.github.io/Limitless-stats/)

---

## 🏆 TCG Tournament Check

Full-stack tournament operations platform created to support **Pokémon TCG judges and tournament organizers** during real competitive events.

The platform handles:

- tournament creation
- player and judge accounts
- digital decklist submission
- Pokémon TCG Live imports
- deck validation
- physical deck-check workflows
- tournament occurrences
- penalties
- PDF reports
- backups
- mobile, iPad and desktop interfaces

Deployment is containerized and integrated with a self-hosted **GitHub Actions** runner.

**Stack:** `TypeScript` · `Node.js` · `SQLite` · `Docker` · `Nginx` · `GitHub Actions`

> Private repository — built for real tournament operations.

---

## 🖥️ HVComp

Educational computing project based on the **Hypothetical Computer (HV)** model.

HVComp provides an environment for teaching fundamental concepts of computer architecture and program execution through a simplified hypothetical machine.

The project explores:

- CPU execution
- memory
- machine instructions
- machine language
- program execution
- computer architecture education

It is also connected to academic work involving **Computer Science Education and Design Science Research**.

🌐 [hvcomp.io](https://hvcomp.io)

---

## 🃏 [Pokémon TCG Master Set](https://github.com/SamuelNahas/my-master-set)

Collection-management application combining multiple Pokémon TCG data sources to create a more complete catalog of Brazilian, international and Japanese card releases.

Features include collection tracking, card image resolution, variant filtering, completion statistics, backups and automatically generated visual checklists.

**Stack:** `JavaScript` · `HTML` · `CSS` · `REST APIs` · `GitHub Actions`

---

# 💼 Industry Experience

## ClickTI — Confidential AI / RAG Project

Working on a **private AI-focused software project at ClickTI** centered around a **Retrieval-Augmented Generation (RAG) pipeline** for processing and retrieving information from large document collections.

At a high level, the system follows a pipeline similar to:

```text
Documents
    ↓
Ingestion & Processing
    ↓
Embeddings
    ↓
Vector Search / Retrieval
    ↓
Relevant Context
    ↓
Large Language Model
    ↓
Grounded Response
```

The project combines backend engineering, document processing, semantic retrieval and LLM integration to allow model responses to be grounded in information retrieved from the project's document base.

The system is also being developed with integration into **NVIDIA Spark infrastructure**, exploring accelerated AI workloads and local/high-performance model execution.

My work involves areas such as:

- RAG architecture
- document ingestion pipelines
- backend API development
- vector-based semantic search
- LLM integration
- data persistence
- containerized services
- testing and deployment
- integration with NVIDIA AI infrastructure

Because this is an active commercial project, **client data, internal architecture, business rules, model configuration and implementation details are intentionally not disclosed publicly**.

**Areas:** `RAG` · `LLMs` · `Vector Search` · `Backend Engineering` · `Document Processing` · `NVIDIA AI` · `Docker`

---

# ⚙️ What I Work With

My recent projects have given me practical experience with:

- backend architecture
- REST API design
- relational databases
- vector databases and semantic retrieval
- Retrieval-Augmented Generation
- real-time systems
- authentication and authorization
- automated data pipelines
- web scraping and ingestion
- LLM integration
- AI-assisted analytics
- explainable AI / data provenance
- caching strategies
- Dockerized systems
- CI/CD
- automated testing
- self-hosted infrastructure
- full-stack web development

### Main technologies

`Python` · `Java` · `TypeScript` · `JavaScript`  
`FastAPI` · `Spring Boot` · `Node.js`  
`React` · `Next.js` · `React Native`  
`PostgreSQL` · `Redis` · `SQLite` · `Supabase`  
`Docker` · `Linux` · `GitHub Actions`

---

<div align="center">

## 🎓 Education

### Universidade Federal de Mato Grosso do Sul 🇧🇷

**B.Sc. Computer Science**

<br>

### Leuphana University Lüneburg 🇩🇪

**International Exchange Studies**

Worked in multidisciplinary and international teams on software engineering and AI projects.

---

### Currently interested in

**Backend Engineering · Software Architecture · RAG · AI Applications · Data Engineering · Full-Stack Development**

<br>

### 📫 Let's build something.

<a href="https://www.linkedin.com/in/samuel-nahas-23b809281/">
  <img src="https://img.shields.io/badge/Contact_me_on_LinkedIn-ff0043?style=for-the-badge&logo=linkedin&logoColor=white">
</a>

</div>
