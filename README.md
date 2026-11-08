<h1 align="center">Louis Cospain</h1>

<p align="center">
  <a href="https://github.com/elcoosp"><img alt="GitHub" src="https://img.shields.io/badge/%40elcoosp-181717?style=flat-square&logo=github&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/louis-cospain-a71464169"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:elcoosp@gmail.com"><img alt="Email" src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white"/></a>
  <img alt="Location" src="https://img.shields.io/badge/Nantes,%20France-4F46E5?style=flat-square&logo=googlemaps&logoColor=white"/>
</p>

<p align="center">
  <img alt="Rust" src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img alt="Zig" src="https://img.shields.io/badge/Zig-F7A41D?style=flat-square&logo=zig&logoColor=black"/>
  <img alt="Commits" src="https://img.shields.io/badge/34,280_contributions_last_year-0D9488?style=flat-square"/>
  <img alt="Repos" src="https://img.shields.io/badge/15_new_repositories_Nov_2026-4F46E5?style=flat-square"/>
</p>

**Rust engineer with a product-builder's track record.** Eight years shipping TypeScript to production — six of them at Weenat (agri-tech, 10k+ IoT sensors, live on the App Store & Google Play). Since 2024 I have bet on Rust full-time and built everything in public: complete systems with specs, ADRs, test suites and CI — not tutorials.

> **November 2026 alone:** 15 new repositories, spanning a UI compiler (`ligature`), a retained-mode GUI framework (`alacer`), a Zig JSX compiler (`zsx`), a parser toolkit (`syntact`), a Tailwind-to-native styling engine (`aeolus`), and a zero-copy BitTorrent toolkit (`magnetite`) — alongside sustained work on `glyim`, `oxide`, `pkr-sota`, and more.

---

## Work Map

### Compilers & Language Infrastructure

- **[glyim](https://github.com/elcoosp/glyim)** — Research-grade compiler for a Rust-like language. Full pipeline: lexing → HIR/MIR → type inference & trait solving → NLL borrow checking → LLVM/bytecode. **20+ crates · end-to-end functional**
- **[ligature](https://github.com/elcoosp/ligature)** — UI compiler turning Solid TSX and Vue SFC into `no_std` Rust components. Byte-identical IR across both frontends.
- **[syntact](https://github.com/elcoosp/syntact)** — Parser toolkit that compiles grammar packages into lossless, error-recovering parsers, queries, and LSP servers. Language packs for JSON, TOML, Python, TypeScript, Rust, C, SQL, INI, CSV, Markdown.
- **[zsx](https://github.com/elcoosp/zsx)** — JSX-like view syntax for Zig, compiled at comptime to native GUI code for `dvui` and `nanoui`. **130+ tests · no runtime parser**

### UI Frameworks & Reactive Systems

- **[oxide](https://github.com/elcoosp/oxide)** — Framework-agnostic full-stack meta-framework with a Rust core. React, Vue, Svelte, and Solid over one shared engine. Compiles to a single static binary. **18 crates · ODF binary wire format · 3-tier cache · 2,300+ commits in Oct 2026**
- **[quoin](https://github.com/elcoosp/quoin)** — Framework-agnostic reactive abstraction layer for Rust. Signals and effects that run across GPUI, Leptos, Dioxus, Xilem, or Floem.
- **[flux](https://github.com/elcoosp/flux)** — Write-once UI language for native iOS & Android. Hot-reload as binary IR patches over WebSocket; release builds compile to SwiftUI & Jetpack Compose. **16 crates · ~63k LOC Rust · 39 ADRs**
- **[alacer](https://github.com/elcoosp/alacer)** — Retained-mode Rust GUI framework with accessibility built in. Only dirty subtrees relayout or repaint. **14.76× faster incremental relayout · headless CI**
- **[aeolus](https://github.com/elcoosp/aeolus)** — Tailwind CSS v4 class strings compiled to native properties for Xilem/Masonry, Floem, Iced, egui, and Slint. **No Node · no CSS build step**
- **[tuvix](https://github.com/elcoosp/tuvix)** — Terminal UI framework where input preempts rendering. Budgeted frames, zero-alloc diffing, built-in time-travel debugging. **Three backends · C embedding boundary**
- **[nexum](https://github.com/elcoosp/nexum)** — Framework-agnostic deep linking for Rust desktop apps. Custom URL schemes and OAuth callbacks across Windows, macOS, Linux, Android, and iOS.

### Developer Tools & Systems

- **[kod](https://github.com/elcoosp/kod)** — Local-first AI coding-agent harness (TUI + CLI). Streaming agentic loop, multi-agent swarm, MCP & LSP clients, sandboxed shell. **20 crates · ~4000 tests · Landlock / bwrap / sandbox-exec**
- **[wraith](https://github.com/elcoosp/wraith)** — High-performance in-memory PNG → optimised SVG vectorizer. Sub-pixel geometric colour engine, gradient fitting, OXVG minification. **6.4 ms for 3.2 kB → 765 B**
- **[magnetite](https://github.com/elcoosp/magnetite)** — Zero-copy BitTorrent metadata toolkit: bencode codec, magnet URI and `.torrent` parsing, UDP tracker client. **No unsafe · no async runtime**
- **[pkr-sota](https://github.com/elcoosp/pkr-sota)** — End-to-end heads-up NLHE poker AI in Rust. CFR blueprint training, `mmap` runtime, nanosecond lookups. **p50 ≈ 42 ns · 460+ tests**

### Applications & Platforms

- **[vautr](https://github.com/elcoosp/vautr)** — Zero-knowledge password manager: OPAQUE authentication + Argon2id, offline-first sync. **Rust core · React / Expo / GPUI clients · AGPL**
- **[stackbluff](https://github.com/elcoosp/stackbluff)** — Multiplayer poker platform: sub-10ms Rust engine, AI coach, bots, anti-cheat, clubs & tournaments, Stripe billing.
- **[takumi-motion](https://github.com/elcoosp/takumi-motion)** — Deterministic server-side animation engine rendering React components or HTML to GIF, WebP, or APNG.

---

## Created in November 2026

These repositories were created between **Nov 3–7, 2026**, according to your public activity feed:

| Domain                  | Repositories                                                                     |
| ----------------------- | -------------------------------------------------------------------------------- |
| **Compilers & parsing** | `ligature` · `zsx` · `syntact`                                                   |
| **GUI & native UI**     | `alacer` · `aeolus` · `guiwright`                                                |
| **Systems & tooling**   | `magnetite` · `wraith` · `upd`                                                   |
| **Other**               | `starlight` · `catheo` · `tuvix` · `peregrine` · `gpui-rsx` · `leptos-shadcn-ui` |

All are public and active as of **Nov 8, 2026**.

---

## How I Work

- **Spec before code** — `flux` carries 39 MADR ADRs plus a full wire-protocol & VM-ISA spec; `kod` ships SPEC, ARCHITECTURE and TESTING documents; `oxide` maintains strict spec-vs-code deviation docs.
- **Tests are the design review** — `cargo-nextest`, `proptest`, `insta` snapshots, `criterion` performance budgets (`parse < 5 ms`, `diff < 1 ms`, `VM eval < 2 ms`); ~4000 tests across `kod`'s crates; Miri-clean core crates in `pkr-sota`.
- **CI like it's production** — clippy `-D warnings`, `#![forbid(unsafe_code)]` in every library crate, fuzzed wire protocol, mutation testing, parity harnesses, golden-hash CI gates.
- **AI-augmented, engineer-owned** — I ship daily with AI & MCP, and I built my own harness (`kod`) to keep the loop local, sandboxed, and auditable.

---

## Currently (November 2026)

- **glyim** — Fixing signed wrapping arithmetic and literal receiver method resolution; investigating an LLVM backend miscompile around `checked_*` on signed integers.
- **oxide** — Fixing website routing/CSS injection across render paths, refining the CLI/router scanner, expanding documentation.
- **pkr-sota** — K=7 action abstraction shipped but documented a +261 mbb regression (“DO NOT SHIP”); measured Phase 5 infeasibility; corrected audit claims on memory size.
- **kod** — Refactoring `tools.rs` by extracting shared helpers (`atomic_write`, `kill_child_tree`); closed v0.1.27 audit sweep.
- **New November projects** — `ligature`, `alacer`, `syntact`, `aeolus`, `tuvix`, `magnetite`, `wraith`, `nexum`, `zsx` all created and actively updated through **Nov 8, 2026**.

---

## Open To

**Rust engineer roles** — backend, systems, product, or security-adjacent. France (Nantes / Paris) or remote. I want a long-term product team where I own features end-to-end and keep shipping. Bonus points if the roadmap touches compilers, real-time, developer tooling, reactive systems, or applied crypto — that is where my public work lives.

[elcoosp@gmail.com](mailto:elcoosp@gmail.com)

---

## Stack

<p>
  <img alt="Rust" src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white"/>
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img alt="React" src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img alt="React Native" src="https://img.shields.io/badge/React_Native-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img alt="Expo" src="https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white"/>
  <img alt="Next.js" src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white"/>
  <img alt="Node.js" src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white"/>
  <img alt="Spring Boot" src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white"/>
  <img alt="AWS" src="https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white"/>
</p>

**Rust ecosystem, in anger:** `tokio` · `axum` · `clap` · `ratatui` · `redb` · `blake3` · `MessagePack` · `proptest` · `insta` · `criterion` · `cargo-nextest` · `OpenTelemetry` · `hyper` · `rustls` · `Oxc` · `Rolldown`

---

<p align="center"><i>Everything I build is public. If any of it is interesting — <a href="mailto:elcoosp@gmail.com">let's talk</a>.</i></p>
