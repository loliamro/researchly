# Literature Review

**Owns:** finding, screening, extracting, appraising, and synthesizing scholarly literature;
literature maps; paper-by-paper comparisons; extracting the claims a paper attributes to its
citations; study notes from papers; and writing the literature-review section or standalone review.
**Use when:** "do a literature review on…", "what does the research say about…" (scholarly
focus), "compare these papers", "summarise these 10 PDFs", "extract the key claims from this
paper", "map the field", "find gaps".
**Don't use when:** the question is practical or current and not mainly scholarly
(`deep-research-modes.md`), or the user only needs one claim checked
(`source-evaluation-and-fact-checking.md`). Prose polishing of an existing review belongs to
`editing-and-polish.md`.

Depth: use the quick / standard / deep budgets in `deep-research-modes.md` §3. Grade sources with
`source-evaluation-and-fact-checking.md`. Format references per `citations.md` (APA 7 default).

## Contents
1. Pick the review type
2. Workflow
3. Extraction: literature matrix
4. Appraisal
5. Synthesis methods
6. Lightweight formats: three-way scan, atomic claims, study notes
7. Writing the review
8. Pitfalls

---

## 1. Pick the review type

| Type | Purpose | Rigor requirements |
|---|---|---|
| **Narrative / background** | Position a study; explain a field | Representative, balanced coverage; explicit search description encouraged |
| **Scoping** | Map what exists, concepts, and gaps | Documented search, inclusion criteria, charting; no quality-based exclusion (PRISMA-ScR) |
| **Systematic** | Answer a focused question with all eligible evidence | Protocol, reproducible multi-database search, dual screening (or a disclosed single-reviewer limitation), risk-of-bias appraisal, PRISMA 2020 reporting |
| **Rapid** | Systematic-like under time pressure | Same as systematic but with stated shortcuts |
| **Meta-analysis** | Pool effect estimates quantitatively | Systematic review plus compatible outcomes and statistical expertise. This suite plans and reports; it doesn't compute. |
| **Paper comparison** | Compare a shortlist of papers quickly | Three-way scan (§6) |

Tell the user honestly what an AI-assisted process can do: a narrative or scoping review is
realistic, but a full systematic review needs database access, full texts, and a second human
screener. Label anything short of that accordingly (e.g., "systematic-style search, single reviewer").

## 2. Workflow

1. **Question and criteria.** Get a sharp question (from `research-planning.md` if needed). Write
   inclusion and exclusion criteria **before** screening: population, concept or intervention,
   context, study designs, dates, and languages.
2. **Search.** Use concept blocks with synonyms, two or more disciplinary databases where possible,
   plus citation chasing (backward: reference lists; forward: "cited by") and preprints if the field
   uses them. Record the database, the query, the date, and the count for every search.
3. **Deduplicate.** Remove duplicate records, then link multiple reports of the same study (preprint
   + journal version + follow-up) so one study isn't counted twice.
4. **Screen.** Screen titles and abstracts, then full text against the criteria. Record exclusion
   reasons at the full-text stage. Citation counts can order your reading but must never decide
   eligibility.
5. **Extract.** Fill the literature matrix (§3) from the **full text**, not abstracts alone, for
   included studies. If the full text isn't available, say so.
6. **Appraise.** Assess quality or risk of bias with a tool that fits the design (§4).
7. **Synthesize.** Synthesize by theme, not study by study (§5).
8. **Write** (§7), then run `final-checklists.md` (literature-review checklist + self-critique pass).

For systematic and scoping reviews, keep PRISMA counts: records identified, duplicates removed,
records screened, reports sought, reports not retrieved, reports assessed, reports excluded with
reasons, and studies included.

## 3. Extraction: literature matrix

```markdown
| Study (Author Year) | Question/aim | Design & sample | Setting | Measures/intervention | Key findings (with numbers) | Limitations (named) | Quality/RoB | Relevance/theme |
|---|---|---|---|---|---|---|---|---|
```

Write findings with numbers, direction, and units ("reduced X by 12%, 95% CI 4–20"), not "had a
positive effect". Name limitations concretely: give the design choice and the condition under
which it would distort the result ("n = 24 from one site, so effects may not generalise beyond
specialist clinics"), not "small sample".

## 4. Appraisal

Match the tool to the design and name it; don't turn checklists into a single score:
- Randomised trials: **RoB 2**, judged per outcome.
- Non-randomised interventions: **ROBINS-I**.
- Observational: **Newcastle–Ottawa** or **JBI** checklists.
- Qualitative: **CASP** qualitative or **JBI**.
- Diagnostic accuracy: **QUADAS**.
- Systematic reviews: **AMSTAR 2**.
- Certainty of a body of evidence per outcome: **GRADE**.

Check the current version of each tool before a formal assessment. Keep three things separate:
reporting completeness, risk of bias, and certainty of the overall evidence.

## 5. Synthesis methods

- **Thematic synthesis (default):** cluster studies by concept, mechanism, or finding; for each
  theme, state what the studies agree on, where they disagree and why (design, population,
  measures, period), and how strong the evidence is.
- **Framework synthesis:** organise by an established theory or model when one fits.
- **Chronological:** only when the development of the idea *is* the argument.
- **Methodological:** compare how different methods produce different answers.
- **Narrative synthesis of quantitative studies (SWiM-style):** group by outcome, report direction
  and size consistently, and explain heterogeneity. Don't count votes ("7 positive vs. 3 negative")
  as evidence of effect.

**Gap analysis:** for each theme, note what is missing: populations, settings, methods,
long-term outcomes, replications, or conflicting results never resolved. A gap is a claim too.
Support it with your search ("no studies in the 2015–2025 searches examined…").

**Literature map (optional table):**
```markdown
| Theme/cluster | Representative studies | Core idea | Strength of evidence | Open questions |
|---|---|---|---|---|
```

## 6. Lightweight formats

**Three-way scan (rapid paper comparison).** For each paper:
```markdown
### [Author Year] [Title]
- WHY: the problem or gap it addresses and why it matters
- HOW: design, data, and method
- WHAT: the main finding, with numbers, plus its named method weakness
```
Then a cross-paper synthesis: the shared WHY, the divergent HOW, the conflicting or complementary
WHAT, and the remaining gaps.

**Atomic claims (what a paper's citations say).** When the user wants to map the literature *as a
paper presents it*: collect every in-text citation; for each, write one sentence stating the
specific claim the citing author attributes to it, keeping numbers exact; group the claims by
sub-topic; end each group with a one-sentence synthesis. Mark these as *claims attributed by the
citing paper*. They are Unverified about the cited works until those are opened. If a citation's
role is ambiguous, flag it rather than inventing a claim.

**Study notes from a paper.** For students reading a paper:
```markdown
**Citation:** [APA 7]
**In one sentence:** …
**Question & why it matters:** …
**Method:** design, sample, measures
**Results (3–5, with numbers):** …
**Authors' interpretation:** …
**Limitations (named):** …
**How it connects to [my topic]:** …
**Quotes worth keeping (with page):** …
**Questions I still have:** …
```
For review papers, replace "Results" with "Main claims and the evidence base".

## 7. Writing the review

**Structure (standalone review):** introduction (question, why it matters, scope) → methods
(search, criteria, screening, appraisal, synthesis) → results (study characteristics, then
themes) → discussion (what the evidence shows, its strength, gaps, implications) → limitations
of the review → conclusion → references. For a review *section* inside a paper or thesis, see
`academic-writing.md` §4.

**Paragraph pattern:** a topic sentence that makes a claim about the literature, then the
evidence (several citations compared, not listed), then the qualification or contrast, then a link
to the next theme or to the study's gap.

- Weak: "Smith (2019) studied X. Lee (2020) studied Y. Chen (2021) studied Z."
- Strong: "Studies agree that X improves Y in short trials (Smith, 2019; Lee, 2020), but the only
  long-term cohort found no lasting effect (Chen, 2021), which suggests the benefit may fade."

Report the evidence strength in words consistent with the appraisal, and show disagreements;
don't hide them.

## 8. Pitfalls

Searching a single database; undocumented searches; summarising study by study; treating a DOI's
existence as proof that the work supports the claim; citing from abstracts alone for central
claims; ignoring preprint-to-journal updates and retractions; including predatory-journal papers;
overstating "the literature shows" when it is a few small studies; and omitting the search date.
