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
  <img alt="Contributions" src="https://img.shields.io/badge/Contributions-34280-0D9488?style=flat-square"/>
  <img alt="Repos" src="https://img.shields.io/badge/Repos-15_new-4F46E5?style=flat-square"/>
</p>

**Rust engineer with a product-builder's track record.** Eight years shipping TypeScript to production — six of them at Weenat (agri-tech, 10k+ IoT sensors, live on the App Store & Google Play). Since 2024 I have bet on Rust full-time and built everything in public: complete systems with specs, ADRs, test suites and CI — not tutorials.

> **November 2026 alone:** 15 new repositories, spanning a UI compiler (`ligature`), a retained-mode GUI framework (`alacer`), a Zig JSX compiler (`zsx`), a parser toolkit (`syntact`), a Tailwind-to-native styling engine (`aeolus`), and a zero-copy BitTorrent toolkit (`magnetite`) — alongside sustained milestone work on `glyim`, `oxide`, `pkr-sota`, `kod`, and more.

---

## Work Map

### Compilers & Language Infrastructure

- **[glyim](https://github.com/elcoosp/glyim)** — Research-grade compiler for a Rust-like language. Full pipeline: lexing → HIR/MIR → type inference & trait solving → NLL borrow checking → LLVM/bytecode. Backed by a readiness ledger that gates milestones and a `glyim-metrics` ratchet wired into CI.
- **[ligature](https://github.com/elcoosp/ligature)** — UI compiler turning Solid TSX and Vue SFC into `no_std` Rust components. Byte-identical IR across both frontends; M10 adds per-mount identity and branch-time assembly.
- **[syntact](https://github.com/elcoosp/syntact)** — Parser toolkit compiling grammar packages into lossless, error-recovering parsers, queries, and LSP servers. Pack LSP now shipped; grammar→descriptor compiler (`descent-lower`) landed.
- **[zsx](https://github.com/elcoosp/zsx)** — JSX-like view syntax for Zig, compiled at comptime to native GUI code for `dvui` and `nanoui`. No runtime parser; playgrounds for both adapters.

### UI Frameworks & Reactive Systems

- **[oxide](https://github.com/elcoosp/oxide)** — Framework-agnostic full-stack meta-framework with a Rust core. React, Vue, Svelte, and Solid over one shared engine. F04 substrate milestone landed: experiments config section, assignment engine, criterion benches.
- **[quoin](https://github.com/elcoosp/quoin)** — Framework-agnostic reactive abstraction layer for Rust. Signals and effects that run across GPUI, Leptos, Dioxus, Xilem, or Floem.
- **[flux](https://github.com/elcoosp/flux)** — Write-once UI language for native iOS & Android. Hot-reload as binary IR patches over WebSocket; release builds compile to SwiftUI & Jetpack Compose. **16 crates · ~63k LOC Rust · 39 ADRs**; Astro Starlight docs site scaffolded.
- **[alacer](https://github.com/elcoosp/alacer)** — Retained-mode Rust GUI framework with accessibility built in. Only dirty subtrees relayout or repaint. M9 windowed a11y scope: 47-case corpus, a11y-ratio budget, action tier in the dispatch contract.
- **[aeolus](https://github.com/elcoosp/aeolus)** — Tailwind CSS v4 class strings compiled to native properties for Xilem/Masonry, Floem, Iced, egui, and Slint. No Node, no CSS build step. v0.8 merged; v0.9 variant & grid engine planned.
- **[tuvix](https://github.com/elcoosp/tuvix)** — Terminal UI framework where input preempts rendering. Budgeted frames, zero-alloc diffing, built-in time-travel debugging. M18 adds `SurfaceStack` floating-surface routing.
- **[nexum](https://github.com/elcoosp/nexum)** — Framework-agnostic deep linking for Rust desktop apps. Custom URL schemes and OAuth callbacks across Windows, macOS, Linux, Android, and iOS.

### Developer Tools & Systems

- **[kod](https://github.com/elcoosp/kod)** — Local-first AI coding-agent harness (TUI + CLI). Streaming agentic loop, multi-agent swarm, MCP & LSP clients, sandboxed shell. **v0.1.28 · 20 crates · ~4000 tests**; auto-regenerated changelog pipeline.
- **[wraith](https://github.com/elcoosp/wraith)** — High-performance in-memory PNG → optimised SVG vectorizer. v0.2.0 adds a sub-pixel geometric colour engine, redesigned settings, and a ground-truth quality harness gated in CI.
- **[magnetite](https://github.com/elcoosp/magnetite)** — Zero-copy BitTorrent metadata toolkit. v0.2.0 ships the BEP 15 UDP tracker client, span-tracking bencode decoder, and raw-slice infohash derivation. No `unsafe`, no async runtime.
- **[pkr-sota](https://github.com/elcoosp/pkr-sota)** — End-to-end heads-up NLHE poker AI in Rust. CFR blueprint training, `mmap` runtime, nanosecond lookups. **p50 ≈ 42 ns · 460+ tests**

### Applications & Platforms

- **[vautr](https://github.com/elcoosp/vautr)** — Zero-knowledge password manager: OPAQUE authentication + Argon2id, offline-first sync. **Rust core · React / Expo / GPUI clients · AGPL**
- **[stackbluff](https://github.com/elcoosp/stackbluff)** — Multiplayer poker platform: sub-10ms Rust engine, AI coach, bots, anti-cheat, clubs & tournaments, Stripe billing.
- **[takumi-motion](https://github.com/elcoosp/takumi-motion)** — Deterministic server-side animation engine rendering React components or HTML to GIF, WebP, or APNG.

---

## Created in November 2026

Repositories created between **Nov 3–7, 2026**, per the public activity feed:

**Compilers & parsing** — `ligature` · `zsx` · `syntact`
**GUI & native UI** — `alacer` · `aeolus` · `guiwright`
**Systems & tooling** — `magnetite` · `wraith` · `upd`
**Other** — `starlight` · `catheo` · `tuvix` · `peregrine` · `gpui-rsx` · `leptos-shadcn-ui`

All public and active as of **Nov 8, 2026**.

---

## How I Work

- **Spec before code** — `flux` carries 39 MADR ADRs plus a full wire-protocol & VM-ISA spec; `kod` ships SPEC, ARCHITECTURE and TESTING documents; `oxide` maintains strict spec-vs-code deviation docs.
- **Tests are the design review** — `cargo-nextest`, `proptest`, `insta` snapshots, `criterion` performance budgets (`parse < 5 ms`, `diff < 1 ms`, `VM eval < 2 ms`); ~4000 tests across `kod`'s crates; Miri-clean core crates in `pkr-sota`.
- **CI like it's production** — clippy `-D warnings`, `#![forbid(unsafe_code)]` in every library crate, fuzzed wire protocol, mutation testing, parity harnesses, golden-hash and allocation-budget CI gates (`dhat` in `syntact`), metrics ratchets (`glyim`).
- **AI-augmented, engineer-owned** — I ship daily with AI & MCP, and I built my own harness (`kod`) to keep the loop local, sandboxed, and auditable.

---

## Currently (November 2026)

- **glyim** — Readiness ledger v1 foundation landed (M1.1 schema + check). New `glyim-metrics` crate with a TDD ratchet, plus a dedicated CI metrics-ratchet job and PR body. M0 pedantic lint/doc pass across the tool crates, M0.6 baseline recorded, stable toolchain pinned for local dev, session handoffs archived.
- **oxide** — F04 substrate milestone closed: experiments config section types with DSP-110 validation, the §15.4 assignment engine in dispatch, criterion benches for assign/resolve, and `blake3` added for the engine. Workspace lints policy adopted pedantic across the config crate; checked-in config schema regenerated; worklog, deviations and handoff docs appended.
- **pkr-sota** — Runtime correctness sweep: session shadow/gadget routing, mmap ordering warning, masked ranges, bot-pipe contract. Export gains v2 anchor offsets, deterministic FMph and directory fsync; exploit evaluation decorrelates seeds with CRN for LBR; core gets a short all-in guard and uncalled-bet return. FNV-1a known-answer vectors added, fuzz seeds domain-separated, scripts made portable (signal forwarding to the process group, per-version lock), scattered docs synthesized into ARCHITECTURE / STATUS / HISTORY.
- **kod** — v0.1.28 shipped (162 commits since v0.1.27): clippy warning cleanup campaign, MSRV bump, LICENSE normalization, publish workflow. Changelog workflow rewritten to prepend only the new release and auto-regenerate on tag push. README command list, test count, minisign reference and site version corrected; stale docs removed.
- **ligature** — M10 per-mount identity and branch-time assembly merged. M9 delivery report and ADR-022 for component-in-content and nested outlets; `slots-component` and `slots-nested` fixtures with canonical IR for both Solid and Vue inputs; `codegen_composed` budget ceiling registered in the CLI ledger.
- **syntact** — Pack LSP epic (issue 042) closed: pack registry, document model with prebuilt view caches, positioned tree-index outline builder, state-machine dispatch, stdio loop generalized over a `Handler` trait, and a `pack-lsp` CLI subcommand. Dhat allocation budget gates and editor-facing hot-path benchmarks added; the pack LSP book chapter authored. The grammar→descriptor compiler (`descent-lower`) landed.
- **zsx** — DVUI playground stabilized: scrollArea wrapper, window sizing for large displays, skeleton margin/background fixes, corner-radius handling. Snapshot tests write to `docs/screenshots` with the corrected `@TypeOf(.enum_literal)` logFn signature and auto-downscaling. Nanoui 15-component playground render captured; DX docs rewritten for the v0.1.0 single-pipeline reality.
- **alacer** — M9 windowed accessibility: selection model joins the editing and a11y contracts, action tier joins the dispatch contract (ADR-0016); windowed path drains the pipeline's own sink; 47-case corpus with an a11y-ratio budget; 32 blessed PNGs across the two suites; frame-batched input queue documented (ADR-0015).
- **aeolus** — v0.9 variant & grid engine plan filed; variant engine documented beside the set-mask; RED-to-GREEN and test-pyramid hardening records written. v0.8 merged (set-mask + variant engine + pyramid); shadcn oracle-fidelity ledger pinned; process-level CLI end-to-end suite; snapshot header and set-mask round-trip re-pinned at schema v3.
- **tuvix** — M18 `SurfaceStack` floating-surface routing plus the B21 stacked-composite bench; M17 dropdown composite (`dropdown_rows`) with the B20 gate; L5/L6 surface-stack benches. `memgate` realloc delta sign fixed so shrinks release bytes; repository metadata corrected.
- **nexum** — Platform target-gating sweep across unix paths, macOS targets, and Xilem/Leptos/Dioxus/Floem registration tests; MSRV bumped to 1.86; `cargo-deny` licenses extended for the quick-xml advisory; `libxdo-dev` added to CI; internal doc link paths corrected.
- **magnetite** — v0.2.0: BEP 15 UDP tracker client with compact peers, span-tracking bencode decoder, and raw-slice infohash derivation; tracker packet proptests and benchmarks; error taxonomy gains a `Tracker` variant.
- **wraith** — v0.2.0: sub-pixel geometric colour engine (M1–M5), settings redesigned into engine/color/background with alpha as a first-class background policy, ground-truth quality harness with a CI baseline gate, palette and path counts in reports, CLI presets exposed.
- **flux** — Astro Starlight docs site scaffolded: homepage, first-app tutorials, 11 how-to guides, 7 API reference pages, 5 explanation pages, plus docs-site ADRs. ISA vector cleanup moved list insert/remove to literal-index bytecode and dropped the reverted NaN and register-index vectors; iOS host reverts (component-name wiring, FLUX-066 perf harness, snapshot full store).

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

**Rust ecosystem, in anger:** `tokio` · `axum` · `clap` · `ratatui` · `redb` · `blake3` · `MessagePack` · `proptest` · `insta` · `criterion` · `cargo-nextest` · `dhat` · `OpenTelemetry` · `hyper` · `rustls` · `Oxc` · `Rolldown`
