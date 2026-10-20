# Veridion POC Simulation – Part 1: Entity resolution and data QC

**Read first: [report_final.pdf](report_final.pdf)** (2-3 minute summary of my thinking, results and what is not done).
**All the work: [presales_work_final.xlsx](presales_work_final.xlsx)** – start with the `README` tab, then `Reasoning` (every step: what I did, why, result, and in which tab).

## In short
- 592 client companies, 2,951 candidates. I scored each candidate (name 40, country 20, street 20, city 10, postal code 10) and chose one per company. The weights are my judgement.
- 7 ties were decided by hand from company registers and websites.
- A sample of 30 accepted rows showed that matches on the first word only are unreliable, so Auto-accept now needs the full name to match.
- Final: 252 Matched, 273 Review (provisional), 67 No match. No rows are deleted.
- Task 2: 11 consistency rules on the chosen records (tab `QC_findings`) and a curation proposal.
- Not done: Review and Unmatched rows were not checked by hand; flagged rows were not verified on the web.

## AI use
I used Claude for the first version of the formulas, the data checks and the first wording of the tabs and report, and Microsoft Copilot to reorder the input columns. I defined the approach and rules, decided the ties, the sample verdicts and the rule change, verified part of the sample on the web, and corrected the wording. Details are in the report.
