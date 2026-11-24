# Research Planning

**Owns:** turning a topic into a researchable question, scoping, and planning the search or study.
**Use when:** the user has a vague topic, asks "what should I research", needs a research
question, aims, scope, or a search plan, or is about to start a literature review, proposal, or
deep research and the question is not yet sharp.
**Don't use when:** the question is already precise. Go straight to `deep-research-modes.md` or
`literature-review.md`. Don't use it to write the proposal itself (`academic-writing.md`).

## Contents
1. Intake
2. Research-question builder
3. Scope and boundaries
4. Aspect map (what could change the answer)
5. Search plan
6. Study/analysis plan (empirical projects)
7. Output: the research brief

---

## 1. Intake

Capture these fields, inferring the obvious ones and stating your assumptions in one line.

| Field | Question |
|---|---|
| Purpose | Decide, learn, publish, propose, or teach? What will the answer be used for? |
| Deliverable | Answer, brief, literature review, report, proposal, paper section? |
| Audience | Expert, general, executive, reviewer/committee? |
| Freshness | Does recency matter (prices, policy, software, fast-moving science)? Cut-off date? |
| Risk | What happens if the answer is wrong? Low / medium / high (health, legal, financial, safety, reputational). |
| Constraints | Time, word limit, region/jurisdiction, language, required sources or style, no-browse. |
| Materials | Files or papers the user supplied, and whether they are trusted inputs or claims to check. |

Ask a clarifying question only when the missing detail would change the research target. A
budget, region, or population can change the answer; a font preference can't. Use at most 2–3
questions, then proceed.

## 2. Research-question builder

Work through these five steps, showing the user steps 2–5 briefly.

**Step 1: Name the topic and the problem.** One sentence each: the area, and what is unknown,
contested, or costly about it.

**Step 2: Pick the question type.** The type sets the method.

| Type | Template | Typical method |
|---|---|---|
| Descriptive | What is the level/pattern of X in P (during T)? | Survey, data analysis, scoping review |
| Comparative | How does X differ between A and B in P? | Comparative study, structured comparison |
| Relational | Is X associated with Y in P? | Correlational/observational |
| Causal / intervention | Does I, compared with C, change O in P over T? | Experiment, quasi-experiment, systematic review |
| Explanatory / mechanism | How/why does X lead to Y? | Qualitative, process tracing, theory synthesis |
| Evaluative / decision | Which option best meets criteria K for stakeholder S? | Decision matrix, deep research |
| Methodological | How well does method M measure/estimate X? | Validation study, benchmark |

**Step 3: Structure it.** Use **PICO(T)** for intervention or causal questions: Population,
Intervention/exposure, Comparator, Outcome, Time. Use **PEO** for qualitative questions:
Population, Exposure/phenomenon, Outcome/experience. Use **SPIDER** for mixed or qualitative
evidence syntheses. For decision questions use **Options × Criteria × Stakeholder × Context**.

**Step 4: Score it with FINER.** Rate each item 1–3 and fix anything scored 1:

| Criterion | Check |
|---|---|
| Feasible | Answerable with available time, data, access, and skills? |
| Interesting | Does the answer matter to the stated audience? |
| Novel | Does it add something beyond what is already settled? For a decision question, is it unanswered for *this* context? |
| Ethical | Any harm, consent, privacy, or dual-use concern? |
| Relevant | Does the answer change a decision, theory, or practice? |

**Step 5: Rewrite it.** Produce three versions, a **narrow**, a **balanced** (recommended), and an
**ambitious** one, each with one line on the trade-off. Then list 2–5 **sub-questions** that
together answer the main question.

**Common fixes:**
- Too broad ("AI in education"): add population, outcome, and setting.
- Yes/no with an obvious answer: ask *how much*, *for whom*, or *under what conditions*.
- Two questions in one: split them.
- Value-laden ("Is X bad?"): convert to measurable criteria.
- Unanswerable with evidence ("Will X happen?"): reframe as drivers, scenarios, or current indicators.

**Socratic option.** If the user is unsure what they want to ask, guide them with short questions
in this order: *What made you curious? → Who is affected? → What would count as an answer? →
What would surprise you? → What can you actually access?* Then return to Step 2.

## 3. Scope and boundaries

State in the plan:
- **In scope / out of scope:** populations, settings, time window, languages, source types.
- **Key terms and definitions:** including synonyms and aliases for search.
- **Assumptions:** the defaults you inferred.
- **Success criterion:** what a sufficient answer looks like (e.g., "a ranked recommendation with
  the evidence for each option" or "a thematic synthesis of studies since 2015").

## 4. Aspect map

List what could change the answer and where that evidence lives. This prevents searching only
the easy sources.

| Aspect | Example | Source classes |
|---|---|---|
| Definitions and scope | Terms, standards, entities | Standards bodies, textbooks, official docs |
| Authoritative anchors | Laws, official statistics, filings, specifications | Government, regulators, official sites |
| Research evidence | Studies, reviews, replications | Databases, journals, preprint servers |
| Practice and implementation | How it works in reality | Documentation, code, case studies, practitioner reports |
| Data | Datasets, benchmarks | Data portals, benchmark sites |
| Counterevidence | Critiques, failures, null results, retractions | Commentaries, replication studies, issue trackers, retraction notices |
| Stakeholder views | Positions, incentives | Organizations, interviews, reputable journalism |

## 5. Search plan

- **Concept blocks:** one block per PICO/PEO element; combine synonyms with OR within a block and
  blocks with AND. Add exclusions with NOT sparingly.
- **Routes:** at least three distinct routes, for example an authoritative/official route, a
  scholarly route, a practice or data route, and always a **counterevidence** route ("limitations",
  "criticism", "failed", "replication", "retraction").
- **Where:** pick by discipline. Examples: PubMed or Cochrane (health), ERIC (education), PsycINFO
  (psychology), IEEE Xplore or ACM DL (computing), SSRN or RePEc (economics), Google Scholar,
  OpenAlex, or Semantic Scholar (cross-disciplinary), arXiv, bioRxiv, or medRxiv (preprints).
  These are places to search. Read whatever you cite.
- **Record:** the date, each query string, the database, and the result count. This is mandatory
  for systematic work and good practice everywhere.
- **Depth:** choose the mode (quick / standard / deep) from `deep-research-modes.md` by risk and
  deliverable.

## 6. Study / analysis plan (empirical projects only)

Use this when the user is designing a study rather than only reviewing literature:
- **Design** that matches the question type (Step 2 table) and the unit of analysis.
- **Variables and measures,** with how each is operationalised and its known reliability and validity.
- **Sampling:** population, frame, size rationale (power or precision), inclusion/exclusion.
- **Analysis:** the pre-specified primary analysis, secondary and exploratory analyses labelled as such,
  and how missing data and multiple comparisons are handled.
- **Threats to validity:** confounding, selection, measurement, attrition, generalisability, and the
  mitigation for each.
- **Ethics:** approvals needed, consent, data protection, and whether pre-registration is appropriate.

## 7. Output: the research brief

```markdown
## Research brief: [short title]
**Question (recommended):** …
**Alternatives:** Narrow: … | Ambitious: …
**Sub-questions:** 1. … 2. … 3. …
**Type & framework:** [e.g., causal; PICO = …]
**FINER check:** F_/3 I_/3 N_/3 E_/3 R_/3. [one-line note on any weakness]
**Scope:** In: … | Out: … | Time window: … | Assumptions: …
**Aspect map & routes:** [table or bullets]
**Mode:** quick / standard / deep. [one-line reason]
**Success criterion:** …
**Next step:** [owner file that runs next]
```
