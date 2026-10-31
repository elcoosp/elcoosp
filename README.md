<h1 align="center">Louis Cospain</h1>

<p align="center">
  <a href="https://github.com/elcoosp"><img alt="GitHub" src="https://img.shields.io/badge/%40elcoosp-181717?style=flat-square&logo=github&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/louis-cospain-a71464169"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:elcoosp@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img alt="Location" src="https://img.shields.io/badge/Nantes,%20France-4F46E5?style=flat-square&logo=googlemaps&logoColor=white"/>
</p>

<p align="center">
  <img alt="Rust" src="https://img.shields.io/badge/2_years_full--time_Rust,_100%25_in_public-000000?style=flat-square&logo=rust&logoColor=white"/>
  <img alt="Output" src="https://img.shields.io/badge/2_compilers_-_7_products_in_public-4F46E5?style=flat-square"/>
  <img alt="Contributions" src="https://img.shields.io/badge/6k%2B_contributions_in_Oct_2026-0D9488?style=flat-square"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/8_years_production_TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
</p>

**Rust engineer with a product-builder's track record.** Eight years shipping TypeScript to production — six of them at Weenat (agri-tech, 10k+ IoT sensors, live on the App Store & Google Play). Since 2024 I have bet on Rust full-time and built everything in public: complete systems with specs, ADRs, test suites and CI — not tutorials.

> Recent output: a framework-agnostic full-stack meta-framework (`oxide`), a reactive abstraction layer (`quoin`), an end-to-end HUNL poker AI (`pkr-sota`), and massive ongoing work on `kod`, `glyim`, and `flux`.

```rust
// this profile, as code
let shipped = vec!["flux", "kod", "vautr", "glyim", "stackbluff", "oxide", "quoin", "pkr-sota"];
debug_assert!(shipped.iter().all(|p| is_public(p) && is_spec_driven(p) && is_tested(p)));

let next = Role::rust().in_france(&["Nantes", "Paris", "remote"]);
// interested? -> elcoosp@gmail.com
```

## Flagship Rust Work

| Repository | What it is | Receipts |
|---|---|---|
| **[oxide](https://github.com/elcoosp/oxide)** | Framework-agnostic full-stack meta-framework with a Rust core. React, Vue, Svelte, and Solid over one shared engine. Compiles to a single static binary, ships to 12 deploy targets. | 18 crates · ODF binary wire format · 3-tier cache · 2,300+ commits in Oct 2026 |
| **[quoin](https://github.com/elcoosp/quoin)** | Framework-agnostic reactive abstraction layer for Rust. Write reactive business logic once using signals and effects, run across GPUI, Leptos, Dioxus, Xilem, or Floem. | Unified Reactive API · Declarative macros · Tailwind class transpilation |
| **[kod](https://github.com/elcoosp/kod)** | Local-first AI coding-agent harness (TUI + CLI). Streaming agentic loop, multi-agent swarm, MCP & LSP clients, sandboxed shell, JSONL session audit. Your code never leaves your machine. | 20 crates · ~4000 tests · Landlock / bwrap / sandbox-exec · 1,300+ commits in Oct 2026 |
| **[glyim](https://github.com/elcoosp/glyim)** | From-scratch compiler for a Rust-like systems language, written in Rust: lexing -> HIR/MIR -> type inference & trait solving -> NLL borrow checking. | Full pipeline, no rustc internals · 580+ commits in Oct 2026 |
| **[pkr-sota](https://github.com/elcoosp/pkr-sota)** | End-to-end heads-up No-Limit Hold'em poker AI in Rust. Precompute, train, export, and query a CFR blueprint on a single machine with nanosecond lookup times. | Deterministic training · mmap blueprint loading · p50 ≈ 42ns queries · 460+ tests |
| **[vautr](https://github.com/elcoosp/vautr)** | Zero-knowledge password manager: OPAQUE authentication + Argon2id, offline-first sync. The server never sees your secrets. | Rust core · React / Expo / GPUI clients · AGPL, self-hostable forever |
| **[flux](https://github.com/elcoosp/flux)** | Write-once UI language for native iOS & Android. Hot-reload on-device as binary IR patches over WebSocket — release builds compile to real SwiftUI & Jetpack Compose. | 16 crates · ~63k LOC of Rust · 92 golden ISA vectors · 39 ADRs |
| **[stackbluff](https://github.com/elcoosp/stackbluff)** | Multiplayer poker platform: sub-10ms Rust engine, AI coach, bots, anti-cheat, clubs & tournaments, Stripe billing. | Built end-to-end by 5 parallel AI agents |

## TypeScript & Full-Stack Work

| Repository | What it is | Receipts |
|---|---|---|
| **[takumi-motion](https://github.com/elcoosp/takumi-motion)** | Deterministic server-side animation engine that renders React components or HTML to GIF, WebP, or APNG. | TypeScript/React integration · Server-side rendering pipeline · Created Oct 2026 |

## Production Track Record (Pre-Rust)

- **Weenat** — agri-tech, 6 years full-stack TypeScript
  - 10k+ IoT weather sensors in production; mobile app live on App Store & Google Play
  - Led the React Native/JS -> Expo/TypeScript migration across mobile & web
  - Built the IoT alert microservice (Node.js, AWS SQS)
  - Shipped a back-office letting marketing manage 5 languages with zero dev tickets

## How I Work

- **Spec before code** — flux carries 39 MADR ADRs plus a full wire-protocol & VM-ISA spec; kod ships SPEC, ARCHITECTURE and TESTING documents; oxide maintains strict spec-vs-code deviation docs.
- **Tests are the design review** — cargo-nextest, proptest, insta snapshots, criterion performance budgets (`parse < 5 ms`, `diff < 1 ms`, `VM eval < 2 ms`); ~4000 tests across kod's crates; Miri-clean core crates in pkr-sota.
- **CI like it's production** — clippy `-D warnings`, `#![forbid(unsafe_code)]` in every library crate, fuzzed wire protocol, mutation testing, parity harnesses, golden-hash CI gates.
- **AI-augmented, engineer-owned** — I ship daily with AI & MCP, and I built my own harness (kod) to keep the loop local, sandboxed and auditable.

## Currently (October 2026)

- **oxide**: Fixing website routing/CSS injection across render paths, refining the CLI/router scanner, and expanding documentation (local dev, CI, release, security) while enforcing workspace-wide build checks.
- **quoin**: Implementing proper `JoinHandle` abort/detach semantics and fixing `request_update` recursion across all framework adapters (GPUI, Leptos, Dioxus, Xilem, Floem). Bounding cancellation waker registries to prevent memory leaks.
- **kod**: Refactoring `tools.rs` by extracting shared helpers (`atomic_write`, `kill_child_tree`) to enable parallel tool splits. Closed v0.1.27 audit sweep with memory obfuscation fixes and documented the main-loop split proposal.
- **glyim**: Fixing signed wrapping arithmetic and literal receiver method resolution. Investigating a critical LLVM backend miscompile where `checked_*` operations on signed integers incorrectly used unsigned intrinsics, requiring a coordinated fix across typeck, interp, and LLVM backends.
- **pkr-sota**: Shipped K=7 action abstraction, but documented a +261 mbb regression in run 1 ("DO NOT SHIP"). Measured Phase 5 infeasibility at current resolution (time bottleneck) and corrected audit claims about memory size (UndoRecord is the dominant cost). Fixed parallel test temp-file races.
- **flux**: Expanding ISA vector coverage for uncovered opcodes (`remove_item_basic`, `clear_basic`), fixing `BOOL_EQ` operand lengths, and ensuring `content_address` gracefully handles dangling child references without panicking.

## Open To

**Rust engineer roles** — backend, systems, product or security-adjacent. France (Nantes / Paris) or remote. I want a long-term product team where I own features end-to-end and keep shipping. Bonus points if the roadmap touches compilers, real-time, developer tooling, reactive systems, or applied crypto — that is where my public work lives.

## Stack

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

**Rust ecosystem, in anger:** tokio · axum · clap · ratatui · redb · blake3 · MessagePack · proptest · insta · criterion · cargo-nextest · OpenTelemetry · hyper · rustls · Oxc · Rolldown

## Stats

![](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=elcoosp&theme=github&animation=fade)
![](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=elcoosp&theme=github&animation=fade)

<p align="center"><i>Everything I build is public. If any of it is interesting to you — <a href="mailto:elcoosp@gmail.com">let's talk</a>.</i></p>
