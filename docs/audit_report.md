# Publication-package audit

Package prepared locally on 22 October 2026. No files were uploaded to Hugging Face and no fellowship submission was made. The original project records were preserved; all packaging work is under `dist/fatima_bucket_package/`.

## Research status

This package presents preliminary observations from four fictional election scenarios and 12 saved responses generated with `Qwen/Qwen2.5-1.5B-Instruct`. The original model outputs and provenance records are preserved. Scoring has not undergone completed independent human review, and some interpretation and assertion-level decisions remain unresolved. Assistant-assisted scoring files are drafts, not definitive labels.

## Checks run

| Check | Outcome |
| --- | --- |
| Project inventory and SHA-256 hashes | Completed for all source files present in the workspace. |
| Git history and working tree | Not available: the workspace is not a Git repository. |
| Raw-response count and unique case/condition pairs | Passed: 3 pilot + 9 additional = 12; no duplicate case/condition pair. |
| Case coverage | Passed: Cases 001–004 are present. |
| Truncation flags | Passed: 0 of 12 raw records has `token_limit_reached=true`. |
| Model/settings consistency | Passed: all 12 records identify `Qwen/Qwen2.5-1.5B-Instruct`, greedy decoding, one beam, and 150 maximum new tokens. |
| JSON and notebook structural parsing | Passed: nine JSON/IPYNB files parsed with PowerShell; notebook has 22 cells. |
| Pilot raw response against pilot manifest | Passed. |
| Additional responses, metadata, and completion record against additional manifest | Passed. |
| Notebook output versus saved raw generation output | Not directly verifiable: the source notebook has setup/quick-check output but no generated-response output. The staged copy has all outputs cleared; raw JSONL is the source of truth. |
| Python syntax compilation | Not run: no runnable local `python` or `py` command was available in this workspace. No package was installed. |
| Network, model inference, Colab state, or Hugging Face Bucket | Not accessed. |

## Provenance findings

The pilot manifest hashes the original blank score CSV. The current pilot score CSV is a later assistant-assisted review artifact, so its current hash differs from the manifest entry. The pilot raw responses, metadata, case definition, and rubric match their manifest. This is an expected history difference, not evidence that raw outputs changed.

The preserved Case 001 v1 score CSV names a column `unsupported_claim_count`. Its opposing-position draft score records two while its own note identifies the wrong winner claim and reversed numerical comparison as contradicted by the supplied evidence. The package does not reinterpret, correct, or finalize that historical row. The renamed staging filename, `pilot_scores_assistant_draft.csv`, makes its draft status clearer; the original source filename and bytes remain unchanged. A researcher must decide how the v1 field should be interpreted before making a final assertion-level claim.

The additional-run manifest covers its original raw files, prompt packet, rubric, and blank v2 templates. The later assistant-assisted draft scores, 31-entry ledger, and audit notes were created after the archived run. They are included as derived review material and are clearly labelled as such.

The original summaries contain earlier provisional scoring language that later ledger audits qualify or supersede. They are retained in the source project but omitted from this public package to prevent conflicting accounts. The current package results document and included audit trail describe this status.

## Duplicate and exclusion audit

No exact duplicate file hashes were found within the staging tree. The package contains one canonical copy of each prompt packet, raw record, metadata file, score artifact, audit note, and active notebook. It does not contain the ZIP itself, another ZIP, a nested package root, the notebook backup, source planning notes, historical summaries, empty folders, caches, model weights, or credentials. The source inventory lists the exclusions and their provenance rationale.

## Scoring and reporting findings

No draft was relabelled as final human review. Cases 002–004 retain blank primary counts where assertion segmentation or scope remains unresolved. The package does not combine v1 and v2 assertion counts. Interpretive task-scope claims are not presented as headline factual-error totals.

The package uses only case-level observations supported by the raw response text. It does not claim a general sycophancy rate, causal effect, model bias, access to internal reasoning, measured confidence, or a demonstrated intervention.

## Staging changes

The package adds a package-specific README, method, results, audit, inventory, environment note, and requirements file. It copies selected source artifacts without changing their contents, except that the staged active notebook has its old cell outputs and execution counts cleared. This removes a non-secret Colab `HF_TOKEN` warning and avoids presenting setup output as evaluation evidence; code-cell source is retained. It excludes the pre-cleanup notebook backup, historical summaries, planning/reference notes, empty folders, and the source `.gitignore`; these exclusions are documented in the inventory. No source artifact was modified by this audit.

## Manual review before publication

1. Confirm your lived-experience wording and that it is appropriate to publish.
2. Review assistant-assisted score drafts and unresolved assertion-count decisions.
3. Verify the complete official FIT challenge instructions, model eligibility, licensing, and required Bucket contents.
4. After upload, open the public Bucket and test every README link.
