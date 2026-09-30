# Hamid Khan

**Full-Stack Developer & AI Engineer — ERP & Business Systems**

Lahore, Pakistan · hamidkhan069731@gmail.com · 0348 6311899 · [linkedin.com/in/hamid-khan-dev07](https://www.linkedin.com/in/hamid-khan-dev07) · [github.com/hamidkhan069731-blip](https://github.com/hamidkhan069731-blip)

---

## Summary

Full-stack developer and AI engineer specialising in **business/ERP systems** and **practical AI integration**. I build complete products end to end — database schema, REST API, authentication and permissions, frontend, and desktop packaging — with a consistent rule: no fake functionality. If a feature exists, it is wired to a real implementation and real data.

Recent work spans four production-architected systems: an AI voice receptionist that books real appointments, a Windows desktop AI assistant with a governed tool-permission engine, a multi-role law firm ERP, and a university ERP with student/faculty/admin portals.

---

## Technical Skills

- **Backend:** Node.js, Express, Python, FastAPI, REST API design, WebSockets
- **Frontend:** JavaScript (ES6+), HTML5, CSS3, responsive UI
- **Databases:** PostgreSQL, SQLite — schema design, migrations, seeded fixtures, parameterised query hygiene
- **AI Engineering:** Anthropic SDK, tool-calling / agent loops, OpenAI-compatible providers, system prompt & tool-schema design, graceful degradation without keys
- **Auth & Security:** JWT, bcrypt, role-based access control, zod input validation, rate limiting, helmet/CSP, SQL-injection prevention, row-level ownership enforced in SQL
- **Desktop:** Electron packaging (Windows / macOS / Linux)
- **Tooling:** Git & GitHub, npm, pip, Jest, environment & configuration management

---

## Projects

### AI Dental Receptionist — *AI voice/chat booking system*
`Node.js` · `Express` · `SQLite / PostgreSQL` · `Anthropic tool-calling` · `JWT` · `Web Speech API` · `Jest`

- Built a patient-facing voice and chat receptionist that books, cancels, and reschedules appointments against a **real database** — no invented availability or mock responses.
- Implemented an availability engine with **slot locking and double-booking prevention**, shared by the REST API, the voice widget, and the LLM tool layer through one code path.
- Wired real Anthropic tool-calling so the AI calls the exact same service functions as direct API clients; designed the system to degrade to a clear "AI unavailable" state with no key set.
- Layered JWT authentication, rate limiting, an `NotificationService` abstraction (email/SMS/WhatsApp), and a Jest test suite over the business logic.

### J.A.R.V.I.S. — *Personal AI operating system for Windows*
`Python 3.11+` · `FastAPI` · `WebSocket` · `Web Speech API` · `Anthropic / OpenAI-compatible providers`

- Designed a modular desktop AI assistant that performs **real computer operations** — launching apps, managing files, monitoring system health, and running gated shell commands — exposed through **36 tools** across app, file, system, web, memory, and developer categories.
- Built a **permission and risk engine** classifying every action by permission level (safe / confirm / always-confirm) and risk (low → critical), so irreversible actions can never be silently auto-run.
- Implemented a genuine offline **rule-based intent router** provider so the assistant is fully useful with no API key and no internet, with cloud providers swappable at runtime and nothing hard-coded.
- Added multilingual routing (English, Urdu, Roman Urdu), a live system HUD (CPU/RAM/disk/network/battery), voice with wake word and barge-in, and a drop-in plugin/skill system — with every tool call and approval written to an audit log.

### LexOffice — *Law firm management ERP*
`Node.js` · `Express` · `SQLite` · `JWT` · `bcrypt` · `Electron`

- Re-architected a single-file, browser-IndexedDB demo into a **multi-user client-server system** with a real server-side database and server-verified login.
- Built a REST API and data layer covering clients, cases, and firm modules, with **role-based permissions** for Admin, Lawyer, Assistant, and Accountant.
- Implemented first-run seeding so a new install self-populates demo data and is usable immediately.
- Packaged the entire stack as a cross-platform **Electron desktop application** (`.exe` / `.dmg` / `.AppImage`).

### University ERP System — *Student · Faculty · Admin portals*
`Node.js` · `Express` · `PostgreSQL` · `JWT` · `bcrypt` · `zod` · `helmet`

- Delivered three role-based portals plus a public admissions website, all reading and writing **live PostgreSQL data** — no sample data in the running system.
- Implemented attendance marking with duplicate-save prevention, results with automatic letter-grade computation, CGPA, transcripts (print/PDF), exam slips, invoices, hostel, and multi-step student request workflows (retest, course drop, defer term, final degree).
- Secured the system end to end: bcrypt password hashing, fully parameterised queries, zod validation on every input, rate-limited login and write endpoints, and a Content-Security-Policy via helmet.
- Enforced **row-level ownership in SQL** rather than the UI — a student can only ever read their own records, and faculty can only mark or grade students enrolled on their own courses.

---

## Experience

**Independent Projects** — *Self-directed* · *2024 – Present*
- Designed and delivered four full-stack systems end to end (database schema, REST API, auth and permissions, frontend, desktop packaging) spanning ERP, AI assistant, and AI voice-booking domains.
- Built AI features using the Anthropic SDK with real tool-calling agent loops wired to production service functions, including graceful degradation when no API key is configured.
- Implemented security baselines on every project: bcrypt hashing, JWT auth, role-based access control, zod validation, rate limiting, and row-level ownership enforced in SQL.

*[Add any employer roles here — title, company, dates, and 2–3 bullet points. Most recent first.]*

**Job Title** — Company Name · *Month YYYY – Month YYYY*
- What you built or improved, and the measurable result (e.g. "cut X from Y to Z").
- What you worked on and who you owned.

---

## Education

**BS Computer Science** — Superior University, Lahore

*Currently in 2nd semester — expected graduation 2029*

---

## Languages

- **Urdu** — Native
- **English** — Professional working proficiency
- **Punjabi** — Conversational

---

*All projects listed above are open-source on GitHub ([github.com/hamidkhan069731-blip](https://github.com/hamidkhan069731-blip)), with a live portfolio at [hamidkhan069731-blip.github.io](https://hamidkhan069731-blip.github.io/).*
