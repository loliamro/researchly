# Professional Reports

**Owns:** technical reports, business and analytical reports, executive summaries, strategy and
decision memos, status updates, white papers, briefing notes, and lab or project reports written
for a professional (non-journal) audience.
**Use when:** "write a technical report on…", "executive summary", "turn this research into a
report for management", "decision memo", "weekly status update", "briefing note".
**Don't use when:** it's a journal manuscript, thesis, or proposal (`academic-writing.md`); the
research hasn't been done yet (run `deep-research-modes.md` first, then return here); or the
user only wants their existing report polished (`editing-and-polish.md`).

## Contents
1. Principles
2. Choosing the format
3. Executive summary template
4. Technical report template
5. Business / analytical report template
6. Decision or strategy memo template
7. Status update template
8. Briefing note and white paper
9. Tables, figures, and numbers
10. Report QA (pointer)

---

## 1. Principles

- **Answer first (BLUF).** The reader should get the conclusion and the ask in the first five lines.
- **Write for a decision.** Know who reads it, what they must decide or do, and by when.
- **One message per section.** Headings state findings ("Costs rise 18% under Option B"), not
  topics ("Costs").
- **Evidence-bound.** Every factual statement is sourced (numbered [1] by default, per
  `citations.md`); figures are reproducible from the stated data; assumptions are listed.
- **The user's own data is a source.** Cite internal data, test results, and interviews by name
  and locator ("Bench test log, 12 Mar 2025, Appendix B"), never as unsourced fact. Don't
  extrapolate beyond what the data shows; label projections as projections, with assumptions.
- **Separate** findings (what is), analysis (what it means), and recommendations (what to do).
- **Honest about risk and uncertainty.** Give a confidence tag on key findings (see
  `source-evaluation-and-fact-checking.md`) and a limitations section.
- **Scannable:** short paragraphs, informative headings, tables for comparisons. Prose still
  carries the reasoning.

## 2. Choosing the format

| Need | Format | Length |
|---|---|---|
| Executive needs the gist and the ask | Executive summary (standalone or front of report) | ½–1 page |
| Document a technical investigation, test, or design | Technical report | 5–30 pages |
| Analyse a business question with data | Business/analytical report | 3–20 pages |
| Get a decision between options | Decision/strategy memo | 1–5 pages |
| Keep stakeholders informed | Status update | < 1 page |
| Brief a senior person quickly | Briefing note | 1–2 pages |
| Persuade an external audience with evidence | White paper | 5–15 pages |

## 3. Executive summary template

```markdown
## Executive summary
**Purpose:** [One sentence: what question this answers and for whom.]
**Bottom line:** [The answer or recommendation in 1–2 sentences, with a confidence tag.]
**Key findings:**
1. [Finding + the number that matters + source] — Confidence: High/Medium/Low
2. …
3. …
**Recommendation(s):** [What to do, who, by when. Tie each to a finding.]
**Risks and uncertainties:** [The 1–3 that could change the recommendation.]
**Decision or action needed:** [The specific ask and deadline.]
```

Rules: 150–400 words (about 10% of the report at most); readable alone; no new information that
isn't in the body; no jargon or undefined acronyms; numbers instead of adjectives ("cut
processing time from 6 to 2 days", not "significantly faster").

## 4. Technical report template

```markdown
# [Title: specific, findings-oriented]
Author(s) · Date · Version · Distribution
## Executive summary            (§3)
## 1. Introduction             (problem, objectives, scope, audience)
## 2. Background               (context, prior work or standards, definitions)
## 3. Method / approach        (setup, materials, data, procedure, tools and versions — enough to reproduce)
## 4. Results                  (objective presentation; tables and figures with units and uncertainty)
## 5. Analysis and discussion  (interpretation, comparison with requirements or benchmarks, error sources)
## 6. Conclusions              (answers to each objective)
## 7. Recommendations          (prioritised, actionable, each traced to a conclusion)
## 8. Limitations and assumptions
## References
## Appendices                  (raw data, calculations, code listings, detailed specs)
```

For lab reports, use: Title → Abstract → Introduction/theory → Method → Results → Discussion
(including error analysis) → Conclusion → References → Appendices. Use the instructor's template
if one is given.

## 5. Business / analytical report template

```markdown
# [Title]
## Executive summary
## 1. Context and question     (why now; the decision this informs)
## 2. Approach and data        (sources, period, definitions, method; data limitations)
## 3. Findings                 (one subsection per finding; headline sentence first, then evidence)
## 4. Options and analysis     (if relevant: options × criteria table, costs, benefits, risks)
## 5. Recommendations          (what, who, when, cost, expected impact, success metric)
## 6. Risks and mitigations    (likelihood · impact · mitigation · owner)
## 7. Next steps
## Appendix: method details, data tables, assumptions register
```

**Options × criteria table:**
```markdown
| Criterion (weight) | Option A | Option B | Option C | Evidence |
|---|---|---|---|---|
```
Make the weights explicit, and say how sensitive the result is to them.

## 6. Decision or strategy memo template

```markdown
# Memo: [Decision to be made]
**To / From / Date / Status:** Draft · For decision · Final
## TL;DR              (recommendation + why, in 3–4 sentences)
## Context            (current state, what changed, why decide now)
## Recommendation     (specific; scope; owner)
## Rationale          (strategic fit, user or customer value, business impact — each with evidence)
## Alternatives considered (each option: pros, cons, why not)
## Risks and mitigations (table)
## Implementation     (phases, milestones, resources, success metrics with targets)
## Open questions
```
Memo variants: a **decision** memo chooses between options; a **vision** memo describes a
future state; a **planning** memo describes execution; a **problem/solution** memo defines and proposes.

## 7. Status update template

```markdown
**Status — [Project] — [Period/Date]**
**Overall:** On track / At risk / Blocked — [one-sentence reason]
**Done this period:** [outcomes, not activities]
**In progress:** [item — status — ETA]
**Metrics:** [metric: value (change vs. last period)]
**Risks / blockers:** [issue — impact — mitigation or what's needed]
**Next steps:** [action — owner — due date]
**Asks:** [specific request + deadline]
```
Keep it under one page. Report bad news early and plainly. Every next step has an owner and a
date. Give trends, not just levels.

## 8. Briefing note and white paper

**Briefing note:** Issue (1 sentence) → Background (key facts) → Current status → Key
considerations (options, implications, stakeholder positions) → Recommendation → Contact. Plain
language, 1–2 pages.

**White paper:** Problem and stakes → evidence-based analysis → the proposed approach and how it
works → evidence that it works (cases, data) → implementation considerations → conclusion and
call to action → references. Persuasive but evidence-bound: mark marketing claims as claims, and
cite independent evidence for key assertions.

## 9. Tables, figures, and numbers

- Each table or figure has a numbered, self-explanatory title, units, the source, the n or period,
  and is referenced in the text.
- Round sensibly and consistently; state the base for percentages; distinguish % from percentage points.
- Choose the chart for the message: comparison → bar; trend → line; part-to-whole → stacked bar
  (avoid pie charts with more than 3 slices); distribution → histogram or box plot; relationship → scatter.
- Don't truncate axes to exaggerate differences. Label directly where possible, and don't rely on
  colour alone.
- Keep the same number the same everywhere (summary, body, tables). Mismatches destroy credibility.

## 10. Report QA

Before delivery, run the **report QA checklist** and the **self-critique pass** in
`final-checklists.md`.
