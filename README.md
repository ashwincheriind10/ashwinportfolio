# 👋 Welcome to My Portfolio

Hi, I'm Ashwin

I'm a Grade 11 student passionate about Mathematics, Physics, Robotics, Artificial Intelligence, and software development. I enjoy building innovative products that solve real-world problems and create meaningful impact. Beyond technology, 
I am passionate about social service, philanthropy, and using innovation to improve lives.

This repository showcases the platforms and projects I've built and continue to develop. While the source code for most projects is private, this portfolio provides an overview of each product, its purpose, and the technologies behind it.

I'm constantly learning, experimenting with new technologies, and exploring the future of AI, robotics, and intelligent systems.
---

# Featured Projects

## CheriMathLab
What CheriMathLab actually is

CheriMathLab is a unified STEM learning ecosystem where students learn, practise, compete, get guidance, and keep improving, all in one place. Instead of juggling separate tools for lessons, practice, help, classes, and assessments, everything works together as one connected experience.

A student can learn from structured content, attempt quizzes and full length mock exams, solve daily challenges that build steady habits, enter academic competitions, ask an AI tutor for help the moment they get stuck, join live classes, connect with tutors and mentors, and receive personalised guidance, all in the same platform.

The adults supporting that student stay in the loop and step in when it matters, each seeing a different view of the same student.


**Highlights**
- AI-powered adaptive learning
- AI study coach and chat (RAG + knowledge base)
- ML-based performance prediction and recommendations
- Weekly quizzes and assignments
- Olympiad preparation
- AP preparation and AP mock exams
- SAT preparation
- Practice mode and Problem of the Day
- Learning paths and mock exams
- Mistake Journal
- Question bank and subject sets
- Doubt solving
- Multiplayer quiz battles
- Competitions, scholarships, and success stories
- Student progress analytics and intelligent insights (weak areas, exam readiness, time analysis, XP history)
- Higher-Ed consultancy (college application CRM)
- Guidance, counselling, and expert sessions
- 1:1 tutoring with hours and payments
- Live classes and webinars
- Chat, group chat, forum, and study groups
- Notifications and push notifications
- Attendance, leave, fees, and payroll (school management)
- Video lessons, content store, and document vault
- Teacher, parent, student, and school-admin dashboards
- Multi-school, multi-language (with RTL), and per-school feature gating

**Technology**
- Frontend: Next.js, React, TypeScript, Tailwind CSS
- Backend: ASP.NET Core (C#) microservices
- Machine learning: Python, XGBoost, prediction and recommendation models
- Data: MySQL, Redis, vector database (RAG)
- Realtime: SignalR (WebSockets)
- Background jobs: Hangfire
- Security: JWT with httpOnly cookies, 2FA and OTP, Google sign-in, DOMPurify, CSP and security headers
- Payments: Razorpay
- Math rendering: KaTeX
- Delivery: PWA with service worker and push notifications
- Infrastructure: Docker, Linux, Vercel, self-hosted Windows (IIS + NSSM), Caddy, zero-downtime deploys

**Status**
🟢 Live in production, active development(http://cherimathlab.com)

---
## CheriMind
A Retrieval-Augmented Generation (RAG) platform that gives accurate, cited, context-aware answers from an organization's private documents and live data - deployable fully on your own infrastructure, so data never leaves the building.

**Highlights**
- Document ingestion and processing (PDF, Word, text, URLs, structured data)
- Semantic search using embeddings, with cross-encoder reranking
- Search-only mode (no AI, no cost) or AI-written, source-cited answers
- Live data sources fused with document knowledge at query time
- Personalized, context-aware responses per user
- Rules engine: field redaction and required-source enforcement
- Multi-tenant, multi-project isolation with role-based access
- Cost intelligence: per-question cost estimate from history and an ML forecast
- Flexible key handling: managed (encrypted at rest), bring-your-own-key, vault reference, or return-the-prompt
- Glass-box audit log, answer feedback, and a coverage-gaps report
- Fully self-hostable, with offline signed licensing for on-prem

**Technology**
- ASP.NET Core (.NET 10)
- Python FastAPI sidecar (embeddings, reranking, cost ML)
- PostgreSQL + pgvector (HNSW)
- sentence-transformers (all-MiniLM-L6-v2, 384-dim) + cross-encoder reranker
- Ollama / Azure OpenAI / OpenAI (pluggable LLMs)
- React 19 + Vite + TypeScript (landing site)
- Docker / Docker Compose (on-prem installer)
- REST APIs

**Status**
🟢 Production(https://cherimind.duckdns.org/)

---

## CheriHire
AI recruitment platform: reads every resume, flags fakes, predicts fit,
and runs the whole hire, for employers, hiring companies, and job seekers.

Highlights
- Authenticity scoring (fake-resume detection) with reasons
- Explainable fit prediction + shortlist odds
- Two-sided: recruiter dashboard + job-seeker careers portal
- Full hire loop: interviews, scorecards, offers, referrals, verification
- Resume ingestion: upload, shared folder, email inbox
- Analytics, forecasting, and a self-learning ranking model
- Multi-tenant with per-org isolation and plans

Technology
- .NET 10 (ASP.NET Core), MySQL 8
- Next.js
- Python (FastAPI) + XGBoost ML service
- Ollama + Azure OpenAI for resume parsing
- Linux, systemd, Caddy; ClamAV upload scanning

Status
🟢 Live MVP (https://cherihire.com)

---

## ♻️ Recycler Intelligence
**Buyer-intelligence platform for India's recycling ecosystem: a source-tracked, verified recycler/buyer directory, a weekly recyclable-commodity price tracker, upstream waste-intake tracking, and buyer-to-lot matching, with a login-protected operations console.**

**Highlights**
- Config-driven ingestion pipeline (add a new source in YAML, no code)
- Five source connectors: file, http, api, db, pdf
- Dedicated collectors: internal list, CPCB EPR, SPCB (Telangana + Karnataka), public directories, GeM, outreach, generators, collections, prices
- Cleaning and normalization: company names, phones, emails, cities, materials (PET/HDPE/PAPER/etc.)
- Weighted fuzzy deduplication engine (GST/EPR/phone/name/email/website/city) with review queue
- Cross-source, load-time and DB-wide merge with survivor selection
- Idempotent loader with full provenance: raw JSON audit copy and process log per run
- 6-level verification ladder and 0-100 confidence scoring
- Verification queue and outreach worklist generator
- Buyer Fit Score: ranks buyers per lot on material, distance, price, verification, and past response
- Lot creation and buyer-to-lot matching
- Weekly price tracker with trend and week-over-week anomaly detection
- Buyer-quote-to-price feed (a price quoted on a call becomes a price observation)
- Streamlit operations console: 17 screens, business dashboard, full-pipeline runner, generic CRUD
- Authentication: bcrypt-hashed passwords and security-answer password reset
- Soft-delete-and-restore everywhere (nothing hard-deleted)
- PostgreSQL schema: 19 tables, 8 reporting views, JSONB source tracking, performance index pack
- CLI runner with 20 pipeline steps and dry-run mode
- n8n weekly price-refresh automation with email alerts
- ~89 tests (unit and live-Postgres integration)
- Deployment guides (Linux/Windows/Streamlit), ops runbooks, per-file tech specs, Docker Compose

**Technology**
- Python (ETL pipeline: pandas, SQLAlchemy, RapidFuzz, pdfplumber, bcrypt, pydantic)
- PostgreSQL (JSONB source tracking, soft delete, reporting views)
- Streamlit (operations console)
- n8n (scheduled weekly refresh)

**Status**
🟢 v1.0.0 handover (Phase 2 planned: PostGIS distance, WhatsApp quote capture, OCR, web dashboard + API)

---
# Contact

Feel free to connect with me.

Personal Website - https://ashwincheripally.com/

LinkedIn  -https://www.linkedin.com/in/ashwin-cheripally-054214206/

LinkedIn Company Page- https://www.linkedin.com/company/113554217/admin/dashboard/


# Product Websites
https://cherimathlab.com/
https://cherihire.com/
https://cherimind.duckdns.org/
https://cherifoundation.com/
