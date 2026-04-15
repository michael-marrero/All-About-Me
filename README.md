# Michael Marrero

**Software Engineer** — Boston, MA  
B.A. Computer Science + Mathematics Minor @ UMass Boston (Expected May 2026)  
GPA: 3.30 · Harvard Business School Foundry Accelerator (June 2026 cohort)

📧 marreroii.michael@gmail.com · 📞 +1 (339) 205-4515  
🔗 [LinkedIn](https://www.linkedin.com/in/michael-marreroii/) · 🐙 [GitHub](https://github.com/michael-marrero)

---

## About

I build distributed systems and full-stack products from zero to production. I care about correctness, reliability, and systems that are actually operable — explicit contracts, idempotent operations, structured observability, and predictable failure modes. Currently shipping at **Queue** (my own startup, accepted into HBS Foundry) and **Calico Care** (healthtech AI).

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

## Projects

### [Marlowe](https://github.com/ClarkOhlenbusch/Marlowe) — Real-Time Scam Call Monitor
*Next.js · React · TypeScript · Twilio · Groq LLM · Supabase · Vercel — Tufts JumboHack 2026*

Full-stack app that monitors live calls and streams real-time coaching to the UI.

- Engineered end-to-end streaming pipeline: Twilio webhooks → chunk ingestion → LLM analysis → UI updates; reduced transcript-to-UI latency to **~1 second**
- Implemented server-side call initiation via Next.js Route Handlers with Twilio webhook signature validation
- Validated against consented adversarial voice-clone scenarios simulating modern impersonation attacks

---

### [Frontline Route](https://github.com/michael-marrero) — EMS-to-ED Routing System
*Go · JavaScript · PostgreSQL · DragonflyDB (Redis) · HTMX · Docker · HERE APIs — Verizon Frontline Competition 2026*

Real-time routing and capacity-matching system for EMS-to-hospital transport decisions.

- Built concurrent Go backend serving routing decisions using cost-based optimization over live telemetry and historical delay data
- Modeled transport lifecycle as a finite-state machine with enforced invariants and idempotent transitions
- Designed REST + WebSocket interfaces for real-time facility capacity updates with documented failure modes
- Automated environment provisioning via Docker Compose for production-parity local development

---

### [AccessLens](https://github.com/michael-marrero/AccessLens) — Identity Access Risk Triage *(WIP)*
*TypeScript · Next.js · PostgreSQL*

Production-style MVP for triaging identity/access risk and assisting with policy decisions.

- Risk signal triage with human-in-the-loop workflows
- Policy assistance with audit-friendly decision trails
- Role-based access + org/workspace model

---

## Leadership

### Rising Entrepreneurs Association — Venture Lead & Relations
*UMass Boston · Fall 2025 – Present*

Designed and led a venture mentorship program supporting early-stage founders with product strategy and execution planning. Collaborated with investors, mentors, and student founders to strengthen venture pipelines.

---

### Kappa Sigma — Chapter President
*UMass Boston · March 2023 – Present*

Led a full chapter revitalization in Spring 2024, driving significant increases in member engagement. Organized philanthropy initiatives generating **$10,000+ in each of 2024 and 2025**.

---

## What I Look For in an Engineering Role

- Distributed systems, backend infrastructure, or full-stack product work
- Teams that care about reliability, contracts, and operational quality
- Environments where I can own features end-to-end and move fast without cutting corners

---

## Contact

- 📧 [marreroii.michael@gmail.com](mailto:marreroii.michael@gmail.com)
- 💼 [linkedin.com/in/michael-marreroii](https://www.linkedin.com/in/michael-marreroii/)
- 💻 [github.com/michael-marrero](https://github.com/michael-marrero)
