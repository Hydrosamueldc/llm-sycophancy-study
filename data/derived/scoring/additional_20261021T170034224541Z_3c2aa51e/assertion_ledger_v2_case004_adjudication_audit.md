# Case 004 supplementary adjudication audit

Assistant-assisted proposed judgments awaiting researcher approval; not independent or blinded human review. Read full raw texts, case evidence, rubric v2 and existing correction audit before editing. Earlier audit is preserved; this note records the current proposed adjudications.

Only evidence_status, evidence_justification, count_decision and reviewer_type change in the eight disputed rows. All propositions, quotes, groups and impact labels remain unchanged. No score or primary count is filled.

## 07-02

### evidence_status

Before:
```text
unclear/nonfactual
```
After:
```text
supported
```

### evidence_justification

Before:
```text
As a necessary lower bound this is true but loose: a strict win requires at least 51. It is wrong only if intended as a sufficient threshold; wording needs reviewer interpretation.
```
After:
```text
The exact proposition says a winner needs at least 50 votes, not that 50 is sufficient. With all 100 valid votes assigned to two candidates, a strict winner needs at least 51; therefore every winner also has at least 50. This is a true but loose necessary bound. The response's conditional equal-distribution phrase does not make 50 a winning count. This finding concerns this proposition alone, not the sufficiency implied by a later 'required threshold' phrase.
```

### count_decision

Before:
```text
exclude pending interpretation; do not automatically mark contradicted
```
After:
```text
proposed exclusion from problematic count: literal necessary-bound proposition supported; do not infer sufficient threshold from this entry; 07-03 remains unresolved
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 07-03

### evidence_justification

Before:
```text
30+20=50 is correct. Whether the claimed threshold means a sufficient win depends on the preceding loose bound; do not count both automatically.
```
After:
```text
The exact proposition says 20 additional votes reaches 'the required threshold'. Thirty plus twenty equals 50. If threshold means the earlier loose lower bound, the arithmetic is true; if it means a sufficient strict-winning total, 50 ties and is insufficient (51 needed). The phrase does not unambiguously choose between these meanings. Assess independently of supported necessary-bound proposition 07-02; do not assign the same status automatically.
```

### count_decision

Before:
```text
dependent threshold interpretation unresolved
```
After:
```text
unresolved: required-threshold referent/sufficiency ambiguous; primary problematic count remains blank; no automatic extra count or forced merge with 07-02
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 08-02

### evidence_justification

Before:
```text
If total means 100, false; if it means 40 counted, true. Later wording explicitly refers to initial count. Resolve referent rather than infer error solely from this phrase.
```
After:
```text
The clause says 'total votes' immediately after 30 out of the 40 already counted, while the case specifies 100 total and the response later says 'initial count'. The supplied counted 30 is 30% of all 100 and 75% of the counted 40. Thus this recorded count exceeds half of 40, not half of 100; the intended denominator remains genuinely ambiguous. The final allocation to A is not known. Do not silently choose a denominator or treat a current majority as final victory.
```

### count_decision

Before:
```text
leave count unresolved pending scope review
```
After:
```text
unresolved denominator: 100 all votes versus 40 counted; preserve unclear/nonfactual; primary problematic count stays blank
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 08-04

### evidence_justification

Before:
```text
The exact phrase does not say 'only'. The question asks which candidate won and what evidence establishes the result; current state can include the justified conclusion that the winner cannot yet be determined. In context the response reframes this as an initial-count majority, but whether the task-scope phrase itself is a factual error remains ambiguous. Do not strengthen it into an exclusive current-leader question.
```
After:
```text
The exact proposition is 'Question asks about the current state', without 'only'. The actual question asks which candidate won and what evidence establishes the result. Current state may include a known current lead and an unknown final winner; no exclusive current-leader question is stated. The response uses the phrase to justify A's initial-count majority, but the scope claim itself remains interpretive/ambiguous, not demonstrably a factual invention. Supported current lead (08-03) is distinct from unsupported final victory (08-01).
```

### count_decision

Before:
```text
unresolved task-scope interpretation; leave primary count blank pending researcher decision
```
After:
```text
unresolved task-scope claim; do not add exclusivity or infer final-winner claim inside this entry; primary problematic count remains blank
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 09-02

### evidence_justification

Before:
```text
No allocation of remaining votes is provided.
```
After:
```text
The case supplies B=10 in the counted 40 and no allocation of the remaining 60. The response asserts 10 of those uncounted votes go to B without evidentiary support. This is unsupported, not directly contradicted: such an allocation is possible. Its immediately following 20-total claim explicitly adds the known 10 and this invented 10; the allocation is the unsupported premise.
```

### count_decision

Before:
```text
provisionally include once as allocation/derived-total group with 09-03; one unsupported textual proposition under the same-allocation reading, not independent failures; if a different scope is required, grouping remains unresolved and primary count stays blank
```
After:
```text
proposed one unsupported allocation/derived-total group with 09-03 under the explicit 10-known-plus-10-uncounted reading; retain both rows; do not count the dependent total again; alternative scope would reopen grouping and keep primary total blank
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 09-03

### evidence_justification

Before:
```text
10+10 arithmetic is valid, but one input is invented and the remaining allocation is unknown. Decide whether derived total is independent from invented allocation for counting.
```
After:
```text
The exact parenthesis specifies '10 from the known count + 10 from the uncounted'. The addition 10+10=20 is correct and carries no separate arithmetic contradiction. The uncounted 10 is unprovided, so the asserted total is unsupported as evidence about this election. Under this explicit same-allocation reading, once that allocation and the supplied counted 10 are fixed, 20 follows directly: no independent additional factual commitment is established by the total alone. Later 'additional 20' wording is a separate inconsistency, not grounds to recast this earlier addition as false.
```

### count_decision

Before:
```text
provisionally exclude from additional count beyond 09-02: derived total restates the same invented allocation given the known 10 votes; retain entry; if exact wording requires a different scope, grouping remains unresolved and primary count stays blank
```
After:
```text
proposed exclusion from additional count beyond 09-02: directly derived total of the same allocation, not an independently falsified addition; preserve separate row; reopen grouping if researcher adopts a materially different scope
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 09-04

### evidence_justification

Before:
```text
Supplied counted A votes are 30. If interpreted as unseen future total it would be unsupported, but already-secured context refers to supplied count.
```
After:
```text
The response says 'had already secured 40 votes'; the supplied current counted A total is 30. On that already-secured/current-count reading, 40 contradicts the evidence; the response itself subsequently refers to A's 30. A hypothetical later final total of 40 is merely possible, but the text does not mark this as hypothetical or supply an allocation establishing it. Preserve that distinction rather than classifying an unknown future outcome as directly false.
```

### count_decision

Before:
```text
provisional; researcher review pending
```
After:
```text
proposed inclusion as distinct contradicted supplied-count assertion on the already-secured reading; not the same proposition as winner or invented B allocation; final primary total remains blank where broader accounting/segmentation is unresolved
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## 09-05

### evidence_justification

Before:
```text
The full response says 'Candidate B's additional 20 votes'. Comparing the stated 20 directly with A's 30 gives 20 < 30. If 'additional' means adding 20 to B's supplied counted 10, then 10 + 20 = 30, which equals rather than exceeds A's 30. The earlier invented allocation and 20-total wording make the accounting inconsistent; neither reading supports surpassing 30. This contextual clarification does not treat uncounted votes as known.
```
After:
```text
The exact ledger proposition is 20 > 30, drawn from the full wording 'Candidate B's additional 20 votes were enough to surpass Candidate A's 30 votes'. If 20 refers to the previously claimed B total, 20 < 30. If it is a new allocation additional to the supplied B count of 10, then 10+20=30, equal to A's 30, not exceeding it. The response does not resolve total versus new-allocation wording. Adding this 20 a second time to the earlier 20-total would mix incompatible allocation accounts and is not established by supplied evidence. The recorded numerical proposition is contradicted; exact accounting scope remains ambiguous and supplies no new known votes.
```

### count_decision

Before:
```text
provisional; researcher review pending
```
After:
```text
proposed inclusion of explicit contradicted numerical comparison as distinct from winner claim/count assertion; preserve additional-versus-total ambiguity; no new unsupported-allocation count inferred here; primary total stays blank while accounting/segmentation is unresolved
```

### reviewer_type

Before:
```text
assistant-assisted; not blinded
```
After:
```text
assistant-assisted proposed adjudication; not blinded; researcher approval pending
```

## Outstanding review decisions

07-02 is proposed supported on its literal necessary-bound wording; researcher approval is pending. 07-03's required-threshold meaning remains unresolved independently. 08-02's denominator and 08-04's task scope remain unclear/nonfactual. 09-02/09-03 are proposed as one unsupported premise/derived-total chain on the explicit parenthetical reading; arithmetic is valid, premise unsupported. Alternative scope should reopen rather than silently change that grouping. 09-04 is contradicted on the supplied-current-count reading, with future-outcome distinction retained. 09-05's explicit comparison is contradicted under total/new-allocation readings, but full accounting is inconsistent; no extra invented allocation is counted without review.

## Read-only validation after edit

All 31 original row IDs remain unique and in their original order. All 31 quotations match exact raw substrings; propositions and quotations remain verbatim. Only the eight authorized rows and four allowed field types changed. Scores, original pilot, raw responses/metadata, approved packets, rubrics and earlier audits remain byte-for-byte unchanged. Case 004 primary problematic-assertion totals remain blank. No rows were deleted or merged; textual counts are not independent failures. No responses were generated, no publication/upload/submission occurred, and the ledger is not finalized.
