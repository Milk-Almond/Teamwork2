# Workflow Evidence and Blockers

## Verified evidence from the current repository
On 2026-09-22, the shared repository was inspected through the GitHub connection.

The repository contains `MASY1800_Chart_Improvement_Practice_Scaffold_v1_0`, including:
- frozen/common instructions under `core/`;
- common input and output schemas;
- `tools/check_frozen_core.py`;
- `tools/build_prompt.py`;
- `tools/new_agent.py`;
- `tools/validate_response.py`;
- a SHA-256 frozen-core manifest;
- course-material files and a student agent template.

The frozen-core manifest and current frozen files were checked against their SHA-256 values. Result: **FROZEN CORE INTACT**.

Inspection of `START_HERE.md` and `CHATGPT_CODEX_WORKFLOW.md` confirms that the practice workflow is designed to:
1. inspect the frozen vs. student-editable architecture;
2. create a specialist from the template;
3. build a prompt packet locally;
4. run the packet in ordinary ChatGPT with required attachments;
5. save the structured JSON and artifact;
6. validate the response locally;
7. preserve a failure/revision comparison;
8. re-check frozen-core integrity before committing.

The workflow documentation explicitly states that the scaffold does **not** call the OpenAI API and does **not** require a separate API key.

## Blocker preserved for Team Lab 2
The assignment names a canonical package: `MASY1800_ET_Agent_Scaffold_v1_0`. That exact package is not currently present in `Milk-Almond/Teamwork2` based on repository search and inspection.

Therefore:
- we do **not** claim that the exact Team Lab 2 canonical scaffold has been exercised;
- the current chart-improvement scaffold is used only as concrete evidence of the shared scaffold pattern and local validation workflow;
- when `MASY1800_ET_Agent_Scaffold_v1_0` is added, the team must inspect its actual frozen files, editable files, context intake, output contract, validator, and operating guide, then update the Team Agent Design and Integration Standard if any mapping differs.

## Next verification action when the canonical package is available
1. Commit an unchanged working copy outside the canonical ZIP.
2. Run its included frozen-core/integrity check.
3. Run or inspect the provided sample prompt-packet workflow.
4. Save one structured output and run the included validator.
5. Record the exact commands, pass/fail output, commit SHA, and any blocker here.
6. Update the inventory/standard only through team review; never alter the canonical Brightspace ZIP.
