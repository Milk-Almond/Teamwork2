# Team Agent Design and Integration Standard

**MASY1-GC 1800 | Emerging Technologies | Team Lab 2**

## Governing Question

**What must remain common across seven specialist agents so independently developed experts can later be integrated into one reliable team system?**

## Team Decision

Every team-approved specialist will preserve the same frozen technical architecture, context discipline, evidence expectations, testing procedure, version/contribution lineage, and integration gate. Specialists may differ in their bounded domain instructions, analytical criteria, evidence rules, and examples, but they may not redefine the common intake contract, structured output contract, validator, or shared acceptance rules. This standard is intended to make each specialist independently improvable while keeping all seven compatible with the final mixture-of-experts system.

## 1. Fixed Architecture vs. Specialist-Editable Elements

The canonical Brightspace scaffold remains the authoritative starting point and is never modified directly. Development occurs only in a separate working copy under version control. Before and after meaningful specialist work, the team will run the scaffold's frozen-core integrity check.

Frozen/common elements include the shared operating instructions, context/intake schema, structured output schema, validator, prompt-building utilities, and frozen-core manifest/check procedure. In the professor-approved chart-improvement practice scaffold, these include `core/common_instructions.md`, `core/input_schema.json`, `core/output_schema.json`, and the shared tools under `tools/`.

A specialist may change only files explicitly designated student-editable. In the team's chart-improvement practice agent, these include `specialist_instructions.md`, `agent_metadata.json`, `cases/primary.json`, `records/agent_record.md`, and permitted specialist-owned assets/responses. A specialist may not solve a local convenience problem by altering the frozen core. If a common contract appears inadequate, the issue is logged for team review and later integration rather than patched inside one specialist.

## 2. Common Context, Evidence, and Judgment Discipline

Every specialist must preserve three levels of judgment: **(1) the emerging technology generally, (2) the technology for the intended application, and (3) that application in the specified organization or industry.** Organizational posture, stakeholders, capabilities, constraints, risk consequences, governance, and decision horizon may change interpretation and management action, but they do not rewrite the underlying general evidence.

Consequential claims must be supported by relevant evidence. Specialists must distinguish evidence from inference; identify assumptions, missing evidence, contradictions, and uncertainty; and qualify or abstain when the evidence is insufficient. When the assignment supplies materials with different roles, the agent must state their authority. The team's current chart-improvement specialist, for example, treats the visualization-principles document as the governing framework and the applied case study as calibration rather than as a template to copy. The same source-authority discipline will be used for later specialists.

## 3. Common Candidate Comparison and Testing Procedure

Candidates will not be selected because their prose is more polished, their instructions are longer, or one isolated output looks impressive. Competing versions of the same specialty will be compared on common evidence and common tests.

1. **Integrity and contract check.** Confirm frozen-core integrity, build or inspect the prompt packet using the scaffold workflow, save the response in the required structured form, and preserve validator pass/fail evidence.
2. **Primary case.** Run the same representative case for competing candidates and review evidence fidelity, specialist reasoning, output-contract compliance, uncertainty handling, and relevance to the stated management decision.
3. **Context-contrast case.** Change a meaningful application or organizational condition while keeping the common architecture stable. A contextual specialist should appropriately adapt its priorities, interpretation, or management implications rather than return interchangeable boilerplate.
4. **Failure/revision cycle.** Preserve at least one weak, generic, unsupported, or overconfident result. Diagnose the problem, revise only the smallest appropriate student-editable element, rerun the same case, and keep both before-and-after evidence. The team will not change the test simply to manufacture success.
5. **Team acceptance review.** The team reviews the evidence package and records any important dissent, limitation, or unresolved issue before approving integration.

## 4. Minimum Evidence for Team Approval

A specialist is not integration-ready on fluency alone. At minimum, every team-approved specialist must carry an **Agent Record**, an explicit **version tied to a Git commit or reviewed PR**, **primary and context-contrast test evidence**, one **preserved failure and revision**, a documented **limitation/uncertainty/abstention condition**, **validator and frozen-core verification**, an **AI-use and verification note**, and **contribution lineage** showing who materially built, tested, challenged, or verified the work.

The Agent Record must identify the specialist's governing question and boundaries, three-level context logic, evidence rules and contrary-evidence treatment, key test results, the revision made after failure, the remaining limitation or dissent, and the handoff expectations for other specialists.

## 5. Version, Contribution, and Decision Discipline

Every meaningful specialist revision receives a descriptive commit. Agent versions must map to identifiable repository states, and a version number is not reused after substantive changes. Failed or superseded tests are preserved rather than overwritten. Git history provides technical lineage, while the contribution record explains the professional reason for consequential changes.

The shared team inventory records each specialist's bounded purpose, contributor(s), version, commit/PR, primary and contrast test status, failure/revision evidence, limitation, validator/frozen-core status, and integration status. Disagreement is documented rather than silently reconciled. When the team cannot resolve a consequential question, the record should state the competing views and what additional evidence would reopen the decision.

## 6. Integration Gate and Final-Project Handoff

A candidate moves into the shared team system only after its evidence package has been reviewed and consequential technical checks have been independently verified by another team member. The team then makes an explicit human decision to accept, revise, reject with evidence, or preserve the candidate as blocked.

A team-approved specialist must continue to use the common context intake and common structured output contract. Its exact version is entered in the team inventory. After all seven specialists have been synthesized, the final mixture-of-experts stage will test routing, orchestration, contradictory findings, fallback behavior, human-review requirements, and synthesis across experts. Individual specialists therefore remain bounded: they provide traceable expert findings in a common form rather than attempting to perform the responsibilities of every other specialist.

## Team Lab 2 Report-Out

- **Frozen rule:** Individual specialists do not modify the frozen common architecture, shared intake contract, output contract, or validation mechanism.
- **Team convention:** Every candidate carries the same minimum evidence package and is evaluated using primary, context-contrast, and failure/revision testing before team approval.
- **Integration failure to prevent:** Seven individually persuasive agents that use incompatible contracts, cannot be traced to tested versions, ignore organizational context, conceal weak runs, or cannot later be synthesized into one accountable management system.

*Basis for this standard: Team Lab 2 instructions, Weekly Team Professional-Practice Lab requirements, the professor-approved chart-improvement scaffold, and the team's existing GitHub chart-improvement work and version history.*
