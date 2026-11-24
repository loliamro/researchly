# Citations

**Owns:** in-text citations, reference lists and bibliographies, style choice and conversion,
completing and auditing references, citation integrity, and BibTeX/LaTeX citation mechanics.
**Use when:** "format my references", "convert to IEEE", "is this APA correct?", "check my
citations match my reference list", "make BibTeX for these DOIs", "cite this website".
**Don't use when:** the question is whether a source is *trustworthy* or *supports* a claim
(`source-evaluation-and-fact-checking.md`).

## Contents
1. Integrity rules
2. Choosing the style (suite standard)
3. APA 7 essentials
4. Other common styles
5. Completing and verifying references
6. Auditing a document
7. BibTeX and LaTeX
8. Citing tricky sources

---

## 1. Integrity rules

1. **Never invent** an author, title, year, venue, volume, pages, DOI, URL, or quotation. If a
   field is unknown and can't be found, leave it out per the style's rules or mark it `[MISSING: field]`.
2. **A reference must be a real, specific work** that you or the user have seen. If you recall a
   work from memory and can't open it, label it `[UNVERIFIED — check before use]`.
3. **Cite what you read.** If you only saw a work quoted in another source, cite it as secondary
   ("as cited in"), or find and read the original.
4. **A DOI that resolves isn't proof.** Confirm that the DOI, title, authors, and year all belong to
   the same work and that the work says what you attribute to it.
5. **Prefer the version of record** over a preprint once published, and note retractions or corrections.
6. **Placeholders:** use `[CITATION NEEDED]` in drafts where support is still to be found. Never
   fill one with a plausible-looking reference.

## 2. Choosing the style (suite standard)

Use the first that applies:
1. The style the user, instructor, publisher, or venue requires (ask once if unclear and it matters).
2. The style already used consistently in the user's document.
3. The field default: APA 7 for social sciences, education, psychology, and business; IEEE for
   engineering and computing; Vancouver/NLM or AMA for medicine; Chicago notes-bibliography for
   history and humanities; MLA 9 for literature and languages; Harvard where a UK institution expects it.
4. Otherwise **APA 7** for academic work and **numbered [1]** (IEEE-like) for research briefs
   and professional reports.

Announce any style switch in one line. Never mix styles within one document.

**Research feeding academic work:** if a research brief or literature review is meant for a
student essay, thesis, or paper, use that work's style (e.g., APA 7) from the start rather than
numbered references, so the user can paste it in without reformatting.

## 3. APA 7 essentials

**In-text:** (Author, Year) or Author (Year).
- Two authors: (Smith & Lee, 2020) in parentheses, "Smith and Lee (2020)" in narrative.
- Three or more authors: (Smith et al., 2020) from the first citation.
- Group author: (World Health Organization [WHO], 2023) first time, then (WHO, 2023).
- Direct quotes need a page or locator: (Smith, 2020, p. 14) or (para. 3).
- Several works: semicolons, alphabetical: (Lee, 2019; Smith, 2020).
- No date: (Author, n.d.).

**Reference list:** alphabetical by first author, hanging indent, double-spaced in manuscripts.
- Journal article: Author, A. A., & Author, B. B. (Year). Title of article in sentence case.
  *Journal Name in Title Case*, *Volume*(Issue), pages. https://doi.org/xx.xxxx
- Book: Author, A. A. (Year). *Title of book* (2nd ed.). Publisher. https://doi.org/… (if any)
- Chapter: Author, A. A. (Year). Chapter title. In E. E. Editor (Ed.), *Book title* (pp. x–y). Publisher.
- Webpage: Author or Organization. (Year, Month Day). *Title*. Site Name (omit if it is the
  author). URL. Add "Retrieved Month Day, Year, from URL" only for pages designed to change.
- Report: Organization. (Year). *Title* (Report No. x). Publisher (omit if same as author). URL
- Dataset: Author. (Year). *Title* (Version x) [Data set]. Publisher. https://doi.org/…
- Software or AI tool: Developer. (Year). *Name* (Version) [Computer software or Large language
  model]. URL. Follow current APA guidance and the instructor's or venue's policy on AI-use disclosure.
- Up to 20 authors listed; for 21 or more: first 19, ellipsis, last author.
- DOIs as https://doi.org/ links; no "Retrieved from" before DOIs; no publisher location for books.

## 4. Other common styles (quick patterns)

| Style | In-text | Journal reference pattern |
|---|---|---|
| **IEEE** | [1], numbered in order of first citation | [1] A. Author and B. Author, "Title," *Abbrev. Journal*, vol. x, no. y, pp. a–b, Mon. Year, doi: … |
| **Vancouver / NLM** | Superscript or (1), order of citation | 1. Author AA, Author BB. Title. Abbrev Journal. Year;Vol(Issue):pages. doi:… |
| **Chicago author-date** | (Smith 2020, 14) | Smith, Ann, and Bo Lee. 2020. "Title." *Journal* 12 (3): 45–67. https://doi.org/… |
| **Chicago notes-bibliography** | Footnote numbers | Note: 1. Ann Smith, "Title," *Journal* 12, no. 3 (2020): 45. |
| **MLA 9** | (Smith 14) | Smith, Ann, and Bo Lee. "Title." *Journal*, vol. 12, no. 3, 2020, pp. 45–67, https://doi.org/… |
| **Harvard** | (Smith, 2020) or (Smith 2020) | Smith, A. and Lee, B. (2020) 'Title', *Journal*, 12(3), pp. 45–67. Check the local variant. |

For details beyond these patterns, follow the official manual or the venue's author guide. Say so
when a case is unusual rather than guessing.

## 5. Completing and verifying references

For each reference:
1. Identify it by DOI, PMID, arXiv ID, ISBN, or exact title plus first author.
2. Get the metadata from the publisher page, the DOI record, or a bibliographic database. Check
   that the title, authors (spelling and order), year, venue, volume/issue/pages or article number,
   and DOI agree.
3. Handle online-first articles without volume or pages: use the article number or "Advance online
   publication" per the style; never invent pages.
4. Replace preprints with the published version if one exists, unless the user cites the preprint deliberately.
5. Record anything unresolved as `[MISSING: …]` and list it for the user.

If you can't access the web, format from the information given and list every field you couldn't verify.

## 6. Auditing a document

Produce a table and then fixes:
```markdown
| Issue | Location | Detail | Fix |
|---|---|---|---|
| Cited but not in list | p. 3, (Kim, 2021) | No matching entry | Add entry or remove citation |
| In list but never cited | Ref list: Patel 2018 | — | Remove or cite |
| Mismatch | (Smith, 2019) vs. list "Smith 2020" | Year differs | Check source; correct one |
| Incomplete | Lee 2022 | No DOI/pages | Add from publisher record |
| Style error | Jones et al. | "&" used in narrative citation | "Jones and Lee (2020)" |
```
Also check: consistent style; "et al." rules; page numbers for quotes; alphabetical or numeric
order; duplicate entries for one work; and secondary citations marked as such.

## 7. BibTeX and LaTeX

- One entry per work with a stable key (e.g., `smith2020remote`). Use `@article`, `@book`,
  `@incollection`, `@inproceedings`, `@techreport`, `@misc` (web, software, data), or `@phdthesis`.
- Required fields for `@article`: author, title, journal, year (plus volume, number, pages, doi).
- Authors as `Last, First and Last, First`; protect capitals in titles with braces: `{COVID}-19`, `{B}ayesian`.
- Escape special characters (`\&`, `\%`, `{\"u}`), or use UTF-8 with biblatex and biber.
- LaTeX: `\cite{key}` for numeric styles; with natbib, `\citet{}` (narrative) and `\citep{}`
  (parenthetical); with biblatex, `\textcite{}` and `\parencite{}`. APA in LaTeX: `biblatex` with `style=apa`.
- Compile order: LaTeX → BibTeX/biber → LaTeX → LaTeX. Undefined citations usually mean a key
  mismatch or a skipped bibliography step.
- Build BibTeX from verified metadata, never from memory.

## 8. Citing tricky sources

- **Lecture slides and course materials:** cite only if the instructor allows it, as the style
  directs; prefer the underlying published source.
- **Personal communications** (APA): in-text only, "(A. Smith, personal communication, May 2, 2025)", no reference entry.
- **Social media:** author, handle, date, the first 20 words of the post as title, platform, URL.
- **Generative-AI output:** follow the instructor's or venue's policy. Many require disclosure
  rather than citation, and AI output is not a source for factual claims.
- **Translated or classic works:** cite the edition used and include the original date where the style allows it.
- **Secondary citations:** "(Freud, 1923, as cited in Lee, 2019)". Only Lee goes in the reference list (APA).
