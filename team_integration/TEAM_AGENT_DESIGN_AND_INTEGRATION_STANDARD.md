# Team Agent Design and Integration Standard

## Governing Question
What must remain common across seven specialist agents so independently developed experts can later be integrated into one reliable team system?

## Team Decision
Every team-approved specialist must share the same frozen technical architecture, evidence discipline, test procedure, version/contribution record, and integration gate. Specialists may differ in domain instructions and examples, but they may not redefine the common intake contract, output contract, validator, evidence expectations, or team acceptance rules.

## 1. Fixed vs. Specialist-Editable Elements

### Fixed technical architecture
The following categories are common and must not be redesigned by individual specialists:
- frozen/common instructions that define the shared operating boundary;
- common context/intake schema and required context fields;
- common structured output contract/schema;
- validator and scaffold utilities used to build or check prompt packets and outputs;
- frozen-core integrity manifest/check procedure;
- team-level evidence, version, contribution, and integration requirements.

In the professor-approved `MASY1800_Chart_Improvement_Practice_Scaffold_v1_0`, frozen/common elements include `core/common_instructions.md`, `core/input_schema.json`, `core/output_schema.json`, and the shared tools under `tools/`. The frozen-core manifest/check is used to verify that these common elements remain intact.

### Specialist-editable elements
A specialist may change only the files or fields explicitly designated student-editable by the scaffold. For a created chart-improvement specialist, the student-editable files are:
- `specialist_instructions.md`;
- `agent_metadata.json`;
- `cases/primary.json`;
- `records/agent_record.md`;
- specialist-owned assets/responses where the scaffold workflow calls for them.

No specialist may solve a local convenience problem by modifying frozen-core files. If a common contract appears inadequate, record the issue for team review rather than patching one specialist.

## 2. Minimum Evidence for Team Approval
A candidate specialist is not accepted on fluency alone. Its repository/evidence package must contain, at minimum:
1. **Agent Record** — purpose, scope, governing sources, important design choices, and known limitations.
2. **Version** — explicit version identifier tied to a Git commit.
3. **Primary test** — representative in-scope case using the common intake/output architecture.
4. **Context-contrast test** — materially different context that checks whether the specialist adapts to evidence rather than repeating generic language.
5. **Preserved failure and revision** — at least one weak/unsupported behavior, the diagnosis, the instruction change, and rerun evidence.
6. **Limitation** — at least one clear boundary or known failure mode.
7. **Verification note** — validator result and frozen-core integrity result, plus any unresolved blocker.

A polished response without this evidence is not integration-ready.

## 3. Common Candidate Comparison Procedure
All candidate agents are compared using the same evidence and the same test sequence.

### Step A — Integrity and contract checks
- Confirm the frozen core is unchanged using the included integrity tool or manifest.
- Build/inspect the candidate prompt packet using the scaffold workflow.
- Confirm the response can be saved in the required structured form.
- Run the included validator and preserve pass/fail output.

### Step B — Primary-context test
Run the same agreed primary case for competing candidates. Review whether the output:
- answers the supplied decision/business context rather than substituting another task;
- uses provided evidence correctly and avoids invented facts;
- follows the common output contract;
- applies specialist expertise concretely rather than generically;
- states uncertainty, limitations, or abstention when evidence is insufficient.

### Step C — Context-contrast test
Change important context while keeping the common architecture stable. A contextual specialist should materially adapt its reasoning, priorities, or recommendations to the changed evidence. A generic specialist fails when it returns essentially interchangeable advice, ignores changed inputs, or relies on boilerplate expertise statements.

### Step D — Failure/revision test
Preserve one weak or unsupported run. Diagnose the failure, revise only permitted specialist files, rerun the same case, and compare before/after evidence. The revision passes only if it improves the diagnosed behavior without breaking the common contract or creating unsupported claims.

### Step E — Team acceptance review
The team reviews evidence, not just final prose. Acceptance requires: contract compliance, evidence fidelity, contextual behavior, preserved failure/revision, documented limitation, validator success, frozen-core integrity, and complete contribution lineage. Dissent is recorded rather than erased.

## 4. Version, Commit, and Contribution Rules
- Never modify the canonical Brightspace ZIP. Work from a separate committed copy.
- Every meaningful specialist revision receives a commit with a descriptive message.
- Agent versions must map to commits; do not reuse a version number after substantive changes.
- Use branches/pull requests for team integration so candidate history remains inspectable.
- Do not overwrite failed tests. Store or reference them as evidence.
- The team inventory records specialist owner/contributor, version, commit/PR, test status, limitation, and approval state.
- Contributions from multiple people must remain attributable in the contribution record.

## 5. Procedure for Moving a Specialist into the Shared Team System
1. Candidate developer freezes a review version and completes the evidence package.
2. A second team member verifies frozen-core integrity and validator results.
3. The team runs or inspects the primary, contrast, and failure/revision evidence under the common comparison procedure.
4. Any disagreement is recorded in the dissent field of the contribution record.
5. If accepted, the specialist is copied/merged into the shared integration workspace without altering common contracts.
6. The inventory status changes from `candidate` to `team-approved`, recording version and commit/PR.
7. A later cross-agent integration test must confirm that the specialist can coexist with the other agents under the same intake/output conventions.

## 6. Failure Modes This Standard Is Designed to Prevent
- one specialist silently changing the shared schema or validator;
- specialists that sound fluent but ignore the supplied context;
- untraceable versions or edits with no contribution lineage;
- selecting a candidate from one impressive run with no contrast test;
- deleting failed runs and losing evidence of revision quality;
- merging unsupported claims or hidden assumptions into the team system;
- incompatible agent outputs that cannot later be composed into one reliable workflow.

## Report-Out
- **Frozen rule:** individual specialists do not modify the frozen common architecture or shared intake/output contract.
- **Team convention:** every candidate carries the same minimum evidence package and is evaluated with primary, contrast, and failure/revision tests before approval.
- **Integration failure to prevent:** seven individually impressive agents that use incompatible contracts, undocumented versions, or generic context-insensitive behavior and therefore cannot operate reliably as one system.
