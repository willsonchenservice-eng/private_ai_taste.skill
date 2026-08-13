# Chinese Language Quality Pass

Use this reference only as a second-layer quality check. First preserve facts, intended meaning, genre, and the user's evidence-backed voice. The goal is readable Chinese, not compliance with a universal “human-sounding” style.

## Decision rule

Change a passage only when all three conditions hold:

1. A specific feature creates a real problem in clarity, rhythm, specificity, or voice fidelity.
2. The rewrite preserves the claim, factual strength, and commitment.
3. The rewrite does not erase an established personal or genre-specific choice.

A trigger word is evidence to inspect, never proof of a problem.

For an explicit request to remove AI-like writing, preserve facts, commitments, and intended emphasis rather than the source's rhetorical shell. If deleting a frame changes no fact, qualification, relation, or necessary emphasis, delete it.

## Checks

### 1. Recover the real action

Inspect empty verbs plus abstract nouns, such as “进行分析”“实现提升”“完成验证”“产生影响”. When the noun hides the action, restore the direct verb.

- “对代码进行验证” → “验证代码”
- “实现了响应速度的提升” → state what became faster and by how much, when known

Keep nominalization when the text genuinely discusses a concept, process, policy, or legal/technical entity rather than an action.

### 2. Test abstract suffixes against meaning

Inspect repeated “化、性、型、度” and vague professional nouns. Replace them only when ordinary wording is more exact.

- “前置化” may become “提前做”
- “颗粒度” may become “拆得多细”

Keep established technical terms when substitution would reduce precision or sound unnatural to the intended readers.

### 3. Shorten delayed meaning

Inspect long “的” phrases, stacked modifiers, and sentences whose main action arrives very late. Move the action forward or split the sentence when readers must hold too much unresolved information.

Do not impose short sentences. Technical and analytical prose may need long sentences; the problem is lost structure, not length itself.

### 4. Inspect translation-like scaffolding

Look closely at repeated frames such as “作为”“基于”“关于”“前者/后者”“是……的”“不是 X，而是 Y”. Ask whether the frame clarifies a real relation or merely carries the sentence.

Keep a contrast only when both sides contain a meaningful distinction. If “不只是/不是” exists only to make the following claim sound larger, state the claim directly.

Back-translation into English is a weak heuristic. Smooth translation does not prove Europeanized Chinese, and difficult translation does not prove good Chinese.

### 5. Replace posture with judgment

Inspect meta-discourse such as “值得深思的是”“我们不禁要问”“综上所述”“这标志着”. Delete it when the following sentence already contains the point. If no concrete judgment remains after deletion, the missing work is reasoning, not wording.

Treat “值得关注” the same way when it merely announces that the next sentence matters. Let the consequence show why it matters.

### 6. Prefer evidence before abstraction when the genre allows

Replace generic claims with a concrete scene, action, consequence, number, or contrast when that evidence actually exists. Never invent specificity to simulate human writing.

Formal summaries, executive briefs, and reference documents may need the conclusion first. Follow the audience's task rather than a universal “scene first” rule.

### 7. Break mechanical rhythm

Inspect repeated three-part lists, identical sentence lengths, symmetrical reversals, and paragraph-ending verdicts. Keep genuine parallel structure; revise only when the pattern makes different ideas sound artificially equal or predictable.

### 8. Trust the reader selectively

Delete repeated summaries, defensive disclaimers, and grand conclusions when the preceding evidence already lands. Keep necessary caveats in legal, medical, technical, safety, or contested factual contexts.

### 9. Read aloud

Read the affected paragraph aloud or simulate its pauses. Revise where the reader loses the subject, action, contrast, or breath. Do not mistake colloquiality for rhythm; a formal sentence can still read naturally.

## Diagnose and rewrite

For each important issue:

1. Quote the smallest relevant span.
2. Name the reading problem rather than the surface marker.
3. Offer the smallest viable rewrite.
4. State any genre or personal-style reason to keep the original.

When the user asks only for a rewrite, apply the checks silently. When the user asks for diagnosis, separate voice mismatches from Chinese-language friction.

After rewriting, scan the output once more. Do not reintroduce an inspected phrase such as “形成闭环” unless the text names what returns to what and that relation is necessary to the claim.

## Calibration boundary

Do not record these checks as personal-style rules by default. Record only the user's observable edits. Promote a related preference when the user explicitly chooses it or repeats it across independent samples. If the user repeatedly restores a construction that this lint questioned, narrow or disable that check for the relevant genre.
