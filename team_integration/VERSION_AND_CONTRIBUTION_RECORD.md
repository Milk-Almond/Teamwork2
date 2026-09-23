# Version and Contribution Record

Record substantive changes to the team integration workspace and later specialist integrations here. This record supplements Git history by capturing purpose, evidence, and team judgment.

| Date | Artifact / Specialist | Version | Contributor(s) | Commit / PR | Change | Evidence Checked | Decision | Dissent / Follow-up |
|---|---|---|---|---|---|---|---|---|
| 2026-09-22 | Team Agent Design and Integration Standard | 0.1 | Team Lab 2 initialization | `team-lab-2-standard` branch | Initialized shared acceptance, evidence, testing, versioning, and integration rules | Existing repository structure and available chart-improvement frozen scaffold inspected | draft for team review | Canonical `MASY1800_ET_Agent_Scaffold_v1_0` is not currently present; verify mappings when added |
| 2026-09-22 | Team Agent Inventory | 0.1 | Team Lab 2 initialization | `team-lab-2-standard` branch | Initialized seven specialist slots and evidence/status fields | Team Lab 2 requirements | draft for team review | Fill owner/contributor names and candidate evidence during later labs |

## Required entry for each later specialist
Each candidate or approved specialist should have a row that identifies:
- specialist name and bounded purpose;
- version and exact commit/PR;
- contributor(s);
- substantive change made;
- primary and contrast tests reviewed;
- preserved failure/revision evidence;
- validator and frozen-core verification;
- team decision and any dissent;
- remaining limitation or follow-up action.

## Version convention
Use a simple semantic progression unless the canonical course guide specifies otherwise:
- `0.x` — candidate / developmental versions;
- `1.0` — first team-approved integration version;
- `1.x` — backward-compatible evidence/instruction improvements;
- `2.0+` — material specialist redesign that requires full comparison testing again.

A version label is not sufficient by itself; it must be tied to an immutable Git commit or reviewed PR.
