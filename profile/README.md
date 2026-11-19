<p align="left">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://nikrun.dev/brand/nikrun-lockup-dark-mono.svg">
    <img alt="Nikrun" src="https://nikrun.dev/brand/nikrun-lockup-light.svg" height="52">
  </picture>
</p>

[![nik CLI Build](https://github.com/nikrun/cli/actions/workflows/build.yml/badge.svg)](https://github.com/nikrun/cli/actions/workflows/build.yml)
[![Free Pascal SDKs](https://github.com/nikrun/sdk/actions/workflows/build-fpc-sdk.yml/badge.svg)](https://github.com/nikrun/sdk/actions/workflows/build-fpc-sdk.yml)
[![License: GPL-3.0-or-later](https://img.shields.io/badge/license-GPL--3.0--or--later-blue.svg)](https://github.com/nikrun/cli/blob/main/LICENSE)
[![Website: nikrun.dev](https://img.shields.io/badge/website-nikrun.dev-0b0e14)](https://nikrun.dev)

> **Modern, zero-config toolchain for Free Pascal.**

[nikrun.dev](https://nikrun.dev) · [Documentation](https://nikrun.dev/docs/) · [`nik` CLI](https://github.com/nikrun/cli) · [Free Pascal SDKs](https://github.com/nikrun/sdk) · [VS Code Extension](https://github.com/nikrun/vscode) · [GitHub Action](https://github.com/nikrun/github-setup-nik) · [Example Project](https://github.com/nikrun/github-example)

---

**Nikrun** *(named in tribute to [Niklaus Wirth](https://en.wikipedia.org/wiki/Niklaus_Wirth))* brings the cohesive workflow of modern ecosystems like Rust (`rustup` + `cargo`) and Go to **Free Pascal & Object Pascal**. At its core sits the standalone **`nik` CLI** — a single dependency-free native binary uniting portable multi-arch compiler SDKs, declarative `nik.yaml` builds, decentralized `nik.lock` packages, and a built-in Language Server (`nik lsp`) strictly in user scope (`~/.nikrun`).

- **100% User Scope (`~/.nikrun`):** Zero administrator or root privileges, zero global `PATH` collisions, and zero broken system-wide `/etc/fpc.cfg` files.
- **Instant Multi-Version & Multi-Arch SDKs:** Run Free Pascal `3.2.2`, `3.2.4`, `fixes_3_2`, and nightly `3.3.1` side by side in seconds across Windows, Linux, and macOS (`x86_64` & `aarch64`, including native Windows ARM64).
- **Declarative `nik.yaml` & `nik.lock`:** One clean manifest for programs, shared libraries, and packages — with profiles, OS/CPU overlays, and SHA-256 lockfile-pinned dependencies.
- **Zero-Config `nik lsp` & VS Code:** Live Free Pascal compiler diagnostics on unsaved buffers, `Go to Definition` deep into bundled RTL sources, and status-bar SDK/profile switchers via **Nikrun for VS Code** (`nikrun.vscode`).
- **Built for CI/CD & AI Agents:** Deterministic `--json` diagnostics, automatic `CI`/`NO_COLOR` detection, and worktree-safe checkout caches (`.nik/cache/`).

---

### Quick Install & 60-Second Workflow

**Windows (PowerShell):**
```powershell
irm https://nikrun.dev/install.ps1 | iex
```

**Linux & macOS:**
```bash
curl -fsSL https://nikrun.dev/install.sh | bash
```

**Scaffold & compile a native executable:**
```bash
nik init hello-nikrun          # Scaffold project & declarative nik.yaml manifest
cd hello-nikrun
nik build -p release           # Auto-install pinned Free Pascal SDK & compile optimized binary
./bin/hello-nikrun             # Run compiled native executable
```

---

### Ecosystem Repositories

| Repository | Description |
| :--- | :--- |
| **[`nikrun/cli`](https://github.com/nikrun/cli)** | **Nikrun CLI (`nik`)** — Standalone native toolchain, SDK manager, `nik.yaml` build system, package manager, and `nik lsp` for Free Pascal. |
| **[`nikrun/sdk`](https://github.com/nikrun/sdk)** | **Nikrun SDKs** — Automated, SHA-256-verified portable Free Pascal toolchains (`3.2.2`–`3.3.1`) for Windows, Linux, and macOS (`x86_64` & `aarch64`). |
| **[`nikrun/vscode`](https://github.com/nikrun/vscode)** | **Nikrun for VS Code** — Official Visual Studio Code extension (`nikrun.vscode`) powered by `nik lsp`. |
| **[`nikrun/github-setup-nik`](https://github.com/nikrun/github-setup-nik)** | **Nikrun GitHub Action** — Official GitHub Action (`uses: nikrun/github-setup-nik@v1`) for Free Pascal & Object Pascal CI workflows. |
| **[`nikrun/github-example`](https://github.com/nikrun/github-example)** | **Nikrun GitHub Example** — Minimal cross-platform Free Pascal & Object Pascal starter with a 6-target GitHub Actions matrix workflow. |
| **[`nikrun/web`](https://github.com/nikrun/web)** | **Nikrun Website & Docs** — Official [nikrun.dev](https://nikrun.dev) landing page, documentation, and CLI installer endpoints. |
| **[`nikrun/brand`](https://github.com/nikrun/brand)** | **Nikrun Brand Assets** — Canonical vector marks, lockups, application icons, favicons, and social preview cards. |
| **[`nikrun/build-lib`](https://github.com/nikrun/build-lib)** | **Nikrun Build Library** — Shared PowerShell build, packaging, SBOM, and release automation across Nikrun repositories. |
