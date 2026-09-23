# Workflow Evidence and Remaining Work

## Verified evidence from the current repository
On 2026-09-22, the shared repository was inspected through the GitHub connection.

The professor-approved course scaffold is `MASY1800_Chart_Improvement_Practice_Scaffold_v1_0`, and it is present in `Milk-Almond/Teamwork2`. It includes:
- frozen/common instructions under `core/`;
- common input and output schemas;
- `tools/check_frozen_core.py`;
- `tools/build_prompt.py`;
- `tools/new_agent.py`;
- `tools/validate_response.py`;
- a SHA-256 frozen-core manifest;
- course-material files and a student agent template.

The frozen-core manifest and current frozen files were checked against their SHA-256 values. Result: **FROZEN CORE INTACT**.

Inspection of `START_HERE.md` and `CHATGPT_CODEX_WORKFLOW.md` confirms that the workflow is designed to:
1. inspect the frozen vs. student-editable architecture;
2. create a specialist from the template;
3. build a prompt packet locally;
4. run the packet in ordinary ChatGPT with required attachments;
5. save the structured JSON and artifact;
6. validate the response locally;
7. preserve a failure/revision comparison;
8. re-check frozen-core integrity before committing.

The workflow documentation explicitly states that the scaffold does **not** call the OpenAI API and does **not** require a separate API key.

## Current Team Lab 2 status
There is **no missing-scaffold blocker**. The professor-approved scaffold is the chart-improvement scaffold already in the repository.

Verified so far:
- correct scaffold identified and present;
- frozen vs. student-editable architecture inspected;
- frozen-core integrity checked successfully;
- prompt-packet/build/validation workflow inspected;
- shared team standard, inventory, and contribution workspace initialized.

Still to preserve as workshop evidence before calling the lab fully complete:
1. run or inspect one complete prompt-packet case with all required inputs;
2. save one structured response and run `tools/validate_response.py` on it;
3. preserve one deliberately weak/generic output and explain why it is insufficiently contextual;
4. run or inspect one context-contrast case and record what changed appropriately;
5. record the team's final review, any dissent, and the agreed report-out.

## Verification discipline
- Do not modify the frozen-core files to make a test pass.
- Preserve failed/weak runs rather than overwriting them.
- Record exact commands, pass/fail results, versions/commits, and limitations.
- Update the team inventory only after the agreed evidence has been reviewed.
