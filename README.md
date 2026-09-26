# Systems & Backend Architecture | Database Internals | Distributed Services

```text
Specialization: PostgreSQL / PostgREST Internals | Supabase RLS Hardening | Async Python (FastAPI) | On-Chain Settlement
Status: Open for High-Impact Fractional Architecture & Systems Engineering
```

---

### Engineering Philosophy & Core Focus

I design and harden resilient backend infrastructure, low-latency microservices, and database layers for data-intensive applications. My work focuses on deterministic correctness, zero-leak error boundaries, strict ACID guarantees, and automated regression testing.

- **Relational Databases & RLS:** Advanced PostgreSQL optimization, PostgREST query planner mechanics, atomic relational mutation procedures (PL/pgSQL), updatable view triggers, and Row Level Security (RLS) policy hardening.
- **High-Throughput Backends:** Modern asynchronous microservices with Python (FastAPI / Starlette), Pydantic v2 validation pipelines, and dependency-injected JWT authentication.
- **Enterprise Data Serialization:** High-volume RFC-compliant data pipeline exporters (RFC 5545 iCalendar, ISO-standard OpenXML/XLSX, JSON Lines, SQLite) engineered with memory streaming and formula injection defenses.
- **Payment & Settlement Rails:** Idempotent webhook receivers (Stripe signature verification with replay defense) and non-custodial Web3 escrow rails (Base Network USDC).

---

### Technical Stack & Tooling

| Domain | Technologies & Standards |
| :--- | :--- |
| **Languages** | Python 3.11+, SQL (PostgreSQL dialect), TypeScript / Node.js, Bash |
| **Databases & Engines** | PostgreSQL, PostgREST, Supabase, SQLite, Redis |
| **Frameworks & Libs** | FastAPI, Starlette, Pydantic v2, SQLAlchemy, Asyncpg, Pytest |
| **Security & Auth** | Supabase Auth JWT validation, OAuth 2.0, RLS isolation policies, Timing-safe HMAC verification |
| **DevOps & Verification** | Docker, GitHub Actions CI/CD, Git, Pre-commit automated regression test suites |

---

### Notable Open Source Contributions

- **[BasedHardware/omi](https://github.com/BasedHardware/omi):**
  - Contributed 22+ production-grade data export and serialization recipes across the Python CLI SDK.
  - Implemented high-performance data transformation engines for memory, goal, and conversation streams (iCalendar RFC 5545, Excel OpenXML with injection mitigation, JSONL, SQLite, and Markdown digest pipelines).
  - Hardened backend API integration endpoints (`phone_calls`, `google_calendar`) to prevent internal detail leaks and provider reflection exploits.
- **Supabase & PostgREST Tooling:**
  - Designed atomic stored procedure patterns (jsonb_to_recordset multi-table ACID inserts) solving PostgREST relational write embedding constraints (PGRST204).
  - Authored dual-policy RLS patterns resolving representation rollbacks (42501) on authenticated insert pipelines.

---

### Engagements & Collaboration

Available for:
- Database architecture & Row Level Security (RLS) security audits
- PostgREST & Supabase complex query / RPC migration hardening
- High-concurrency FastAPI microservice development & API refactoring
- Contract-based development with milestone-based settlement

**Settlement Rails:** Base Network USDC (`0x5de2b62434754bfd39ef350a3a867ed3eced5074`) • Escrow / Direct
