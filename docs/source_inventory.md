# Source inventory and package decisions

This inventory describes the source workspace at packaging time. “Authoritative” means the file is the closest available record of a run or review stage; it does not make a draft score final.

| Source artifact | Type and purpose | Status / relation | Package decision |
| --- | --- | --- | --- |
| `README.md` | Documentation | Current project overview | Rewritten as package `README.md` with paths adapted to this ZIP. |
| `notebooks/01_model_setup.ipynb` | Notebook | Active Colab workflow; source notebook has setup output but no generated-response output | Include with outputs and execution counts cleared in staging; code source is retained. |
| `notebooks/01_model_setup.before_cleanup.ipynb` | Notebook backup | Historical pre-cleanup copy | Exclude from public package; not needed to inspect or reproduce saved runs. |
| `data/pilot_*_case.json` | Prompt/case definition | Authoritative Case 001 definition | Include as `prompts/pilot_case.json`. |
| `data/pilot_*_rubric.json` | Rubric | Historical Case 001 v1 rubric | Include as `prompts/pilot_rubric_v1.json`. |
| `data/additional_*/approved_packet.json` | Prompt packet | Authoritative Cases 002–004 prompts and references | Include as `prompts/additional_approved_packet.json`. |
| `data/additional_*/rubric_v2.md` | Rubric | Authoritative v2 rubric for Cases 002–004 | Include as `prompts/rubric_v2.md`. |
| `data/additional_cases_002_004_review.json` | Prompt-review record | Earlier review copy related to approved packet | Exclude; packet is the run-linked authoritative copy. |
| `results/raw/pilot_*` | Raw responses, metadata, manifest | Authoritative Case 001 run record | Include without alteration. |
| `results/raw/additional_*/responses.jsonl` | Raw responses | Authoritative Cases 002–004 responses | Include without alteration. |
| `results/raw/additional_*/metadata.json`, `completion.json`, `manifest.json` | Run provenance | Authoritative additional-run metadata | Include without alteration. |
| `results/scored/pilot_*_human_scores.csv` | Scoring | Historical assistant-assisted draft despite filename; v1 `unsupported_claim_count` terminology requires review | Include as `pilot_scores_assistant_draft.csv`; label draft and preserve source bytes. |
| `results/scored/additional_*/scores_v2.csv`, `assertions_v2.csv` | Templates | Original blank score forms hashed in run manifest | Include and label blank historical templates. |
| `results/scored/additional_*/scores_v2_assistant_draft.csv` | Scoring | Current response-level assistant-assisted draft | Include and label draft. |
| `results/scored/additional_*/assertions_v2_assistant_draft.csv` | Scoring | Earlier partial assistant-assisted review | Include and label earlier partial draft. |
| `results/scored/additional_*/assertion_ledger_v2_review.csv` | Scoring | Current assertion-level ledger; unresolved fields remain blank | Include and label assistant-assisted review. |
| `results/scored/additional_*/assertion_ledger_*_audit.md` | Audit | Corrections and Case 004 status provenance | Include without alteration. |
| `results/*_summary.md` | Summary | Historical summaries with superseded provisional wording | Exclude; audit report documents the reason. |
| `research/exploratory_report.md` | Report | Current source synthesis | Replace with package-specific method/results documents; do not duplicate. |
| `research/project_plan.md` | Planning | Predates completed experiment | Exclude. |
| `research/reference_comparison.md` | Reference notes | External-example organization notes | Exclude. |
| `research/additional_cases_002_004_review.md` | Prompt-review note | Earlier narrative review of approved packet | Exclude. |
| `figures/`, `src/` | Directories | Empty | Exclude. |
| `.gitignore` | Configuration | Local development ignore rules | Exclude. |

No credentials, `.env` files, virtual environments, caches, remote Colab files, or downloaded ZIP archives were present in the workspace inventory. No remote Colab state was inspected.
