<h1 align="center">Louis Cospain</h1>

<p align="center">
  <a href="https://github.com/elcoosp"><img alt="GitHub" src="https://img.shields.io/badge/%40elcoosp-181717?style=flat-square&logo=github&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/louis-cospain-a71464169"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:elcoosp@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img alt="Location" src="https://img.shields.io/badge/Nantes%2C%20France-4F46E5?style=flat-square&logo=googlemaps&logoColor=white"/>
</p>

<p align="center">
  <img alt="Rust" src="https://img.shields.io/badge/2_years_full--time_Rust%2C_100%25_in_public-000000?style=flat-square&logo=rust&logoColor=white"/>
  <img alt="Output" src="https://img.shields.io/badge/2_compilers_%C2%B7_7_products_in_public-4F46E5?style=flat-square"/>
  <img alt="Contributions" src="https://img.shields.io/badge/20k%2B_contributions_last_year-0D9488?style=flat-square"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/8_years_production_TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
</p>

**Rust engineer with a product-builder's track record.** Eight years shipping TypeScript to production — six of them at Weenat (agri-tech, 10k+ IoT sensors, live on the App Store & Google Play). Since 2024 I've bet on Rust full-time and built everything in public: complete systems with specs, ADRs, test suites and CI — not tutorials.

> Two years produced: a UI language that compiles to real SwiftUI & Jetpack Compose, a local-first AI agent harness, a zero-knowledge password manager, a from-scratch Rust-like compiler, and a sub-10ms multiplayer poker engine.

```rust
// this profile, as code
let shipped = vec!["flux", "kod", "vautr", "glyim", "stackbluff", "ataqu"];
debug_assert!(shipped.iter().all(|p| is_public(p) && is_spec_driven(p) && is_tested(p)));

let next = Role::rust().in_france(&["Nantes", "Paris", "remote"]);
// interested? → elcoosp@gmail.com
```

## 🦀 Flagship Rust work

| | What it is | Receipts |
|---|---|---|
| **[flux](https://github.com/elcoosp/flux)** | Write-once UI language for native iOS & Android. Edit `.flux` source, hot-reload on-device in milliseconds as binary IR patches over WebSocket — release builds compile to real **SwiftUI** & **Jetpack Compose**. No webview, no JS bridge, no interpreter in prod. | 16 crates · ~63k LOC of Rust · 92 golden ISA vectors · 39 ADRs · 19 CI workflows incl. wire-protocol fuzzing & mutation testing |
| **[kod](https://github.com/elcoosp/kod)** | Local-first AI coding-agent harness (TUI + CLI). Streaming agentic loop, multi-agent swarm, MCP & LSP clients, sandboxed shell, JSONL session audit with `kod replay`. Your code never leaves your machine. | 20 crates · ~4000 tests · Landlock / bwrap / sandbox-exec |
| **[vautr](https://github.com/elcoosp/vautr)** | Zero-knowledge password manager: OPAQUE authentication + Argon2id, offline-first sync. The server never sees your secrets. | Rust core · React / Expo / GPUI clients · AGPL, self-hostable forever |
| **[glyim](https://github.com/elcoosp/glyim)** | From-scratch compiler for a Rust-like systems language, written in Rust: lexing → HIR/MIR → type inference & trait solving → NLL borrow checking. | full pipeline, no rustc internals |
| **[stackbluff](https://github.com/elcoosp/stackbluff)** | Multiplayer poker platform: sub-10ms Rust engine, AI coach, bots, anti-cheat, clubs & tournaments, Stripe billing. | built end-to-end by 5 parallel AI agents |
| **[ataqu](https://github.com/elcoosp/ataqu)** | 10 natively-integrated business apps (CRM, Chat, HR, Docs, SSO, Analytics…) on a single Rust + PostgreSQL core. | monorepo · Next.js front-end |

Also: **[chameleon](https://github.com/elcoosp/chameleon)** — HUNL poker AI, mixture-of-archetype blueprints trained & benchmarked on an M1 (pure Rust) · **[skilldeck](https://github.com/elcoosp/skilldeck)** — local-first multi-agent AI orchestration (Tauri).

## 📦 Production track record (pre-Rust)

- **Weenat** — agri-tech, 6 years full-stack TypeScript
  - 10k+ IoT weather sensors in production; mobile app live on **App Store & Google Play**
  - Led the **React Native/JS → Expo/TypeScript** migration across mobile & web
  - Built the **IoT alert microservice** (Node.js, AWS SQS)
  - Shipped a back-office letting marketing manage **5 languages with zero dev tickets**
- **[lynxpo](https://github.com/elcoosp/lynxpo)** — 66 Expo-style native modules (Camera, SQLite, SecureStore…) reimplemented for ByteDance Lynx with Kotlin + Swift twins, one pnpm workspace, live playground
- **[vantage](https://github.com/elcoosp/vantage)** — multi-tenant merchant SaaS in Java 21 / Spring Boot 3.4: Saga/Outbox, event-driven, GraphQL, RabbitMQ

## 🧭 How I work

- **Spec before code** — flux carries 39 MADR ADRs plus a full wire-protocol & VM-ISA spec; kod ships SPEC, ARCHITECTURE and TESTING documents.
- **Tests are the design review** — cargo-nextest, proptest, insta snapshots, criterion performance budgets (`parse < 5 ms`, `diff < 1 ms`, `VM eval < 2 ms`); ~4000 tests across kod's crates.
- **CI like it's production** — clippy `-D warnings`, `#![forbid(unsafe_code)]` in every library crate, fuzzed wire protocol, mutation testing, parity harnesses.
- **AI-augmented, engineer-owned** — I ship daily with Claude Code & MCP, and I built my own harness (kod) to keep the loop local, sandboxed and auditable.

## ⚡ Currently

- **flux**: converging the iOS dev tier onto the declarative release pipeline (ADR-0048)
- **kod**: work-stealing swarm dispatch and remote-daemon attach (see "Tracked gaps")

## 🎯 Open to

**Rust engineer roles** — backend, systems, product or security-adjacent. France (Nantes / Paris) or remote. I want a long-term product team where I own features end-to-end and keep shipping. Bonus points if the roadmap touches compilers, real-time, developer tooling or applied crypto — that's where my public work lives.

## 🛠️ Stack

![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![React Native](https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)

**Rust ecosystem, in anger:** tokio · axum · clap · ratatui · redb · blake3 · MessagePack · proptest · insta · criterion · cargo-nextest · OpenTelemetry

## 📈 Stats

![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=elcoosp&theme=github&animation=fade)
![](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=elcoosp&theme=github&animation=fade)

<p align="center"><i>Everything I build is public. If any of it is interesting to you — <a href="mailto:elcoosp@gmail.com">let's talk</a>.</i></p>
