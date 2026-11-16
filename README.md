# Michael Marrero

**AI Engineer, Evaluations Lead @ Confido Health** · New York, NY  
B.A. Computer Science + Mathematics Minor @ UMass Boston (Graduated May 2026)  
Harvard Business School Foundry Accelerator (June 2026 cohort)

📧 marreroii.michael@gmail.com · 📞 +1 (339) 205-4515  
🔗 [LinkedIn](https://www.linkedin.com/in/michael-marreroii/) · 🐙 [GitHub](https://github.com/michael-marrero)

---

## About

I build production AI systems and full-stack products from zero to live. Right now that means voice AI agents and the evaluation infrastructure that keeps them honest. I care about correctness, reliability, and systems that are actually operable: explicit contracts, idempotent operations, structured observability, automated evals, and predictable failure modes. Currently leading evaluations at **Confido Health** (Series A health-tech, voice AI) and building **Queue** (my own startup, accepted into HBS Foundry).

## Currently Reading

- *Why Machines Learn* by Anil Ananthaswamy
- *Zero to One* by Peter Thiel
- *In Love with the World* by Yongey Mingyur Rinpoche

---

## Technical Skills

| Category | Technologies |
|---|---|
| **Voice & AI** | LLM orchestration (OpenAI, Anthropic, Vapi), voice-agent pipelines, Twilio, RAG architectures, prompt engineering, structured outputs & schema validation, automated evals & LLM-as-judge, agentic patterns |
| **Languages** | JavaScript/TypeScript, Python, SQL, Go, C++ |
| **Backend & Infra** | Node.js, FastAPI, Flask, REST APIs, webhooks, Redis, PostgreSQL, Docker |
| **Cloud & Platforms** | AWS, GCP, Vercel, Supabase, Twilio |
| **Data & ML** | Pandas, NumPy, PyTorch, scikit-learn, Hugging Face, FAISS, statistical analysis |

---

## Work Experience

### Confido Health · AI Engineer, Evaluations Lead
*New York, NY · August 2026 to Present*

Series A health-tech building voice AI agents and automations.

- Lead evaluations company-wide: built a fully autonomous evals pipeline that scores every call made by or to our AI agents, replacing manual call review with continuous, automated quality signals
- Co-built an internal recursive self-improvement system: fully autonomous agents that evaluate and optimize our production agents and deployments, with the evals pipeline serving as its evaluation half
- Redesigned agent architecture company-wide, standardizing how voice agents are structured, prompted, and orchestrated across customer deployments
- Forward deployed engineer on select accounts, taking clients from onboarding to live by configuring, testing, and launching their agents in production
- Work directly with the product team to ship new features and build internal tooling across engineering and operations

---

### Calico Care · Software Engineer, AI / Voice Agents
*Boston, MA · December 2025 to May 2026*

Voice AI for a regulated health-tech setting.

- Shipped and hardened patient-facing AI voice agents in production, improving reliability by enforcing structured outputs, schema validation, and idempotent tool/webhook execution to cut downstream errors
- Operated compliance-aware RAG pipelines over clinical protocols and provider knowledge bases via Vapi, with prompt design and guardrails that prevent agents from issuing medical advice
- Embedded HIPAA controls directly in the request pipeline: implemented runtime BAA-gating to block non-compliant vendor and service paths from processing PHI
- Built and maintained observability dashboards and call-review tooling for an agent stack handling **~200 patient calls/month**, turning live production signals into prompt and retrieval improvements

---

### Queue · Founder & Lead Developer
*Boston, MA · August 2025 to Present*

Distributed, real-time waitlist platform letting users join, monitor, and manage venue waitlists digitally.

- Designed and shipped the platform end to end (consumer, venue, API, and admin surfaces); deployed live across **10 Greater Boston venues** and supported them in production
- Built a deterministic queue engine and backend API for fair ordering, real-time ETA updates, and low-latency synchronization across clients
- Worked directly with non-technical venue operators to configure deployments and turn live operational data into dashboards they could act on, owning the full loop from setup to support
- **Accepted into [Harvard Business School's Foundry](https://www.hbs.edu/foundry) accelerator (June 2026 cohort)**

---

### Independent Technical Advisor · Early-Stage AI/Tech Startups
*Independent and via UMass Boston Venture Development Center · 2024 to 2025*

- Embedded with 3 to 5 early-stage startups to advise on architecture, infrastructure, and roadmap
- Translated complex technical products into clear narratives for non-technical and investor stakeholders
- Through the VDC, conducted startup diligence and market analysis (TAM, competition, differentiation, execution risks) at an innovation hub supporting **$2B+ in venture investment** and **$1.5B+ in exits**

---

## Projects I've Done or In Progress

### [DocIntel](https://github.com/michael-marrero/Docintel) · End-to-End RAG over Heterogeneous Documents
*Python · FAISS · BM25 · Cross-Encoder Reranking · Tesseract OCR · FastAPI · Docker · GitHub Actions · April 2026 to Present*

RAG system focused on retrieval quality, grounded answers, and operational rigor.

- Ingests heterogeneous documents (native PDFs, scanned images, structured exports) with semantic chunking and a Tesseract OCR fallback for scanned content
- Hybrid retrieval combining BM25 + dense FAISS via Reciprocal Rank Fusion, followed by cross-encoder reranking and LLM answer synthesis
- Structured citation outputs with refusal logic for low-confidence or out-of-corpus queries
- Evaluation harness (retrieval@k, answer faithfulness across 25+ Q&A pairs) compares chunking, embeddings, and prompts; runs in CI so regressions are caught before merge
- Served via FastAPI; reproducible environment via Docker Compose, with secret scanning (gitleaks) and pre-commit hooks enforced repo-wide

---

### [Prompt Router](https://github.com/michael-marrero/Prompt-Optimizer) · Task-Aware LLM Routing
*Python · scikit-learn · TF-IDF · LLMRouterBench · OpenRouter · AI Course Project (CS470/670), March to May 2026*

Two-stage routing pipeline that classifies a query by task type and routes it to the right LLM.

- Task-type classifier across 10 categories (coding, math, reasoning, factual, agentic, medical, writing, etc.) using TF-IDF (word + char) + handcrafted prompt features into logistic regression with balanced class weights
- Classifier output (predicted type + confidence) feeds a downstream router that selects an exact model from the LLMRouterBench top-model set
- Tier router (cheap / medium / strong) achieving **78% accuracy, 0.75 macro F1**, plus a cost-aware variant that selects the cheapest model within a tolerance band
- End-to-end demo pipeline that maps benchmark labels to live OpenRouter routes via a verified model mapping

---

### [Marlowe](https://github.com/ClarkOhlenbusch/Marlowe) · Real-Time Scam Call Monitor
*Next.js · React · TypeScript · Twilio · Groq LLM · Supabase · Vercel · Tufts JumboHack 2026*

Full-stack app that monitors live calls and streams real-time coaching to the UI.

- Engineered end-to-end streaming pipeline: Twilio webhooks → chunk ingestion → LLM analysis → UI updates; reduced transcript-to-UI latency to **~1 second**
- Implemented server-side call initiation via Next.js Route Handlers with Twilio webhook signature validation
- Validated against consented adversarial voice-clone scenarios simulating modern impersonation attacks

---

## Leadership

### Rising Entrepreneurs Association · Founder, Venture Lead & Relations
*UMass Boston · Fall 2025 to May 2026*

Designed and led a venture mentorship program supporting early-stage founders with product strategy and execution planning. Collaborated with investors, mentors, and student founders to strengthen venture pipelines. I've gotten the chance to interview some really successful entrepreneurs and industry leaders, which has been an incredible experience.

---

## Education

### University of Massachusetts Boston
*B.A. Computer Science, Minor in Mathematics · May 2026*

Relevant coursework: Artificial Intelligence, Computational Statistics, Database Management, Software Engineering, Advanced Algorithms, Operating Systems, Theory of Computation

---

## What I Look For in an Engineering Role

- Production AI systems, evals, distributed systems, backend infrastructure, or full-stack product work
- Teams that care about reliability, contracts, and operational quality
- Environments where I can own features end-to-end and move fast without cutting corners
- Working with interesting technologies, pushing my knowledge further, challenging my engineering ceiling every single day
- Startups!!
