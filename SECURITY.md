# Security Policy

## Reporting a Vulnerability

Please **do not** report security vulnerabilities through public GitHub issues, discussions, or pull requests.

Instead, report suspected vulnerabilities privately through GitHub's built-in **[Private Vulnerability Reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)** in the affected **Nikrun** repository (`Security` -> `Report a vulnerability`):

- **[`nikrun/cli`](https://github.com/nikrun/cli/security/advisories/new)** — `nik` CLI binary, archive extraction, SHA-256 verification, package fetching, and `nik lsp`
- **[`nikrun/sdk`](https://github.com/nikrun/sdk/security/advisories/new)** — Portable Free Pascal SDK build pipelines and `index.json` release artifacts
- **[`nikrun/vscode`](https://github.com/nikrun/vscode/security/advisories/new)** — **Nikrun for VS Code** (`nikrun.vscode`) extension
- **[`nikrun/github-setup-nik`](https://github.com/nikrun/github-setup-nik/security/advisories/new)** — GitHub Action (`nikrun/github-setup-nik`)
- **[`nikrun/web`](https://github.com/nikrun/web/security/advisories/new)** — [nikrun.dev](https://nikrun.dev) website and `install.ps1` / `install.sh` bootstrap scripts

When submitting a report, please include:

1. Affected component, version (e.g., `nik --version`), and operating system / architecture.
2. Minimal steps or `nik.yaml` manifest required to reproduce the issue.
3. Expected security impact.

We aim to acknowledge new reports within **72 hours** and coordinate remediation before public disclosure.
