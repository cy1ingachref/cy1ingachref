![](https://img.shields.io/badge/Cybersecurity_%26_DevSecOps-Student-no?style=flat&logo=shield&logoColor=white&color=4d7cff)
![](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)
![](https://img.shields.io/badge/GitHub_Actions-CI-green?style=flat&logo=github-actions&logoColor=white)

---

**Achref Ferjani** — Cybersecurity & DevSecOps engineering student. I build security tooling that ships with tests.

A portfolio of security engineering projects. Offensive (recon, detection, authorized red-team) and defensive (SOC rules, CI/CD gating, vuln autograding). Each repo has its own README, requirements, and CI — click through for details.

## Projects

| # | Repo | What it does |
|---|------|-------------|
| 01 | [`01-devsecops-pipeline`](https://github.com/cy1ingachref/01-devsecops-pipeline) | DevSecOps CI/CD pipeline as code — GitHub Actions + Semgrep + gitleaks + Trivy + tfsec, with a cross-project JWT gate |
| 02 | [`02-jwt-audit-tool`](https://github.com/cy1ingachref/02-jwt-audit-tool) | JWT security audit CLI — alg:none, weak secrets, expiry abuse, audience/issuer validation gaps |
| 03 | [`03-cloud-soc-detection-lab`](https://github.com/cy1ingachref/03-cloud-soc-detection-lab) | Cloud SOC detection lab — simulate atomic attacks, run detection rules, verify alerts fire |
| 04 | [`04-vuln-app-autograder`](https://github.com/cy1ingachref/04-vuln-app-autograder) | Vulnerability app autograder — OWASP Top 10 checks against a target app, scored report |
| 05 | [`05-purple-team-gym`](https://github.com/cy1ingachref/05-purple-team-gym) | Purple-team exercise gym — simulated attacker/defender loops with a live dashboard |

## Other public repos

- **`netmon-lan-monitor`** — Cyberpunk LAN monitor + blue/red defense console (Windows-first). Packet scan, MAC-primary device recognition, gated ARP-spoof. 45/45 tests.
- **`sigma-lab`** — Sigma detection lab: 4 rules + green-check harness.
- **`bcrypt-5digit-cracker`** — Educational demo: brute-force a bcrypt hash to recover a 5-digit PIN. In-browser + Python CLI.
- **`tn-watch`** — Zero-dependency change/digest monitor (RSS/JSON/HTML) with dedupe.
- **`jarvis-spatial`** — JARVIS holographic spatial interface: webcam hand control + real object identification (COCO-SSD) rendered as controllable 3D proxies.
- **`one-mind`** — Shared memory layer for AI agents. SQLite + HTTP daemon + MCP server, BM25 retrieval, provenance, garbage collection. 40+ tests.
- **`evidence-guardian`** — AI-native security research framework. Every finding carries a reproducible evidence chain. No proof, no claim.
- **`mastermind`** — Multi-agent orchestration. Pick a lead AI to decompose tasks, delegate, and aggregate results.
- **`applied-ml`** — Curated papers & tech blogs from companies on ML in production.

## Stack

Python, GitHub Actions, Semgrep, Trivy, tfsec, gitleaks, Sigma, SQLite, WebSocket, COCO-SSD/MediaPipe, BM25. Zero-dep where practical.

## License

MIT unless a repo states otherwise.

---

*Built Sep 2026. Portfolio grows as I do.*
