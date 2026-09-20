![](https://img.shields.io/badge/DevOps-CI/CD%2C+IaC%2C+Observability-0097FF?style=flat&logo=github-actions&logoColor=white&color=0097FF)
![](https://img.shields.io/badge/DevSecOps-OMG%2C+Detection%2C+Pentest-FF4500?style=flat&logo=shield&logoColor=white&color=FF4500)
![](https://img.shields.io/badge/SWE-Python%2C+Testing%2C+Architecture-3776AB?style=flat&logo=python&logoColor=white&color=3776AB)
![](https://img.shields.io/badge/Student-ISSATM+Bizerte-888?style=flat&logo=school&logoColor=white)

---

# Achref Ferjani

**DevOps  •  DevSecOps  •  Software Engineering**

I build and harden automated systems — CI/CD pipelines that catch vulnerabilities before merge, detection rules that fire on real attacks, and Python infrastructure that multiple agents share. Student at **ISSATM Bizerte, Tunisia**.

Looking for opportunities in DevOps, DevSecOps, or software engineering roles.

---

## How to read this profile

My work spans three tracks. Each has its own project table below — click through for READMEs, tests, and CI status.

| Track | What I do | Proof |
|-------|-----------|-------|
| **DevOps** | CI/CD as code, IaC scanning, monitoring tooling, zero-dep utilities | green CI badges, test suites |
| **DevSecOps** | Pipeline security gates, JWT auditing, SOC detection, vuln autograding, purple-team exercises | live alerts, scored reports, OWASP coverage |
| **Software Engineering** | Python systems with clean architecture, pluggable designs, test-first development | 40+ test suites, documented APIs, real users |

---

## DevOps

*Pipelines, infrastructure, observability, and the tooling that keeps systems running.*

| Project | What it does | Tech |
|---------|-------------|------|
| [**01-devsecops-pipeline**](https://github.com/cy1ingachref/01-devsecops-pipeline) | Full CI/CD security pipeline as code — Gitleaks, Semgrep, Trivy, tfsec on every push/PR. Includes a cross-project JWT gate that proves the pipeline and auditor work together. | GitHub Actions, Docker, Semgrep, Trivy, tfsec, gitleaks |
| [**tn-watch**](https://github.com/cy1ingachref/tn-watch) | Zero-dependency change/digest monitor for RSS, JSON, and HTML feeds. Dedupe + green-check reporting. Built for scripting and cron. | Python, zero deps |
| [**one-mind**](https://github.com/cy1ingachref/one-mind) | Shared memory layer for AI agents — SQLite + threaded HTTP daemon + MCP server. BM25 retrieval, provenance tracking, garbage collection. Multiple agents on one project share context across sessions. | Python, SQLite, MCP, BM25, 40+ tests |

---

## DevSecOps

*Security scanning, detection engineering, authorized testing, and proving vulnerabilities with evidence.*

| Project | What it does | Tech |
|---------|-------------|------|
| [**evidence-guardian**](https://github.com/cy1ingachref/evidence-guardian) | AI-native security research framework. Scans web apps for SSRF, IDOR, XSS, SQLi, open redirect, sensitive data, misconfiguration, and more. Every finding carries a reproducible evidence chain — HTTP request/response pairs, PoC scripts, self-contained HTML reports. OmniRoute routes across 9 free AI providers with failover. | Python, 9 AI providers, 17 tests |
| [**01-devsecops-pipeline**](https://github.com/cy1ingachref/01-devsecops-pipeline) | CI/CD security pipeline with a cross-project JWT gate — the same pipeline that scans for secrets and CVEs also runs the JWT auditor on a weak sample token and fails the build if the HIGH finding isn't caught. | GitHub Actions, JWT audit integration |
| [**02-jwt-audit-tool**](https://github.com/cy1ingachref/02-jwt-audit-tool) | JWT security audit CLI — detects alg:none attacks, cracks weak secrets, tests expiry abuse, validates audience/issuer claims. Exit codes integrate into CI gates. | Python, PyJWT |
| [**03-cloud-soc-detection-lab**](https://github.com/cy1ingachref/03-cloud-soc-detection-lab) | Cloud SOC detection lab — simulate atomic attacks (brute-force, impossible travel), run detection rules, verify alerts fire with live proof. | Python, Sigma rules, Docker |
| [**04-vuln-app-autograder**](https://github.com/cy1ingachref/04-vuln-app-autograder) | Vulnerability app autograder — runs OWASP Top 10 checks against a target application and produces a scored report. Built for grading student apps and self-assessment. | Python, OWASP Top 10 |
| [**05-purple-team-gym**](https://github.com/cy1ingachref/05-purple-team-gym) | Purple-team exercise gym — simulated attacker/defender loops with a live dashboard showing posture scores and technique coverage. | Python, HTML dashboard |
| [**sigma-lab**](https://github.com/cy1ingachref/sigma-lab) | Sigma detection lab — 4 detection rules (auth brute-force, impossible travel, SSRF, data exfiltration) with a green-check harness that proves each rule fires. | Sigma, Python, YAML |
| [**netmon-lan-monitor**](https://github.com/cy1ingachref/netmon-lan-monitor) | Cyberpunk LAN monitor + blue/red defense console (Windows-first). Continuous packet scan, MAC-primary device recognition, gated whole-LAN ARP-spoof for authorized red-team exercises. 45/45 tests. | Python, scapy, Windows |

---

## Software Engineering

*Clean, tested Python systems — pluggable architectures, shared infrastructure, and tools built to be used.*

| Project | What it does | Tech |
|---------|-------------|------|
| [**one-mind**](https://github.com/cy1ingachref/one-mind) | Shared memory layer for AI agents — pluggable architecture with SDK, CLI, MCP server, and daemon mode. BM25 retrieval, TTL-based expiry, provenance (agent_id), garbage collection. Zero external dependencies. | Python, SQLite, MCP, BM25, 40+ tests |
| [**mastermind**](https://github.com/cy1ingachref/mastermind) | Multi-agent orchestration — pick a lead AI to decompose tasks, delegate to other agents, and aggregate results. Built for coordinating multiple AI agents on a single workflow. | Python |
| [**bcrypt-5digit-cracker**](https://github.com/cy1ingachref/bcrypt-5digit-cracker) | Educational demo — brute-force a bcrypt hash to recover a 5-digit numeric PIN. Includes both a working in-browser cracker (Web Worker) and a Python CLI. Clean separation of concerns, tested. | Python, JavaScript, Web Workers |
| [**netmon-lan-monitor**](https://github.com/cy1ingachref/netmon-lan-monitor) | Production-grade LAN monitor — continuous packet capture, MAC-primary device recognition, ARP-spoof capability gated behind authorization checks. Windows-first, 45/45 tests, real-world red-team/bule-team use. | Python, scapy, Windows API |
| [**tn-watch**](https://github.com/cy1ingachref/tn-watch) | Zero-dependency monitoring utility — watches RSS, JSON, and HTML endpoints for changes, deduplicates, and reports. Built as a clean Python CLI with no external packages. | Python, zero deps |

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
- Location: Tunisia
- Available for: DevOps, DevSecOps, and Software Engineering roles

---

*Portfolio updated September 2026. Built and maintained with CI, tests, and honest documentation.*
