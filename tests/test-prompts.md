# Test prompts and walkthrough results

Eight realistic prompts were traced through the router (`SKILL.md`) and the owner files. For
each, we recorded the route, what the suite produces, and any gap, overlap, or contradiction
found, plus the fix applied. Re-run these after any change to the suite.

| # | Prompt | Route (owner → helpers) | Expected output |
|---|---|---|---|
| 1 | "Write a literature review on how social media use affects sleep in teenagers, about 2,000 words, APA." | literature-review → deep-research-modes §3 (standard budget), source-evaluation (grading), citations (APA 7), final-checklists C | Type labelled (narrative, systematic-style search), documented searches, thematic synthesis, gaps, APA references, limitations |
| 2 | "Here are my bench test results for a 6 V lead-acid charger. Write a technical report for my lab course." | professional-reports §4 (lab variant) → final-checklists E | Lab-report structure; results from the user's data cited as data; error analysis; no invented numbers |
| 3 | "Polish this abstract and get it under 250 words." (pasted) | editing-and-polish §8, §5 → academic-writing §5 (structure check) | Clean version, word count before/after, change list; content cuts flagged |
| 4 | "Help me write a master's research proposal on microplastics in drinking water." | research-planning → literature-review (quick) → academic-writing §6 → final-checklists D | Research question with FINER check, then a proposal draft with aims, methods, risks, and timeline; `[CITATION NEEDED]` where unsourced |
| 5 | "Which of these should I trust for my essay on intermittent fasting: a WHO page, a Medium blog, a 2019 RCT?" | source-evaluation (rubric §3, tiers §2) | Tier and rubric score per source for the specific claims; recommendation of what to cite and how |
| 6 | "Is it true we only use 10% of our brains? Give me sources." | source-evaluation (single-claim format), searched at quick/standard budget | Verdict "Contradicted · High", origin of the myth, numbered T1/T2 sources |
| 7 | "Review my paper before I submit it to a journal: what will reviewers say?" | peer-review-and-critique (self-review template) + §5 devil's advocate | Readiness verdict, issue table by severity, claim-evidence check, strongest objection |
| 8 | "Turn my project findings into an executive summary for my manager and a weekly status update for the team." | professional-reports §3 + §7 → final-checklists E | Standalone executive summary (≤1 page) and a status update with owners and dates |

## Issues found and fixed

| # | Found in prompt | Type | Problem | Fix |
|---|---|---|---|---|
| 1 | 6 | Overlap | `deep-research-modes` listed "verifying a contested claim" while `source-evaluation` also owns claim verification. Both could fire. | Deep research now owns *open questions*; source-evaluation owns *verifying given claims*. Added a single-claim answer format and a rule to borrow search budgets without switching owners. |
| 2 | 5 | Overlap | "Compare these sources/papers" matched both literature-review (paper comparison) and source-evaluation. | Router tie-breaker: comparing **content** → literature-review; comparing **trustworthiness** → source-evaluation; if both, grade first. |
| 3 | 2 | Gap | The "cite every factual claim" rule didn't say how to cite the user's own data. | professional-reports §1: the user's data is a source; cite it by name and locator; label projections. |
| 4 | 1, 4 | Contradiction | Research briefs default to numbered citations, but students paste research into APA essays. | citations §2: research feeding academic work uses that work's style from the start. |
| 5 | 4, 5 | Gap | No structure for a student course essay (the most common student task). | academic-writing §4: course-essay structure with thesis statement and rubric mapping. |
| 6 | Design | Contradiction (sources) | Sources disagreed on evidence thresholds ("3+ sources per claim" vs. "primary + independent corroboration"). | One standard: risk-based minimums (R1–R3) in source-evaluation §4; source counts are mode targets, not gates. |
| 7 | Design | Contradiction (sources) | One source required three paragraph variants on every output; another required one clean version. | One version by default; cautious and assertive variants only for key claim sentences or on request. |
| 8 | Design | Contradiction (sources) | "Flag before rewriting" vs. "operate autonomously". | Suite standard: light edits applied directly; substantive changes flagged first; research proceeds on stated defaults. |
| 9 | Design | Contradiction (sources) | Citation styles differed (APA, Vancouver, numeric, evidence IDs). | One decision table in citations §2; evidence IDs used only inside the claim-to-evidence table. |

## Structure tests (run on the ZIP)

- The ZIP root contains exactly one folder, `research-writing-suite/`, with `SKILL.md` directly inside.
- The `SKILL.md` frontmatter has `name` = folder name (lowercase, hyphens, ≤ 64 chars) and a `description` ≤ 1024 chars.
- Every `references/…` path mentioned in `SKILL.md` exists.
- No executable files (`.py`, `.js`, `.sh`, `.ps1`, `.exe`) are in the ZIP.
