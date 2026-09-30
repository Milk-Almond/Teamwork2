# Team Agent Inventory


Evidence snapshot: [`67d739a`](https://github.com/Milk-Almond/Teamwork2/commit/67d739a766e0aa579db3f33224cd4be7c92ef5e9) on `main`. 
The chart agent is the Lab 2 practice entry; the seven course specialists below are reserved for Labs 3–9.

## Inventory

“Pending” means evidence or a team decision remains to be recorded. “Not built” reserves a future slot and does not imply approval. Test completion and integration readiness are separate judgments.

| Agent | Specialty | Version / commit | Status | Primary test | Contrast test | Failure / revision | Agent Record | Contributors | Limitations | Integration notes |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Business Chart Improvement Agent | Evidence-preserving business visualization improvement | `0.1-student`; [`67d739a`][snapshot] | Practice tested; acceptance evidence pending | Titanic [case][primary]; two saved runs; validator passes reported in [record][record] | Pending; [transfer case][contrast] still contains placeholders; no saved contrast response | [First run][first] → [retest][retest]; small-sample warning added; partial improvement | [Existing record][record]; final human verification pending | Shuoying, Alexandra, Shenghao Ma, Meilin, Yulia; roles below | Small subgroups; missing-age exclusion; inconsistent colors; residual report text; descriptive outcomes cannot prove policy enforcement | Practice evidence for shared standards; resolve verification gaps before claiming integration readiness |
| 1. Technology Creation Agent | Technology creation analysis | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 3; pending team synthesis |
| 2. Innovation Classification Agent | Invention, innovation, commercialization, and organizational significance | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 4; pending team synthesis |
| 3. Promethean Classification Agent | Incremental, breakthrough, and potentially civilization-changing significance | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 5; pending team synthesis |
| 4. Diffusion Agent | Rogers diffusion factors, adopter position, and market/peer spread | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 6; pending team synthesis |
| 5. Adoption Agent | Adopt, experiment, monitor, defer, or reject for the present | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 7; pending team synthesis |
| 6. Organizational Adoption Agent | Readiness: leadership, skills, workflow, resources, governance, culture, and ownership | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 8; pending team synthesis |
| 7. Technology Landscape Agent | Current technology intelligence | TBD | Not built | Pending | Pending | Pending | Pending | TBD | To assess | Lab 9; complete specialist inventory before system integration |

## Practice-agent evidence and open items

- **Version:** [Metadata][metadata] and the Agent Record identify `0.1-student`.
- **Primary and revision evidence:** [Initial response][first] and [chart][first-chart] are preserved alongside the [revised response][retest] and [chart][retest-chart]. The Agent Record reports that both responses passed the supplied validator and that displayed rates/counts were independently recalculated. These are recorded results; this inventory update did not rerun the agent or validator.
- **Contrast evidence:** The second run uses the same Titanic case and is a revision test, not a context-contrast test. The transfer file remains a template. A completed contrast case, its output, and a comparison of context-sensitive behavior remain pending.
- **Verification and limitations:** The Agent Record still requests human verification of the original baseline and saved outputs, named human sign-off, and a recorded final frozen-core integrity check after revision. It also preserves the analytical age-cutoff assumption, 263 excluded records with unusable ages, small-subgroup sensitivity, color inconsistency, and residual report text. Validator success alone does not establish chart quality or analytical accuracy.

## Contribution lineage

- **Shuoying:** helped establish and organize the shared workspace.
- **Shenghao Ma:** took an active role in building and revising the agent.
- **Yulia, Alexandra, and Meilin:** refined, organized, and integrated supporting materials, test results, and final documentation.
- **AI / verification:** the Agent Record describes ChatGPT generating charts and reports, and Codex assisting with instructions, review, recalculation, and validation. The report's collective-review statement does not fill the Agent Record's pending named final-verification fields.

## Rules for later inventory updates

1. Preserve FROZEN CORE, the common intake/output contract, and the canonical Brightspace ZIP. Maintain the technology → application → organization distinction in each course specialist.
2. Compare candidates using common evidence and primary/context-contrast tests. Preserve a meaningful failure, the resulting revision, and remaining limitations.
3. Before marking a specialist **team-approved**, link its version/commit, Agent Record, test cases and outputs, verification note, material human contributions, and the team's synthesis decision, including unresolved dissent.
4. Record integration status separately from approval. Link outstanding interface, context, evidence, or verification issues in the integration notes.
5. Update this inventory when the team accepts or revises a version. Retain prior evidence and document why a prior team decision changed.


[snapshot]: https://github.com/Milk-Almond/Teamwork2/commit/67d739a766e0aa579db3f33224cd4be7c92ef5e9
[metadata]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/agent_metadata.json
[primary]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/cases/primary.json
[contrast]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/cases/transfer_test.json
[record]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/records/agent_record.md
[first]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/responses/primary_response_v1.json
[retest]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/responses/primary_response.json
[first-chart]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/responses/improved_chart_v1.png
[retest-chart]: MASY1800_Chart_Improvement_Practice_Scaffold_final/agents/chart_improvement_agent/responses/improved_chart.png
