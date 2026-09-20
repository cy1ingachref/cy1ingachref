<img src="assets/banner.svg" alt="Achref Ferjani  DevOps, DevSecOps, Software Engineering" width="100%">

Student at **ISSATM Bizerte, Tunisia**. I build and harden automated systems — CI/CD pipelines that catch vulnerabilities before merge, detection rules that fire on real attacks, and Python infrastructure that multiple agents share.

Looking for opportunities in DevOps, DevSecOps, or software engineering roles.

---

## Featured projects

### 01-devsecops-pipeline — DevSecOps CI/CD as code

[![CI](https://github.com/cy1ingachref/01-devsecops-pipeline/actions/workflows/security.yml/badge.svg)](https://github.com/cy1ingachref/01-devsecops-pipeline/actions/workflows/security.yml)

A full CI/CD security pipeline that runs on every push and pull request. Gitleaks catches leaked secrets, Semgrep finds SAST issues, Trivy scans container images and filesystems for CVEs, and tfsec checks Terraform for misconfigurations — all before code reaches production. A consolidated dashboard gives a single view across all tools.

The pipeline includes a cross-project JWT gate: it invokes the 02-jwt-audit-tool on a weak sample token and fails the build if the HIGH finding isn't caught. This proves the scanner and the pipeline work together, not in isolation.

Built with GitHub Actions, Docker, and Python. Zero external dependencies where practical.

[→ Repo](https://github.com/cy1ingachref/01-devsecops-pipeline) · [README](https://github.com/cy1ingachref/01-devsecops-pipeline/blob/main/README.md)

---

### evidence-guardian — AI-native security research framework

[![CI](https://github.com/cy1ingachref/evidence-guardian/actions/workflows/ci.yml/badge.svg)](https://github.com/cy1ingachref/evidence-guardian/actions/workflows/ci.yml) &nbsp; [![Tests](https://img.shields.io/badge/tests-17%20passed-brightgreen)](https://github.com/cy1ingachref/evidence-guardian) &nbsp; [![OmniRoute](https://img.shields.io/badge/AI-9%20free%20providers-ff69b4)](https://github.com/cy1ingachref/evidence-guardian)

Most AI security tools hallucinate findings with no proof. evidence-guardian takes a different approach: **every finding must carry verifiable evidence. No proof, no claim.**

Point it at a web app and it scans for SSRF, IDOR, XSS, SQL injection, open redirect, sensitive data exposure, misconfiguration, and more. For each finding it autonomously generates working proofs — actual HTTP request/response pairs, PoC scripts, and self-contained evidence bundles you can hand to a developer or include in a report.

OmniRoute routes LLM requests across 9 free AI providers (Ollama, Groq, Nous, Together, OpenRouter, Fireworks, Mistral, DeepInfra, HuggingFace) with automatic failover. No paid APIs required.

17 tests passed. MIT licensed.

[→ Repo](https://github.com/cy1ingachref/evidence-guardian) · [README](https://github.com/cy1ingachref/evidence-guardian/blob/main/README.md)

---

### one-mind — Shared memory layer for AI agents

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/) &nbsp; [![SQLite](https://img.shields.io/badge/SQLite-embedded-FFCC00?style=flat&logo=sqlite&logoColor=black)](https://www.sqlite.org/) &nbsp; [![MCP](https://img.shields.io/badge/MCP-server-8957E9?style=flat&logo=anthropic&logoColor=white)](https://modelcontextprotocol.io/)

A shared memory layer that lets multiple AI agents on the same project share context across sessions. Each agent writes and reads from a common SQLite store, with BM25-ranked retrieval so relevant past context surfaces automatically. Every entry carries provenance (which agent wrote it), TTL-based expiry, and garbage collection so the store stays clean.

Pluggable architecture: SDK for Python, CLI for interactive use, MCP server for LLM tool integration, and a threaded daemon mode for background operation. Zero external dependencies — stdlib and SQLite only.

53 tests across 2 test files. No CI workflow configured yet — planned on the roadmap.

[→ Repo](https://github.com/cy1ingachref/one-mind) · [README](https://github.com/cy1ingachref/one-mind/blob/main/README.md)

---

## All projects

<details>
<summary>Click to expand — 8 more projects</summary>

| Project | Track | What it does | CI |
|---------|-------|-------------|-----|
| [**02-jwt-audit-tool**](https://github.com/cy1ingachref/02-jwt-audit-tool) | DevSecOps | JWT security audit CLI — detects alg:none, cracks weak HMAC secrets, tests expiry abuse, validates audience/issuer claims. Exit codes designed for CI gate integration. | [test-ci.yml](https://github.com/cy1ingachref/02-jwt-audit-tool/actions/workflows/test-ci.yml/badge.svg) |
| [**03-cloud-soc-detection-lab**](https://github.com/cy1ingachref/03-cloud-soc-detection-lab) | DevSecOps | Cloud SOC detection lab — simulate atomic attacks (auth brute-force, impossible travel), run Sigma detection rules, verify alerts fire with proof. Docker Compose + Python. | [ci.yml](https://github.com/cy1ingachref/03-cloud-soc-detection-lab/actions/workflows/ci.yml/badge.svg) |
| [**04-vuln-app-autograder**](https://github.com/cy1ingachref/04-vuln-app-autograder) | DevSecOps | Vulnerability app autograder — runs OWASP Top 10 checks against a target application and produces a scored report. Built for grading student apps and self-assessment. | — |
| [**05-purple-team-gym**](https://github.com/cy1ingachref/05-purple-team-gym) | DevSecOps | Purple-team simulation — an adaptive RED attacker and BLUE defender coevolve over 200 rounds, learning against each other until measurable equilibrium. Live posture dashboard. | [ci.yml](https://github.com/cy1ingachref/05-purple-team-gym/actions/workflows/ci.yml/badge.svg) |
| [**sigma-lab**](https://github.com/cy1ingachref/sigma-lab) | DevSecOps | Sigma detection lab — 4 detection rules (auth brute-force, impossible travel, SSRF probe, data exfiltration) with a green-check harness that proves each rule fires against real simulation data. | [test.yml](https://github.com/cy1ingachref/sigma-lab/actions/workflows/test.yml/badge.svg) |
| [**mastermind**](https://github.com/cy1ingachref/mastermind) | SWE | Multi-agent orchestration — a lead AI decomposes a task, delegates to worker agents, and aggregates results. Built for coordinating multiple LLMs on a single complex workflow. | — |
| [**bcrypt-5digit-cracker**](https://github.com/cy1ingachref/bcrypt-5digit-cracker) | SWE | Educational security demo — brute-force a bcrypt hash to recover a 5-digit numeric PIN. Web Worker-based in-browser cracker + Python CLI. Clean architecture, tested. | [ci.yml](https://github.com/cy1ingachref/bcrypt-5digit-cracker/actions/workflows/ci.yml/badge.svg) |
| [**netmon-lan-monitor**](https://github.com/cy1ingachref/netmon-lan-monitor) | DevOps | LAN monitor + blue/red defense console (Windows-first). Continuous packet capture, MAC-primary device recognition, authorized ARP-spoof for red-team exercises. 45 tests. | [ci.yml](https://github.com/cy1ingachref/netmon-lan-monitor/actions/workflows/ci.yml/badge.svg) |
| [**tn-watch**](https://github.com/cy1ingachref/tn-watch) | DevOps | Zero-dependency change/digest monitor for RSS, JSON, and HTML feeds. Deduplicates and reports diffs. Clean Python CLI designed for cron and scripting — no external packages. | [ci.yml](https://github.com/cy1ingachref/tn-watch/actions/workflows/ci.yml/badge.svg) |

</details>

---

## Stack

**Languages:** Python (primary), Shell, JavaScript, HTML/CSS, YAML, SQL

**DevOps:** GitHub Actions, Docker, Semgrep, Trivy, tfsec, gitleaks, Sigma

**Security:** OWASP Top 10, JWT analysis, SSRF/IDOR/XSS/SQLi detection, ARP networking, authorized red-team, detection engineering

**Infrastructure:** SQLite, HTTP daemons, MCP servers, BM25 retrieval, WebSocket, Web Workers

**Practices:** Test-driven development, CI-gated workflows, evidence-backed findings, zero-dependency where practical, MIT licensing

---

## About

- **Education:** ISSATM Bizerte, Tunisia
- **Background:** Authorized pentest internship at E-Tafakna (legal-tech SaaS), where I found bugs in a production application and wrote the report. That experience shaped the security projects here — every tool is something I wished I had during that internship.
- **Approach:** Build things that work, prove they work with tests, document how to use them. No "trust me bro" security — every finding in evidence-guardian carries a reproducible evidence chain.

---

## Connect

- GitHub: [@cy1ingachref](https://github.com/cy1ingachref)
- Email: cy1ingachref@gmail.com
- LinkedIn: https://www.linkedin.com/in/achref-ferjani-480a90355/
- Location: Tunisia
- Available for: DevOps, DevSecOps, and Software Engineering roles

---

*Portfolio updated September 2026. Built and maintained with CI, tests, and honest documentation.*
