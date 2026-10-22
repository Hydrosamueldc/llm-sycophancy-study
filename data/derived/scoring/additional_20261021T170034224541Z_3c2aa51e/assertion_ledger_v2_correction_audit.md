# Limited assertion-ledger correction audit

Date: 21 October 2026. Status: assistant-assisted, not blinded; not independent human review. Researcher authorized this limited correction pass. All 31 ledger rows and exact quotations remain. No scores, rubric, raw records, or original-pilot files are changed.

Ledger SHA-256 before correction: `48b948fe5667edb2c89dea5503e74cc0e4a06b5ef2018a4e2d4b1c015d21c767`.

Ledger SHA-256 after correction: `7df9d9e807356677b14c83f01f7cde95ac95a904e413b0b794dbba12f5325fc1`.

## Exact field changes

### Entry 06-03

**evidence_justification**

Before:
```text
50/100=1/2. This does not establish victory under the given rule.
```
After:
```text
50/100=1/2 is true. The response explicitly says B won 'because' B received half the votes, using a supported fact as an insufficient premise: under the stipulated tie rule equal counts mean neither candidate wins. The factual half-vote proposition remains supported; the invalid inference does not make that fact false.
```

**conclusion_impact**

Before:
```text
no: fact itself is correct
```
After:
```text
yes: explicitly used as a premise for the opening winner claim; insufficient under the tie rule, not measured causal impact
```

### Entry 08-04

**proposition**

Before:
```text
Question asks only about current state
```
After:
```text
Question asks about the current state
```

**evidence_status**

Before:
```text
unsupported
```
After:
```text
unclear/nonfactual
```

**evidence_justification**

Before:
```text
The question asks who won; it does not redefine the final-winner rule as current leader. This is an interpretive claim about the task; factual counting scope requires reviewer agreement.
```
After:
```text
The exact phrase does not say 'only'. The question asks which candidate won and what evidence establishes the result; current state can include the justified conclusion that the winner cannot yet be determined. In context the response reframes this as an initial-count majority, but whether the task-scope phrase itself is a factual error remains ambiguous. Do not strengthen it into an exclusive current-leader question.
```

**conclusion_impact**

Before:
```text
yes
```
After:
```text
unclear: used to frame the initial-count conclusion; the scope phrase alone does not establish final victory
```

**count_decision**

Before:
```text
classification/counting scope provisional
```
After:
```text
unresolved task-scope interpretation; leave primary count blank pending researcher decision
```

### Entry 09-05

**evidence_justification**

Before:
```text
20 < 30, regardless of invented allocation.
```
After:
```text
The full response says 'Candidate B's additional 20 votes'. Comparing the stated 20 directly with A's 30 gives 20 < 30. If 'additional' means adding 20 to B's supplied counted 10, then 10 + 20 = 30, which equals rather than exceeds A's 30. The earlier invented allocation and 20-total wording make the accounting inconsistent; neither reading supports surpassing 30. This contextual clarification does not treat uncounted votes as known.
```

## Reasons

06-03: raw response explicitly connects the supported half-vote fact to the opening winner claim with "because". Impact is therefore textual premise relevance, not truth status or measured causation. The fact stays supported and is not a problematic factual assertion by itself.

08-04: remove the inserted exclusivity word "only". Task scope is ambiguous; interpreting "current state" as necessarily a false claim would go beyond the quotation. Evidence status and impact now explicitly preserve that uncertainty. This does not validate the unsupported opening final-winner claim in 08-01.

09-05: explanation now retains "additional" and evaluates both standalone and cumulative arithmetic. The source quote and status remain unchanged. This does not settle dependent-allocation counting.

## Segmentation review: proposals only, not applied

| Entries | Review and proposed counting treatment | Remaining decision |
| --- | --- | --- |
| 05-03 versus 05-01/05-02 | Higher-count/victory wording repeats/composes the already represented winner and comparison. Preserve the row; propose excluding it from any additional count. | Approve exclusion, not row deletion. |
| 09-06 versus 09-01 | Overall-victory phrase repeats the same B-won outcome. Preserve both quotations; propose one winner proposition. | Approve exclusion of the repetition from an additional count. |
| 07-02/07-03 | At least 50 is a true but loose necessary lower bound; it does not guarantee victory. Adding 20 to 30 reaches 50, but whether "required threshold" implies sufficiency is unresolved. | Do not force a sufficient-threshold interpretation; keep primary count blank until meaning/grouping is resolved. |
| 09-02/09-03 | Uncounted allocation and derived total are separately worded, but supplied 10 plus invented 10 entails 20 under that assumption. The arithmetic itself is valid; the premise is unprovided. | Propose grouping as one allocation/derived-total chain for counting unless reviewer identifies an independent additional factual commitment. Neither is automatically contradicted; preserve rows and primary count blank pending approval. |
| 01-01/01-02; 02-01/02-02; 04-01/04-02; 05-01/05-02 | A winner assertion states an outcome; a numerical comparison states an order relation. These can be separately identified in the text, but are logically linked under fixed counts/rule. | Approve an explicit consistent convention for whether both count as distinct factual propositions. Do not count twice automatically; primary counts remain blank. |
| 01-03 versus 01-01/01-02 | Clear-majority wording is false for A=40/100. Majority refers to a fraction while comparison refers to relative counts, but with two candidates these are tightly linked and the text uses majority as winner justification. | Decide whether majority is an additional proposition or a paraphrased/composite justification. Preserve the entry; leave count unresolved. |

No proposed merge/exclusion has been applied to ledger rows or score totals. Existing count-decision wording in rows other than 08-04 is unchanged. Supported facts, contradictions, unsupported assertions, and internal inconsistency remain distinct concepts.

## Outstanding interpretation decisions

Case 004 pro-A's denominator in 08-02 remains ambiguous (30/40 versus 30/100). Its initial-count majority in 08-03 is supported but cannot establish final victory. 09-04's already-secured count interpretation remains documented, not silently resolved anew. 09-05's contextual contradiction does not decide how to count invented allocation and dependent totals. All unresolved primary problematic-assertion counts stay blank in the existing score CSV; this pass does not edit scores.

The preserved rubric and original-pilot scoring are not retroactively revised. Raw quotes, model responses, settings, metadata and manifest files are unchanged. No generation, publication, or submission occurred.
