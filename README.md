# Welcome to My Portfolio

# Hi, I'm Ashwin 

**Ashwin Cheripally** - Grade 11 student · AI / ML Full-Stack Engineer & Founder

I'm a Grade 11 student passionate about Mathematics, Physics, Robotics, Artificial Intelligence, and software development. I enjoy building innovative products that solve real-world problems and create meaningful impact. Beyond technology, I am passionate about social service, philanthropy, and using innovation to improve lives.

This repository showcases the platforms and projects I've built and continue to develop. While the source code for most projects is private, this portfolio provides an overview of each product, its purpose, and the technologies behind it.

---

## What I build

Production AI systems: Retrieval-Augmented Generation (RAG), machine-learning prediction models, and secure multi-tenant SaaS. I ship end-to-end Next.js / React frontends, ASP.NET Core (.NET 10) & Python (FastAPI) backends, vector search, and self-hostable, security-hardened deployments.

**Live products:** [CheriMathLab](https://cherimathlab.com/) · [CheriMind](https://cherimind.duckdns.org/) · [CheriHire](https://cherihire.com/) 

**Core stack:** RAG ·LLMs (Ollama / Azure OpenAI / OpenAI / DeepSeek) · pgvector · sentence-transformers · XGBoost · ASP.NET Core · Python · Next.js · PostgreSQL · MySQL · Redis · Docker · SignalR · PWA
---

# Featured Projects

## CheriMathLab

CheriMathLab is a unified, AI-powered STEM learning platform (LMS + adaptive learning + RAG study coach) for Olympiad, SAT, and AP prep, built with Next.js, ASP.NET Core microservices, and machine-learning performance prediction.

**What CheriMathLab actually is**

CheriMathLab is a unified STEM learning ecosystem where students learn, practise, compete, get guidance, and keep improving, all in one place. Instead of juggling separate tools for lessons, practice, help, classes, and assessments, everything works together as oneconnected experience.

A student can learn from structured content, attempt quizzes and full-length mock exams, solve daily challenges that build steady habits, enter academic competitions, ask an AItutor for help the moment they get stuck, join live classes, connect with tutors and mentors, and receive personalised guidance, all in the same platform.

The adults supporting that student stay in the loop and step in when it matters, each seeing a different view of the same student.


### Highlights

**AI & Machine Learning**
- Student AI Agent: an autonomous, agentic assistant that guides each student end to end
- AI-powered adaptive learning
- AI study coach and chat (RAG + knowledge base)
- ML-based performance prediction and recommendations
- Student progress analytics and intelligent insights (weak areas, exam readiness, time analysis, XP history)
- AI doubt solving

**Learning & practice**
- Structured content, video lessons, and learning paths
- Weekly quizzes and assignments
- Full-length mock exams, Practice mode, and Problem of the Day
- Olympiad preparation, SAT preparation, AP preparation and AP mock exams
- Question bank and subject sets
- Mistake Journal

**Compete & engage**
- Multiplayer quiz battles
- Competitions, scholarships, and success stories

**Guidance & community**
- 1:1 tutoring with hours and payments
- Live classes and webinars
- Guidance, counselling, and expert sessions
- Higher-Ed consultancy (college application CRM)
- Chat, group chat, forum, and study groups

**Platform, security & administration**
- Teacher, parent, student, and school-admin dashboards
- School management: attendance, leave, fees, and payroll
- Content store, document vault, and notifications (with push)
- Multi-school, multi-language (with RTL), and per-school feature gating
- Security: JWT with httpOnly cookies, 2FA and OTP, Google Sign-In, DOMPurify, CSP and security headers

### Technology

- **Frontend:** Next.js, React, TypeScript, Tailwind CSS
- **Backend:** ASP.NET Core (C#) microservices
- **Machine learning:** Python, XGBoost, prediction and recommendation models
- **Data:** MySQL, Redis, vector database (RAG)
- **Realtime:** SignalR (WebSockets)
- **Background jobs:** Hangfire
- **Security:** JWT with httpOnly cookies, 2FA and OTP, Google Sign-In, DOMPurify, CSP and security headers
- **Payments:** Razorpay
- **Math rendering:** KaTeX
- **Delivery:** PWA with service worker and push notifications
- **Infrastructure:** Docker, Linux, Vercel, self-hosted Windows (IIS + NSSM), Caddy, zero-downtime deploys


**Status**
🟢 Live in production, active development(http://cherimathlab.com)

---
## CheriMind

CheriMind is a self-hostable Retrieval-Augmented Generation (RAG) platform that gives accurate, cited, context-aware answers from an organization's private documents and live data. It deploys fully on your own infrastructure, so data never leaves the building.

### Highlights

**AI & retrieval (RAG)**
- Document ingestion and processing (PDF, Word, text, URLs, structured data)
- Semantic search using embeddings, with cross-encoder reranking
- Search-only mode (no AI, no cost) or AI-written, source-cited answers
- Live data sources fused with document knowledge at query time
- Personalized, context-aware responses per user

**Machine learning & cost intelligence**
- Embedding-based semantic search with cross-encoder reranking for precision
- Cost intelligence: per-question cost estimate from history, plus an ML forecast

**Security, privacy & governance**
- Fully self-hostable, with offline signed licensing for on-prem (data never leaves the building)
- Rules engine: field redaction and required-source enforcement
- Multi-tenant, multi-project isolation with role-based access
- Flexible key handling: managed (encrypted at rest), bring-your-own-key, vault reference, or return-the-prompt
- Glass-box audit log, answer feedback, and a coverage-gaps report

### Technology

- **Backend:** ASP.NET Core (.NET 10)
- **AI sidecar:** Python FastAPI (embeddings, reranking, cost ML)
- **Vector data:** PostgreSQL + pgvector (HNSW)
- **Models:** sentence-transformers (all-MiniLM-L6-v2, 384-dim) + cross-encoder reranker
- **LLMs (pluggable):** Ollama / Azure OpenAI / OpenAI
- **Frontend:** React 19 + Vite + TypeScript (landing site)
- **Delivery:** Docker / Docker Compose (on-prem installer)
- **Interface:** REST APIs

**Status**
🟢 Production(https://cherimind.duckdns.org/)

---
## CheriHire

CheriHire is an AI recruitment platform that reads every resume, flags fakes, predicts candidate fit, and runs the entire hiring loop, for employers, hiring companies, and job seekers. Built with .NET 10, Next.js, and a Python XGBoost ML service.

### Highlights

**AI & machine learning**
- Authenticity scoring (fake resume detection) with explainable reasons
- Explainable fit prediction and shortlist odds
- Analytics, forecasting, and a self-learning ranking model
- LLM-based resume parsing (Ollama + Azure OpenAI)

**Hiring workflow (two-sided)**
- Recruiter dashboard and job seeker careers portal
- Full hire loop: interviews, scorecards, offers, referrals, verification
- Resume ingestion: upload, shared folder, email inbox

**Security & multi-tenancy**
- Multi-tenant with per org isolation and plans
- ClamAV malware scanning on every upload
- Hardened Linux deployment (systemd, Caddy TLS)

### Technology

- **Backend:** .NET 10 (ASP.NET Core), MySQL 8
- **Frontend:** Next.js
- **ML service:** Python (FastAPI) + XGBoost
- **LLMs:** Ollama + Azure OpenAI (resume parsing)
- **Infrastructure & security:** Linux, systemd, Caddy, ClamAV upload scanning

Status
🟢 In Development (https://cherihire.com)

---

## Recycler Intelligence

Recycler Intelligence is a source-tracked buyer-intelligence platform for India's recycling ecosystem: a verified recycler/buyer directory, a weekly recyclable-commodity price tracker, upstream waste-intake tracking, and buyer-to-lot matching, powered by a config-driven Python ETL pipeline with full provenance and a login-protected operations console.

### Highlights

**Data pipeline & ingestion**
- Config-driven ingestion pipeline (add a new source in YAML, no code)
- Five source connectors: file, http, api, db, pdf
- Dedicated collectors: internal list, CPCB EPR, SPCB (Telangana + Karnataka), public directories, GeM, outreach, generators, collections, prices
- Cleaning and normalization: company names, phones, emails, cities, materials (PET/HDPE/PAPER/etc.)
- CLI runner with 20 pipeline steps and dry-run mode
- n8n weekly price-refresh automation with email alerts

**Matching & intelligence (ML / analytics)**
- Weighted fuzzy deduplication engine (GST/EPR/phone/name/email/website/city) with review queue
- Cross-source, load-time and DB-wide merge with survivor selection
- 6-level verification ladder and 0 to 100 confidence scoring
- Buyer Fit Score: ranks buyers per lot on material, distance, price, verification, and past response
- Lot creation and buyer-to-lot matching
- Weekly price tracker with trend and week-over-week anomaly detection
- Buyer-quote-to-price feed (a price quoted on a call becomes a price observation)
- Verification queue and outreach worklist generator

**Data integrity & security**
- Idempotent loader with full provenance: raw JSON audit copy and process log per run
- Soft-delete-and-restore everywhere (nothing hard-deleted)
- Authentication: bcrypt-hashed passwords and security-answer password reset
- PostgreSQL schema: 19 tables, 8 reporting views, JSONB source tracking, performance index pack

**Operations & delivery**
- Streamlit operations console: 17 screens, business dashboard, full-pipeline runner, generic CRUD
- ~89 tests (unit and live-Postgres integration)
- Deployment guides (Linux/Windows/Streamlit), ops runbooks, per-file tech specs, Docker Compose

### Technology

- **ETL pipeline:** Python (pandas, SQLAlchemy, RapidFuzz, pdfplumber, bcrypt, pydantic)
- **Database:** PostgreSQL (JSONB source tracking, soft delete, reporting views)
- **Operations console:** Streamlit
- **Automation:** n8n (scheduled weekly refresh)

**Status**
🟢 v1.0.0 handover (Phase 2 planned: PostGIS distance, WhatsApp quote capture, OCR, web dashboard + API)

---
# Contact

Feel free to connect with me.

Personal Website - https://ashwincheripally.com/

LinkedIn  -https://www.linkedin.com/in/ashwin-cheripally-054214206/

LinkedIn Company Page- https://www.linkedin.com/company/113554217/admin/dashboard/

Foundation Website - https://cherifoundation.com/


