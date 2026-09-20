CLAIMS CHANGE LOG — what changed and why
===============================================

CHANGED:
1. "40+ test suites" (SWE table, one-mind row) -> REMOVED
   Why: This was a header label in the "Proof" column, not
   a per-project claim. The SWE table's proof column no
   longer exists in the new layout. One-mind's actual count
   (53 tests) is stated in its featured description.

2. "40+ tests" (one-mind, DevOps table) -> "53 tests across
   2 test files" (one-mind, Featured section)
   Why: Actual count is 53 def test_ functions in 2 files
   (test_cli.py + test_onemind.py). "40+" was an
   underestimate. Using the real number.

3. "real users" (SWE table, Proof column) -> REMOVED
   Why: Not substantiated anywhere in the one-mind repo.
   No user counts, no deployment evidence, no testimonials.
   Keeping vague claims like this risks a recruiter
   checking and finding nothing.

4. "live alerts" (DevSecOps table, Proof column) -> REMOVED
   Why: The 03-cloud-soc-detection-lab README says "verify
   alerts fire with live proof" — the "live" refers to the
   proof being live/active, not to production alerts firing
   in real time. The table claimed "live alerts" as proof
   of the DevSecOps track, which overstates what the lab
   does. The Featured projects section now says "verify
   alerts fire with proof" which is accurate.

5. "bule-team" -> "blue-team" (netmon description)
   Why: Typo. Already fixed in the current README (confirmed
   by grep — not present). No change needed in this commit.

CONFIRMED (no change needed):
- "17 tests" (evidence-guardian): Badge + README both say
  17 passed. Accurate.
- "45/45 tests" (netmon): 45 def test_ functions match.
  Accurate. Featured section uses "45 tests" (shortened).
- "9 free AI providers" (evidence-guardian): OmniRoute badge
  says "9 free providers". README lists all 9 by name.
  Accurate.

RELATIONSHIPS IN MERMAID DIAGRAM:
- sigma -> 03: CONFIRMED. 03 README has Sigma rules and
  detection engine. Real relationship.
- 02 -. designed for CI gates .-> 01: SOFT LINK. 02 README
  says "practical for CI pipeline gates" but doesn't name
  01. 01 README doesn't mention 02 by name. Using a dashed
  edge with "designed for CI gates" label to be honest.
- evidence-guardian -> evidence-backed reports: CONFIRMED.
  Core feature of the project.
- 03 -> 05: DROPPED. No confirmed relationship between the
  SOC detection lab and the purple-team gym. They're
  conceptually adjacent but no explicit link exists.
