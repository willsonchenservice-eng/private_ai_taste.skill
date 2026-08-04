# Calibration Log

Use this file to turn samples and real revisions into testable style rules.

## Evidence index

| ID | Sample | Mode | Strong signals | AI-assisted? | Current endorsement? |
|---|---|---|---|---|---|
| S1 | 《一起看看〈微信背后的产品观〉》 | Professional reflection | Personal time contrast; source idea → product case → own judgment; many concrete work applications | Unknown | Assumed for V1 |
| S2 | 《知和行的 5 个阶段：你在哪一阶段？怎么破？》 | Life reflection | Designer frustration; five-stage model; billiards analogy; actionable ending | Unknown | Assumed for V1 |
| S3 | 《佐藤大：用设计解决问题》读书感想 | Professional reflection | Self-introduction; playful humor; source stories; numbered design lessons; work transfer | Unknown | Assumed for V1 |
| S4 | 《因果——记首次禅修的收获》 | Life reflection | Immersive personal scene; question-led sections; story explanation; personal connection; warm closing | Unknown | Assumed for V1 |

## Baseline inferences

| Observable pattern | Candidate rule | Counter-explanation checked | Status |
|---|---|---|---|
| All four begin from personal context or experience | Enter abstract topics through a lived scene | Could be genre convention, but appears across professional and life modes | Established |
| All four explain ideas through concrete stories, products, hobbies, or daily situations | Make the idea visible before generalizing it | Not limited to book reviews | Established |
| All four move from an outside idea to personal agreement, doubt, or application | Keep the user's judgment visible; do not write neutral summaries | Could reflect assignment prompts, but recurs across unrelated topics | Established |
| Spoken phrases, direct questions, and “我/我们/你” recur across modes | Use warm, colloquial Chinese and direct reader connection | Do not encode typos or uncontrolled sentences as colloquiality | Established |
| Headings, stages, lists, or named principles appear in every sample | Give long articles visible conceptual structure | Platform formatting may amplify this, but conceptual chunking is consistent | Established |
| Humor and emoji appear unevenly | Use only as optional accents | Likely topic- and platform-dependent | Provisional |
| Several endings move toward action, conviction, or blessing | Return the idea to life rather than merely summarize | Inspirational endings can easily become generic AI copy | Provisional by ending type; established at the broader principle level |

## Revision evidence

| Date | Task and format | AI version | User revision | Observable change | Candidate rule | Alternative explanation | Status |
|---|---|---|---|---|---|---|---|
| 2026-08-04 | 《六角馆》全案复盘，长篇游戏推理复盘 | `outputs/六角馆全案复盘-V1重写.md` | Awaiting user revision | Pending | Test whether the established voice transfers to a highly technical entertainment explainer; test reducing repeated “谜面—推导—谜底” blocks while preserving reasoning | Differences may come from genre and source incompleteness rather than personal style | Pending |

## Promotion rules

- Mark a rule **provisional** after one clear example.
- Keep it provisional after a second example while checking genre and audience effects.
- Mark it **established** after three independent examples or one explicit user decision.
- Demote or narrow a rule when a counterexample appears.
- Delete rules that merely restate generic good writing advice and do not distinguish the user's choices.

## Forward test

Test one uncertain rule at a time on a new piece.

- Question: Does the candidate rule improve perceived voice fidelity without reducing clarity or changing meaning?
- Success evidence: The user keeps the relevant passage or explicitly endorses the choice.
- Failure evidence: The user repeatedly reverses it, calls it unlike them, or accepts it only in one narrow format.
- Decision: Promote, narrow, revise, or delete the rule.

## Version note

- **V1 — 2026-08-04:** Calibrated from S1–S4. Added two writing modes, evidence-backed voice and structure rules, and explicit guards against copying raw-draft errors or unverified certainty. Awaiting user edits on unseen prompts.
