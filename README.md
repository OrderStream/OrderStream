# Systems & Protocol Engineering | Database Internals | Distributed Settlement

```text
Specialization: PostgreSQL / PostgREST Internals | Supabase RLS Hardening | Async Python (FastAPI) | Stellar & Soroban Contracts (Rust)
Status: Open for High-Impact Protocol Architecture, Smart Contracts & Distributed Systems Engineering
```

---

### Engineering Philosophy & Core Focus

I design and harden resilient backend infrastructure, low-latency microservices, database layers, and smart contracts for data-intensive and on-chain applications. My work focuses on deterministic correctness, zero-leak error boundaries, strict ACID guarantees, and automated regression testing.

- **Smart Contracts & Blockchain Protocols:** High-performance, memory-metered Soroban smart contracts in Rust (`soroban-sdk`), atomic cross-contract invocations, Soroban RPC event ingestion pipelines, persistent TTL state maintenance, and re-entrancy / replay defenses.
- **Relational Databases & RLS:** Advanced PostgreSQL optimization, PostgREST query planner mechanics, atomic relational mutation procedures (PL/pgSQL), updatable view triggers, and Row Level Security (RLS) policy hardening.
- **High-Throughput Backends:** Modern asynchronous microservices with Python (FastAPI / Starlette), Pydantic v2 validation pipelines, and dependency-injected JWT authentication.
- **Enterprise Data Serialization:** High-volume RFC-compliant data pipeline exporters (RFC 5545 iCalendar, ISO-standard OpenXML/XLSX, JSON Lines, SQLite) engineered with memory streaming and formula injection defenses.
- **Payment & Settlement Rails:** Idempotent webhook receivers (Stripe signature verification with replay defense) and non-custodial Web3 escrow rails (Stellar / Soroban & Base Network USDC).

---

### Technical Stack & Tooling

| Domain | Technologies & Standards |
| :--- | :--- |
| **Languages** | Rust (2021/2024 edition), Python 3.11+, TypeScript / Node.js, SQL (PostgreSQL), Bash |
| **Blockchain & Smart Contracts** | Stellar Network, Soroban SDK, Soroban RPC, WebAssembly (`wasm32v1-none`), Stellar CLI |
| **Databases & Engines** | PostgreSQL, PostgREST, Supabase, Redis (streams/keyspace/caching), SQLite |
| **Frameworks & Libraries** | FastAPI, Starlette, Pydantic v2, SQLAlchemy, Asyncpg, Pytest, Cargo, Vitest / Jest |
| **Security & Audits** | Soroban auth verification (`require_auth`), Timing-safe HMAC verification, JWT blocklisting & Redis Pub/Sub invalidation, RLS isolation policies |
| **DevOps & Verification** | Docker, GitHub Actions CI/CD, Git, cargo-deny, cargo-machete, Pre-commit automated regression suites |

---

### Notable Open Source Contributions

#### 🌊 Stellar & Soroban Ecosystem (Wave Program Contributor & Peer Reviewer)
- **[DelegoLabs/Delego-backend](https://github.com/DelegoLabs/Delego-backend):**
  - Engineered the background Soroban RPC event ingestion worker with persistent checkpoint tracking in Redis and idempotent database synchronization for escrow states ([PR #705](https://github.com/DelegoLabs/Delego-backend/pull/705)).
- **[dultimateade/hermes](https://github.com/dultimateade/hermes):**
  - Resolved market dispute resolution storage tier mismatches, eliminated redundant storage double-reads in `claim_winnings`, aligned persistent TTL extension thresholds, and built resolution unit test suites ([PR #321](https://github.com/dultimateade/hermes/pull/321), [PR #322](https://github.com/dultimateade/hermes/pull/322), [PR #323](https://github.com/dultimateade/hermes/pull/323)).
- **[Pidoko257/proxypay](https://github.com/Pidoko257/proxypay):**
  - Implemented callback idempotency tracking and duplicate suppression for mobile money integration, along with banker's rounding algorithms for multi-currency settlement ([PR #720–#724](https://github.com/Pidoko257/proxypay/pull/720)).
- **Active Peer Reviewer:**
  - Submitted 15+ formal architecture, security, and CI code reviews across open-source Stellar tools including `benelabs/crucible`, `0xLizTech/stellarforge`, and `StreamFi-x/streamfi-frontend`.

#### ⚡ Python, AI & Distributed Systems
- **[BasedHardware/omi](https://github.com/BasedHardware/omi):**
  - Contributed 22+ production-grade data export and serialization recipes across the Python CLI SDK.
  - Implemented high-performance data transformation engines for memory, goal, and conversation streams (iCalendar RFC 5545, Excel OpenXML with injection mitigation, JSONL, SQLite, and Markdown digest pipelines).
  - Hardened backend API integration endpoints (`phone_calls`, `google_calendar`) to prevent internal detail leaks and provider reflection exploits.
- **Supabase & PostgREST Tooling:**
  - Designed atomic stored procedure patterns (`jsonb_to_recordset` multi-table ACID inserts) solving PostgREST relational write embedding constraints (PGRST204).
  - Authored dual-policy RLS patterns resolving representation rollbacks (42501) on authenticated insert pipelines.

---

### Engagements & Collaboration

Available for:
- Soroban smart contract engineering & security audits (Rust)
- Soroban RPC indexing pipelines & on-chain state reconciliation
- Database architecture & Row Level Security (RLS) security audits
- PostgREST & Supabase complex query / RPC migration hardening
- High-concurrency FastAPI microservice development & API refactoring
- Contract-based protocol development with milestone-based settlement

**Settlement Rails:** Base Network USDC (`0x5de2b62434754bfd39ef350a3a867ed3eced5074`) • Stellar Network USDC / XLM • Escrow / Direct
