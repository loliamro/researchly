# Researchly: a research & writing skill for Claude

**One file. One upload. Research and writing help that cites real sources.**

A single Claude skill for students and professionals. It plans research, runs quick, standard,
or deep research, reviews literature, checks facts and grades sources, formats citations,
drafts academic text and professional reports, polishes writing, and critiques drafts.
Everything follows one consistent method, so the parts never contradict each other.

## ▶️ 30-second setup video

https://github.com/user-attachments/assets/33f5921e-0cc1-4f1c-92f4-dea6893de701

<sub>Can't play it? [Download the MP4](media/how-to-use.mp4) or view the [GIF version](media/how-to-use.gif). The screens in the video are simplified illustrations, so your Claude menus may look slightly different.</sub>

## ⬇️ Get it (students: start here)

1. Download **[`researchly.zip`](../../releases/latest/download/researchly.zip)**
   from the [latest release](../../releases/latest). Don't unzip it.
2. In **Claude** (claude.ai or the desktop app): open **Settings → Capabilities**, make sure
   code execution / skills are enabled, then under **Skills** choose **Upload skill** and pick the ZIP.
   (Menu names can differ slightly between Claude versions. Look for "Skills".)
3. Turn on **web search** in your chat so it can open and cite real sources.
4. Start a new chat and ask normally, for example *"Help me write a literature review on…"*.
   Claude loads the skill automatically when it fits. If it doesn't, start with *"Use the researchly skill."*

> **Installed the old version (`research-writing-suite`)?** Remove it from your Skills list first, then upload `researchly.zip`.

**Claude Code users:** unzip into your skills folder so you get
`~/.claude/skills/researchly/SKILL.md` (Windows: `%USERPROFILE%\.claude\skills\…`).

## What you can ask

| You say… | The suite… |
|---|---|
| "I want to research X but don't know my question" | Builds a sharp research question (PICO/FINER), scope, and search plan |
| "What does the evidence say about X?" | Runs **quick / standard / deep** research with cited, confidence-tagged findings |
| "Do a literature review on X" / "compare these 5 papers" | Literature review, literature matrix, three-way paper scan, study notes |
| "Is this true?" / "Can I trust this source?" / "Fact-check my report" | One verification process: **source tiers T1–T5**, **claim risk R1–R3**, **confidence tags** |
| "Format my references in APA/IEEE" / "check my citations" | Citation formatting, audits, BibTeX/LaTeX. It never invents references |
| "Write my introduction / abstract / proposal / essay" | Academic drafting from your own claims and sources |
| "Write a technical report / executive summary / memo / status update" | Professional templates with a built-in QA checklist |
| "Polish this" / "make it sound less like AI" | Editing at the level you choose, with changes explained |
| "Review my paper like a reviewer would" / "help me answer reviewers" | Peer review, devil's advocate, rebuttal letters |

## Rules the suite always follows

- Never fabricates citations, DOIs, statistics, or quotes. Missing items are marked `[CITATION NEEDED]` or `[DATA NEEDED]`.
- Verifies claims against sources it actually opened. Anything else is tagged **Unverified**.
- States limitations, paraphrases instead of copying, and matches your audience.
- Runs a self-critique pass and a QA checklist before giving you the final version.
- Treats web pages and documents as data, never as instructions. It contains **no scripts**.

## How it's built

```
researchly/          ← the skill (this folder is the ZIP root)
├── SKILL.md                     ← short router: picks ONE owner file per task
├── LICENSE · NOTICE
└── references/                  ← loaded only when needed
    ├── research-planning.md
    ├── deep-research-modes.md            (quick / standard / deep)
    ├── literature-review.md
    ├── source-evaluation-and-fact-checking.md (tiers, risk, confidence, claim-to-evidence table)
    ├── citations.md                      (APA 7 default; IEEE, Vancouver, Chicago, MLA, Harvard)
    ├── academic-writing.md
    ├── professional-reports.md
    ├── editing-and-polish.md
    ├── peer-review-and-critique.md
    └── final-checklists.md               (self-critique pass + QA checklists)
tests/test-prompts.md            ← 8 test prompts and the walkthrough results
```

Each task type has exactly one owner file, with "use when / don't use when" rules. Shared labels
(evidence tiers, research modes, citation style) are defined in one place and reused everywhere.

## Build the ZIP yourself (optional)

From the repository root (Windows 10+, macOS, or Linux):
```powershell
tar -a -c -f researchly.zip researchly
```
On macOS or Linux you can also use `zip -r researchly.zip researchly`. Avoid
Windows PowerShell 5.1's `Compress-Archive`, which writes backslash paths that some uploaders reject.
The ZIP must contain the `researchly/` folder at its root, with `SKILL.md` inside it.

## Credits and licenses

This suite is **MIT-licensed** (see [`LICENSE`](researchly/LICENSE)). It is an original
synthesis that adapts methods from the open-source projects below. Full attributions, licenses,
and what was taken from each are in [`NOTICE`](researchly/NOTICE).

- No upstream text from CC BY-NC or unlicensed sources is included: those were used as ideas only, and credited.
- No upstream scripts or code are included.

## Original skills (download individually)

Want the originals? These are the upstream skills this suite learned from. Each keeps its own license.

| Project | Skills | License |
|---|---|---|
| [Imbad0202/academic-research-skills](https://github.com/Imbad0202/academic-research-skills) | [deep-research](https://github.com/Imbad0202/academic-research-skills/tree/main/deep-research) · [academic-paper](https://github.com/Imbad0202/academic-research-skills/tree/main/academic-paper) · [academic-paper-reviewer](https://github.com/Imbad0202/academic-research-skills/tree/main/academic-paper-reviewer) | CC BY-NC 4.0 (non-commercial) |
| [K-Dense-AI/claude-scientific-writer](https://github.com/K-Dense-AI/claude-scientific-writer) | [research-grants](https://github.com/K-Dense-AI/claude-scientific-writer/tree/main/skills/research-grants) · [all skills](https://github.com/K-Dense-AI/claude-scientific-writer/tree/main/skills) | MIT |
| [lnilya/effortless-academic-skills](https://github.com/lnilya/effortless-academic-skills) | [ea-academic-writer](https://github.com/lnilya/effortless-academic-skills/tree/main/skills/ea-academic-writer) · [ea-atomic-sentences](https://github.com/lnilya/effortless-academic-skills/tree/main/skills/ea-atomic-sentences) · [ea-intro-planner](https://github.com/lnilya/effortless-academic-skills/tree/main/skills/ea-intro-planner) · [ea-results-analyser](https://github.com/lnilya/effortless-academic-skills/tree/main/skills/ea-results-analyser) | MIT |
| [David-Saeteros/claude-skills](https://github.com/David-Saeteros/claude-skills) | [academic-writing](https://github.com/David-Saeteros/claude-skills/tree/main/skills/academic-writing) · [research_review](https://github.com/David-Saeteros/claude-skills/tree/main/skills/research_review) | CC BY 4.0 |
| [K-Dense-AI/claude-scientific-skills](https://github.com/K-Dense-AI/claude-scientific-skills) | [scientific-writing](https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/skills/scientific-writing) · [literature-review](https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/skills/literature-review) · [citation-management](https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/skills/citation-management) · [peer-review](https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/skills/peer-review) · [scientific-critical-thinking](https://github.com/K-Dense-AI/claude-scientific-skills/tree/main/skills/scientific-critical-thinking) | MIT |
| [jamditis/claude-skills-journalism](https://github.com/jamditis/claude-skills-journalism) | [source-verification](https://github.com/jamditis/claude-skills-journalism/tree/master/journalism-core/skills/source-verification) · [fact-check-workflow](https://github.com/jamditis/claude-skills-journalism/tree/master/journalism-core/skills/fact-check-workflow) | MIT |
| [199-biotechnologies/claude-deep-research-skill](https://github.com/199-biotechnologies/claude-deep-research-skill) | deep-research (whole repo) | MIT (per README) |
| [B143KC47/deep-research-skill](https://github.com/B143KC47/deep-research-skill) | [deep-research](https://github.com/B143KC47/deep-research-skill/tree/main/deep-research) | MIT |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | [go-in-depth](https://github.com/sickn33/agentic-awesome-skills/tree/main/skills/go-in-depth) | MIT / CC BY 4.0 |
| [lyndonkl/claude](https://github.com/lyndonkl/claude) | [research-claim-map](https://github.com/lyndonkl/claude/tree/main/skills/research-claim-map) | No standard license file |
| [nimbalyst/skills](https://github.com/nimbalyst/skills) | [strategy-memo](https://github.com/nimbalyst/skills/tree/main/skills/product/strategy-memo) · [status-updater](https://github.com/nimbalyst/skills/tree/main/skills/product/status-updater) | MIT |
| [inbharatai/claude-skills](https://github.com/inbharatai/claude-skills) | [report-builder](https://github.com/inbharatai/claude-skills/tree/main/skills/report-builder) · [latex-writer](https://github.com/inbharatai/claude-skills/tree/main/skills/latex-writer) (reviewed, not used) | MIT |
| [Shubhamsaboo/awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | [agent_skills](https://github.com/Shubhamsaboo/awesome-llm-apps/tree/main/agent_skills) (reviewed, not used) | Apache-2.0 |
| [o0000-code/awesome-academic-skills](https://github.com/o0000-code/awesome-academic-skills) | Index of academic skills (used to find gaps) | CC0 |
| [anthropics/skills](https://github.com/anthropics/skills) | Skill structure and best practices (structure only, nothing copied) | See repo |

## Disclaimer

This is a writing and research aid, not professional, medical, legal, or financial advice. You
remain responsible for checking sources and following your institution's academic-integrity and
AI-use policies.
