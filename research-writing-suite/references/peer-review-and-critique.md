# Peer Review & Critique

**Owns:** judging a document's substance: peer review of manuscripts, proposals, and reports;
critical appraisal of a study; devil's-advocate challenges; mock referee reports; responses to
reviewers (rebuttal letters); and critique of the user's own draft before submission.
**Use when:** "review this paper", "what would a reviewer say?", "critique my proposal", "is this
study any good?", "stress-test my argument", "help me respond to reviewer comments".
**Don't use when:** the user wants sentence-level improvement (`editing-and-polish.md`), wants
specific claims fact-checked (`source-evaluation-and-fact-checking.md`), or needs a
final-delivery QA (`final-checklists.md`).

## Contents
1. Ground rules
2. Review workflow
3. What to assess (by document type)
4. Writing the comments
5. Devil's advocate and red team
6. Responding to reviewers
7. Output templates

---

## 1. Ground rules

- **Confidentiality.** Manuscripts under review are confidential. Confirm the user is entitled to
  share it and that the venue's policy allows AI assistance. If they're unsure, tell them to check
  before pasting. Never put manuscript content into web searches.
- **Evidence-bound.** Every criticism points to a location and says why it matters. Don't invent
  manuscript details, analyses, or citations. Write "not reported" when something is absent.
- **Proportionate and constructive.** Separate fatal flaws from fixable ones; note the strengths;
  request only work needed to support the central claims.
- **Same standard for everyone.** Judge by method, not by whether you like the result, who the
  authors are, or the venue's prestige.
- **Decisions belong to editors and panels.** Give a recommendation only when the user is the
  reviewer and the form asks for one; frame it as the reviewer's recommendation.
- **Human accountability.** The output is a draft for the user to check and rewrite in their own
  judgment before submitting.

## 2. Review workflow

1. **Scope:** the document type, the stage, the venue or criteria, the requested focus, and what
   material is available (supplements, data, code).
2. **Neutral map** (before judging): the question, design, population or system, comparator,
   outcomes, and the 3–5 principal claims.
3. **Claim–evidence check:** for each principal claim, find what supports it (result, table,
   analysis, citation) and check that the direction, magnitude, population, and uncertainty match
   the claim. Use the claim-to-evidence table format from `source-evaluation-and-fact-checking.md` §6.
4. **Methods and statistics:** work in this order: question → design → unit of analysis → sampling or
   allocation → measurement → sample size and precision → missing data and attrition → analysis fit
   and assumptions → multiplicity → effect sizes and uncertainty → interpretation and
   generalisation.
5. **Reproducibility and transparency:** protocol and registration, data and code availability,
   software versions, enough detail to repeat.
6. **Ethics and integrity:** approvals, consent, conflicts, funding, and signs of selective
   reporting. Describe what you observe; don't accuse. Route serious concerns to the editor confidentially.
7. **Presentation:** structure, clarity, figures and tables (consistency with the text,
   units, uncertainty), limitations, and citations.
8. **Draft the comments** (§4), separating comments to the authors from confidential comments to the editor.
9. **Self-check:** every location verified, no speculative criticism, a professional tone, the
   limits of your own review stated (e.g., "statistical methods outside my expertise").

## 3. What to assess (by document type)

| Document | Core questions |
|---|---|
| **Empirical paper** | Is the question important and clear? Can the design answer it? Is the analysis appropriate? Do the conclusions follow? Is it reported well enough to evaluate (CONSORT, STROBE, PRISMA, COREQ, etc.)? |
| **Review article** | Search reproducible and comprehensive? Clear criteria? Quality appraised? Synthesis rather than list? Gaps justified? |
| **Theoretical or argumentative paper** | Clear thesis? Valid reasoning? Strongest objections addressed? Contribution beyond existing positions? |
| **Proposal** | Significance? Clear, testable aims? Feasible approach with contingencies? Innovation? Team and resources fit? Realistic timeline and budget? |
| **Professional or technical report** | Answers the question? Evidence sufficient and current? Analysis sound? Recommendations follow from findings? Risks addressed? Usable by the audience? |
| **Student essay or thesis** | Clear thesis or question? Argument structure? Use of sources? Critical analysis vs. description? Meets the assignment criteria or rubric? |

**Common critical-thinking checks** (all types): correlation treated as causation; confounders
ignored; selection or survivorship bias; p-values without effect sizes; non-significance treated as
"no effect"; subgroup fishing or multiplicity; overgeneralisation; cherry-picked citations; circular
reasoning; a straw-man of opposing views; appeals to authority instead of evidence.

## 4. Writing the comments

Each major or minor comment has five parts:
- **Location:** section, page, line, figure, or table.
- **Observation:** what the text says or does.
- **Criterion or evidence:** why this is a problem (the standard, the logic, the data).
- **Why it matters:** its effect on the conclusions.
- **Requested action:** specific and proportionate (clarify, add an analysis, narrow the claim,
  add a limitation, correct).

Severity labels:
- **Critical:** threatens the main conclusions.
- **Major:** affects interpretation, but is fixable.
- **Minor:** clarity, presentation, small errors.

Tone: direct, respectful, specific. Write "The conclusion that X causes Y is not supported by
the cross-sectional design (Methods, p. 6); please reframe as an association or add…", not "The
authors clearly don't understand causality."

## 5. Devil's advocate and red team

Use this for stress-testing the user's own argument, proposal, or report:
1. State the thesis in its strongest form (steelman it).
2. Generate the **three strongest objections**: evidence-based (contrary data), logical (a gap in
   reasoning), and practical (feasibility, cost, side effects).
3. Offer **alternative explanations** for the key finding.
4. Run a **pre-mortem**: "It is a year later and this failed or was rejected. Why?"
5. Look at it as **personas** where useful: a skeptical expert, a methods reviewer, a practitioner
   who has to act on it, an affected stakeholder.
6. For each objection, say whether it is **fatal, answerable (and how), or a limitation to
   acknowledge**.

## 6. Responding to reviewers

1. **Triage** each comment: *Accept* (straightforward fix) · *Accept with reframing* · *Partly
   accept* (concede part, clarify the rest) · *Respectfully decline* (out of scope, mistaken, or
   in conflict with another reviewer). Show the triage table and let the user confirm before drafting.
2. **Plan changes** as a table (comment number → action → location) and hand execution to
   `editing-and-polish.md` §9.
3. **Draft the letter:**
   ```markdown
   Dear Editor,
   Thank you for the opportunity to revise… [one-paragraph summary of main changes]
   ## Reviewer 1
   **Comment 1.1:** [quote or faithful summary]
   **Response:** [thanks where natural → what we did / why not → evidence]
   **Change:** [location, e.g., p. 7, lines 120–134; quote new text if short]
   ```
4. **Tone:** grateful, calm, specific. Never argue emotionally; frame disagreement as scope or
   methodological rationale, with evidence. Mirror the reviewer's terms.
5. **Useful phrasing:**
   - Partial concession: "We agree that [X] and have revised [location]. We would respectfully
     maintain [Y] because [reason/evidence], and have clarified this in [location]."
   - Declining: "We appreciate this suggestion. Because the study is delimited to [scope], [X] falls
     outside it; we now note this as a limitation (p. N)."
   - Misreading: "We thank the reviewer for this close reading; our original wording was
     ambiguous. We have revised it to: '…' (p. N)."
6. Never claim a change that wasn't made, and never invent new analyses or results. Use
   `[DATA NEEDED]` until the user supplies them.

## 7. Output templates

**Referee report**
```markdown
## Summary of the submission (neutral, 3–5 sentences)
## Overall assessment (strengths; main concerns; whether conclusions are supported)
## Major comments (numbered; location · observation · criterion · why it matters · action)
## Minor comments (numbered)
## Recommendation (only if requested by the venue form)
## Confidential comments to the editor (only if needed: conflicts, expertise limits, integrity concerns)
```

**Self-review / pre-submission critique**
```markdown
## Verdict in one paragraph (readiness + top 3 fixes)
## Critical / Major / Minor issues (table: # · location · issue · fix)
## Claim–evidence check (central claims only)
## Strongest objection a reviewer will raise, and how to pre-empt it
```

**Study appraisal (is this study any good?)**
```markdown
## What it asked and did (PICO/design)
## Main result (with numbers and uncertainty)
## Strengths
## Threats to validity (named, with likely direction of bias)
## What it can and cannot support
## Overall: confidence in the main conclusion — High / Medium / Low, and why
```
