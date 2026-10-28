---
name: quality-gate
description: Assess an existing deliverable against measurable acceptance tests, evidence, provenance, privacy rules and completion criteria.
---
# Quality gate

1. Identify the deliverable, exact version, inputs and authorized scope.
2. Verify that input files exist; never claim to have checked inaccessible files.
3. Run mechanical tests locally when possible and preserve commands and outputs.
4. For claims involving scientific or clinical evidence, map each material claim to a verifiable primary source; mark unverified items.
5. Check for data leaks, unsupported assertions, corrupted packaging and regressions.
6. Classify findings:
   - P0: confidentiality, safety, fabricated evidence, broken essential deliverable; stop.
   - P1: substantive verifiable error; fix and retest.
   - P2: optional cosmetic improvement; do not block release indefinitely.
7. Propose at most one bounded revision cycle when no P0 issues remain.
8. Write the result using templates/handoff.md; distinguish PASS, FAIL and NOT RUN.
9. Require human approval before publication, payment or sharing restricted information.
