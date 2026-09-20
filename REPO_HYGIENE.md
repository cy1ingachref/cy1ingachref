REPO HYGIENE SUGGESTIONS
=========================

Topics to add (run with `gh repo edit --add-topic`):

  # evidence-guardian
  gh repo edit cy1ingachref/evidence-guardian --add-topic devsecops
  gh repo edit cy1ingachref/evidence-guardian --add-topic security-automation
  gh repo edit cy1ingachref/evidence-guardian --add-topic vulnerability-scanning
  gh repo edit cy1ingachref/evidence-guardian --add-topic ai-security
  gh repo edit cy1ingachref/evidence-guardian --add-topic pentest
  gh repo edit cy1ingachref/evidence-guardian --add-topic owasp

  # 01-devsecops-pipeline
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic devsecops
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic ci-cd
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic github-actions
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic devops
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic security-automation
  gh repo edit cy1ingachref/01-devsecops-pipeline --add-topic iac-scanning

  # one-mind
  gh repo edit cy1ingachref/one-mind --add-topic python
  gh repo edit cy1ingachref/one-mind --add-topic agent-infrastructure
  gh repo edit cy1ingachref/one-mind --add-topic mcp
  gh repo edit cy1ingachref/one-mind --add-topic memory-layer
  gh repo edit cy1ingachref/one-mind --add-topic bm25
  gh repo edit cy1ingachref/one-mind --add-topic sqlite

  # mastermind
  gh repo edit cy1ingachref/mastermind --add-topic multi-agent
  gh repo edit cy1ingachref/mastermind --add-topic agent-orchestration
  gh repo edit cy1ingachref/mastermind --add-topic python
  gh repo edit cy1ingachref/mastermind --add-topic ai

  # 02-jwt-audit-tool
  gh repo edit cy1ingachref/02-jwt-audit-tool --add-topic devsecops
  gh repo edit cy1ingachref/02-jwt-audit-tool --add-topic jwt
  gh repo edit cy1ingachref/02-jwt-audit-tool --add-topic api-security
  gh repo edit cy1ingachref/02-jwt-audit-tool --add-topic authentication

  # 03-cloud-soc-detection-lab
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab --add-topic devsecops
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab --add-topic soc
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab --add-topic detection-engineering
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab --add-topic sigma
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab --add-topic cloud-security

  # sigma-lab
  gh repo edit cy1ingachref/sigma-lab --add-topic sigma
  gh repo edit cy1ingachref/sigma-lab --add-topic detection-engineering
  gh repo edit cy1ingachref/sigma-lab --add-topic soc
  gh repo edit cy1ingachref/sigma-lab --add-topic siem

  # 05-purple-team-gym
  gh repo edit cy1ingachref/05-purple-team-gym --add-topic purple-team
  gh repo edit cy1ingachref/05-purple-team-gym --add-topic devsecops
  gh repo edit cy1ingachref/05-purple-team-gym --add-topic mitre-attack
  gh repo edit cy1ingachref/05-purple-team-gym --add-topic security-training

  # netmon-lan-monitor
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic network-monitoring
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic blue-team
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic red-team
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic network-security
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic windows
  gh repo edit cy1ingachref/netmon-lan-monitor --add-topic python

  # tn-watch
  gh repo edit cy1ingachref/tn-watch --add-topic monitoring
  gh repo edit cy1ingachref/tn-watch --add-topic cli
  gh repo edit cy1ingachref/tn-watch --add-topic python
  gh repo edit cy1ingachref/tn-watch --add-topic zero-dependency
  gh repo edit cy1ingachref/tn-watch --add-topic cron

  # bcrypt-5digit-cracker
  gh repo edit cy1ingachref/bcrypt-5digit-cracker --add-topic security-demo
  gh repo edit cy1ingachref/bcrypt-5digit-cracker --add-topic python
  gh repo edit cy1ingachref/bcrypt-5digit-cracker --add-topic education

First-line descriptions to improve (run with `gh repo edit --description`):

  # one-mind — add test count + architecture signal
  gh repo edit cy1ingachref/one-mind \
    --description "Shared memory layer for AI agents — SQLite + MCP server + BM25 retrieval. 53 tests, zero external deps, pluggable architecture."

  # 05-purple-team-gym — add coevolution detail
  gh repo edit cy1ingachref/05-purple-team-gym \
    --description "Purple-team coevolution gym — adaptive RED attacker vs BLUE defender over 200 rounds. Live posture dashboard, 23 tests."

  # 03-cloud-soc-detection-lab — add Sigma detail
  gh repo edit cy1ingachref/03-cloud-soc-detection-lab \
    --description "Cloud SOC detection lab — simulate atomic attacks, run Sigma rules, verify alerts fire with proof. 5 tests, Docker Compose."

  # mastermind — add test count
  gh repo edit cy1ingachref/mastermind \
    --description "Multi-agent orchestration — lead AI decomposes tasks, delegates to workers, aggregates results. 44 tests."

  # evidence-guardian — already good, optional addition
  gh repo edit cy1ingachref/evidence-guardian \
    --description "AI-native security scanner — SSRF, IDOR, XSS, SQLi, open redirect. Every finding carries reproducible evidence. 9 free AI providers, 17 tests."

Pinning (GitHub web UI only — API doesn't support reorder):

  Current: purple-team-gym, bcrypt-5digit-cracker, evidence-guardian,
           sigma-lab, 01-devsecops-pipeline, one-mind

  Suggested:
  - Unpin: bcrypt-5digit-cracker
  - Pin: netmon-lan-monitor (45 tests, Windows, blue+red team —
    strong DevOps + security signal)

  Desired order after swap:
  1. evidence-guardian
  2. 01-devsecops-pipeline
  3. one-mind
  4. 05-purple-team-gym
  5. sigma-lab
  6. netmon-lan-monitor
