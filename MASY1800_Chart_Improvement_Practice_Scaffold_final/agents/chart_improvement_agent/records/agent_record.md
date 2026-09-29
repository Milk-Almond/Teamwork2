# Chart Improvement Specialist Agent Record

- Repository / branch / commit:
  [Enter the actual repository URL, branch, and commit identifier. If these have not been created, state “Not yet recorded.”]

- Agent name and version:
  Business Chart Improvement Agent.
  Both generated reports identify the agent version as 0.1-student. The first-run outputs are preserved as primary_response_v1.json and improved_chart_v1.png. The second-run outputs are primary_response.json and improved_chart.png.

- Exact business question:
  Did “women and children first” apply on the Titanic?

- Baseline chart filename:
  agents/chart_improvement_agent/assets/baseline_chart.png

- Improved chart filename:
  agents/chart_improvement_agent/responses/improved_chart.png

- Most important baseline weakness:
  The generated assessments describe the baseline as combining boys and girls into one child category, although the case specifies separate groups. This would conceal subgroup differences relevant to the question. This description must be checked against the original baseline chart before final submission; it has not been independently verified in this review.

- Visualization principle used:
  Purpose—Frame and Audience: preserve the analytical question, use the specified comparison groups, and explain limitations to a non-specialist audience.
  Signs—Communication: present understandable rates, group labels, and sample sizes.
  Charts—Right Chart and Selection: use positions on a common scale to support comparisons.
  Method—Title: communicate a verified finding without implying that observed outcomes prove consistent historical policy enforcement.

- How the case study was used for calibration rather than copied:
  The case study informed the need for human review of AI-generated design recommendations, particularly chart selection and audience communication. The visualization-principles document remained the governing framework. No case-specific title, annotation, or design was adopted as a mandatory template. The observed regression in color consistency during retesting reinforced the need to inspect generated charts rather than accept all proposed improvements.

- Most consequential change made:
  The second run added an explicit chart note identifying first-class girls (n=3) and first-class boys (n=5) and explaining that individual outcomes can substantially change these percentages. This made a limitation visible that sample-size labels alone did not explain.

- Data-fidelity checks performed:
  Survival rates were independently recalculated from Titanic.xlsx using the case definition of children as younger than 16 and adults as 16 or older. Records with missing or non-numeric ages were excluded from these age-defined groups.

  The dataset contains 1,309 passenger records, of which 263 lack usable ages, leaving 1,046 records in the comparisons. The excluded proportion is 20.1%.

  Verified survivor counts, group totals, and rounded rates:
  - First class: adult women 126/130 = 96.9%; girls 2/3 = 66.7%; boys 5/5 = 100.0%; adult men 48/146 = 32.9%.
  - Second class: adult women 76/87 = 87.4%; girls 16/16 = 100.0%; boys 11/12 = 91.7%; adult men 12/146 = 8.2%.
  - Third class: adult women 53/115 = 46.1%; girls 19/37 = 51.4%; boys 13/42 = 31.0%; adult men 46/307 = 15.0%.

  All 12 displayed rates and sample sizes in both improved charts match these calculations.

- First test result:
  The first structured response passed the supplied validate_response.py tool. The chart displayed verified rates, sample sizes, an age-definition note, and the missing-age exclusion. It also distinguished outcomes consistent with “women and children first” from proof of consistent policy enforcement.

- Weakness or failure preserved from the first test:
  The chart did not explicitly explain the sensitivity of the smallest subgroup percentages to individual outcomes. The report also contained extraneous text, including a trailing business_question label, “Pasted text,” and truncated source-document labels.

- Revision made to the specialist instructions:
  Two requirements were added:
  1. Include a visible small-sample caution identifying the relevant group sizes and explaining their sensitivity to individual outcomes.
  2. Check the business-question field and report for extraneous interface text and truncated attachment labels, while retaining readable source attribution.

- Retest result:
  The second structured response passed the supplied validator. All displayed rates and sample sizes remained correct. The chart added the requested small-sample caution, and the business-question field no longer contained the extra trailing label.

  The revision was only partially successful. “Pasted text” and truncated document labels remained elsewhere in the report. The chart also introduced inconsistent colors across passenger classes for the same demographic groups. Its age-cutoff note no longer explicitly stated that the cutoff was an analytical assumption, although this qualification remained in the report.

  This was a revision test using the same analytical case, not a context-contrast test.

- Remaining limitation:
  The second chart is not uniformly better than the first. Color meanings are inconsistent across classes, some report text remains unclean, and the chart should more clearly identify the age cutoff as an analytical assumption.

  Excluding 263 passengers with missing ages may affect representativeness; the available analysis does not establish that missingness is random. Very small child subgroups are sensitive to individual outcomes. Survival differences are descriptive and cannot prove that a boarding policy was consistently enforced.

  Claims about the baseline chart still require human comparison with the original file.

- Independent judgment: Did the specialist materially improve communication of the business answer? Why or why not?
  The instruction revision materially improved communication of one important limitation by making the smallest subgroup sizes and their sensitivity explicit. It preserved verified values and the distinction between observed survival patterns and historical policy enforcement.

  However, the second output should not be described as an unqualified improvement. Inconsistent colors and residual report text demonstrate that satisfying one instruction does not guarantee overall quality. The defensible conclusion is partial improvement with documented limitations. A final judgment about improvement over the original baseline requires direct inspection of that baseline.

- AI / verification note:
  ChatGPT generated the chart and structured report. Codex helped formulate specialist instructions, reviewed both generated reports and chart images, independently recalculated the displayed counts and rates from Titanic.xlsx, and ran the supplied response validator on both pasted reports. Both returned VALIDATION PASSED.

  The validator checks the response contract; it does not establish analytical accuracy, chart quality, or the existence of a saved PNG. These require separate checks.

  An earlier local frozen-core check returned FROZEN CORE INTACT. A final integrity check after the instruction revision remains to be recorded.

  Human contributor(s): [Enter names and actual contributions.]
  Final human verification: [Enter who checked the baseline, saved output files, and remaining limitations.]