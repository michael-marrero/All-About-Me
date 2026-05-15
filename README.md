# Michael Marrero

**Software Engineer** — Boston, MA  
B.A. Computer Science + Mathematics Minor @ UMass Boston (Expected May 2026)  
GPA: 3.30 · Harvard Business School Foundry Accelerator (June 2026 cohort)

📧 marreroii.michael@gmail.com · 📞 +1 (339) 205-4515  
🔗 [LinkedIn](https://www.linkedin.com/in/michael-marreroii/) · 🐙 [GitHub](https://github.com/michael-marrero)

---

## About

I build distributed systems and full-stack products from zero to production. I care about correctness, reliability, and systems that are actually operable, explicit contracts, idempotent operations, structured observability, and predictable failure modes. Currently shipping at **Queue** (my own startup, accepted into HBS Foundry) and **Calico Care** (healthtech AI).

## Currently Reading

- *Why Machines Learn* — Anil Ananthaswamy
- *Zero to One* — Peter Thiel
- *In Love with the World* — Yongey Mingyur Rinpoche

---

## Technical Skills

| Category | Technologies |
|---|---|
| **Languages** | Python, TypeScript/JavaScript, Go, SQL, C++ |
| **Frontend** | Next.js, React, Vite, TailwindCSS, HTML |
| **Backend** | Node.js, Django/Flask, PostgreSQL, Redis, CI/CD |
| **ML / AI** | TensorFlow, PyTorch, Scikit-Learn |
| **Infrastructure** | Git, Docker, Kubernetes, AWS, GCP, Cloudflare |

---

## Work Experience

### Queue — Founder & Lead Developer
*Boston, MA · January 2026 – Present*

Built a **distributed queueing platform** allowing users to join, monitor, and manage venue waitlists digitally.

- Sole lead developer: designed and shipped venue-facing apps, user-facing apps, backend API, a deterministic queue engine for fair real-time ETAs, and internal admin tooling
- Architected for consistency, reliability, and low-latency updates across multiple client surfaces
- **Accepted into [Harvard Business School's Foundry]([https://www.hbs.edu/mba/student-life/activities-and-clubs/entrepreneurship/Pages/foundry.aspx](https://www.hbs.edu/foundry)) accelerator (June 2026 cohort)**

---

### Calico Care — Software Engineer
*Boston, MA · December 2025 – Present*

Healthtech startup building AI-powered digital triage with voice agents.

- Improved production AI voice agent reliability via structured outputs, schema validation, and idempotent webhook/tool execution
- Implemented runtime BAA-gating to prevent non-compliant paths from processing PHI; embedded HIPAA-aware controls into the request pipeline
- Owned the end-to-end agent delivery pipeline (provisioning, orchestration, observability) — supporting **200+ patient-facing calls/month**

---

### Venture Development Center @ UMass Boston — Apprentice
*Boston, MA · June 2025 – September 2025*

- Conducted startup diligence and market analysis (TAM, competition, differentiation, execution risks)
- Supported founders through fundraising and pitch development
- Worked under executive leadership at an innovation hub supporting **$2B+ in venture investment** and **$1.5B+ in exits**

---

## Projects I've Done or In Progress

### [Marlowe](https://github.com/ClarkOhlenbusch/Marlowe) — Real-Time Scam Call Monitor
*Next.js · React · TypeScript · Twilio · Groq LLM · Supabase · Vercel — Tufts JumboHack 2026*

Full-stack app that monitors live calls and streams real-time coaching to the UI.

- Engineered end-to-end streaming pipeline: Twilio webhooks → chunk ingestion → LLM analysis → UI updates; reduced transcript-to-UI latency to **~1 second**
- Implemented server-side call initiation via Next.js Route Handlers with Twilio webhook signature validation
- Validated against consented adversarial voice-clone scenarios simulating modern impersonation attacks

---

### [DocIntel](https://github.com/michael-marrero/Docintel) — Production-Shaped RAG over SEC 10-K Filings

*Python · FAISS · BM25 · Cross-Encoder Reranking · Docker · GitHub Actions*

RAG pipeline focused on retrieval quality, grounded answers, and operational rigor.

- Hybrid retrieval combining BM25 + dense FAISS via Reciprocal Rank Fusion, followed by cross-encoder reranking
- Structured citation outputs with refusal logic for low-confidence or out-of-corpus queries
- Retrieval and answer quality evaluation runs in CI — regressions caught before merge
- Reproducible local environment via Docker Compose; secret scanning (gitleaks) and pre-commit hooks enforced repo-wide

---

### [Prompt Optimizer](https://github.com/michael-marrero/Prompt-Optimizer) — Task-Aware LLM Routing

*Python · scikit-learn · TF-IDF · LLMRouterBench · OpenRouter*

Prompt routing system that classifies queries by task type and recommends the best-performing model per task.

- Task-type classifier across 10 categories (coding, math, reasoning, factual, agentic, medical, writing, etc.) using TF-IDF (word + char) + handcrafted prompt features → logistic regression with balanced class weights
- Two-stage routing: classifier output (predicted type + confidence) feeds a downstream model router that selects an exact model from the LLMRouterBench top-model set
- Experimental tier router (cheap / medium / strong) achieving **78% accuracy, 0.75 macro F1** as a coarse-grained fallback
- End-to-end demo pipeline that maps benchmark labels to live OpenRouter routes via a verified model mapping

---
  
## Leadership

### Rising Entrepreneurs Association — Venture Lead & Relations
*UMass Boston · Fall 2025 – Present*

Designed and led a venture mentorship program supporting early-stage founders with product strategy and execution planning. Collaborated with investors, mentors, and student founders to strengthen venture pipelines. I've gotten the chance to interview some really successful entrepreneurs and industry leaders, which has been an incredible experience. 

---

## What I Look For in an Engineering Role

- Distributed systems, backend infrastructure, or full-stack product work
- Teams that care about reliability, contracts, and operational quality
- Environments where I can own features end-to-end and move fast without cutting corners
- Working with interesting technologies, pushing my knowledge further, challenging my engineering ceiling every single day
