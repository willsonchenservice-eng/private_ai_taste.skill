---
name: personal-writing-style
description: Apply and iteratively calibrate the user's evidence-backed Chinese writing style. Use when drafting or rewriting long-form book notes, product and design reflections, personal-growth essays, experience-led explainers, or other Chinese prose; diagnosing why a draft does not sound like the user; updating the style after the user edits AI-generated text; or responding to requests such as “去 AI 味”, “降低 AI 味”, “写得像我”, or “别像通用 AI 文案”. Preserve the user's warm, colloquial, example-driven voice without copying errors, inventing personal experience, or replacing personal voice with generic anti-AI tricks.
---

# Personal Writing Style

Build a reproducible voice from evidence. Treat style as a versioned set of choices, not a list of generic “human-sounding” tricks.

## Load the evidence

Read [references/style-profile.md](references/style-profile.md) completely before writing. Read [references/calibration-log.md](references/calibration-log.md) when diagnosing or updating the style.

For requests to remove AI-like writing, improve Chinese naturalness, diagnose translation-like prose, or perform a final language pass, also read [references/chinese-language-lint.md](references/chinese-language-lint.md) completely. Treat that reference as a clarity check, not as evidence of the user's personal style.

Classify each personal-style rule by evidence:

- **Established**: explicitly chosen by the user or repeated across at least three representative samples.
- **Provisional**: observed in one or two samples; test but do not enforce rigidly.
- **Unknown**: unsupported. Do not fill it with stereotypes or generic anti-AI advice.

Prefer samples written independently by the user. Down-weight copied passages, AI-assisted drafts, one-off formats, and writing the user no longer endorses. Select the professional-reflection or life-reflection mode defined in the profile; do not flatten both into one template.

## Choose the operation

### Draft

1. Preserve the user's intended claim, audience, format, and factual constraints.
2. Apply established rules first and provisional rules only when they fit the task.
3. Use a neutral, clear baseline wherever the profile is unknown.
4. When the request includes naturalness or AI-taste concerns, run the Chinese quality pass after the personal-style draft.
5. Return the finished text without a style lecture unless the user asks for analysis.

### Rewrite

1. Separate content changes from style changes.
2. Preserve facts, commitments, quoted material, and intended meaning unless the user authorizes changes.
3. Rewrite structure, rhythm, diction, transitions, examples, and emphasis according to the profile.
4. Use the Chinese quality pass to remove language friction only when it improves clarity, rhythm, or voice fidelity. Do not enforce generic markers against evidence-backed preferences.
5. For an explicit “去 AI 味” request, preserve the source's facts and intended emphasis, not its rhetorical scaffolding. Re-scan the rewritten output once so the rewrite does not reintroduce empty frames from the source.
6. Flag any substantive claim that would need to change for the piece to work; do not hide it as a stylistic edit.

### Diagnose

Diagnose on two separate axes:

1. **Voice fidelity**: compare the draft against the profile and identify the smallest high-impact mismatch.
2. **Chinese quality**: when relevant, identify sentence-level friction described in the Chinese-language lint.

Prioritize recurring differences and meaning loss over cosmetic markers such as punctuation, forced slang, or isolated trigger words. Give concrete before/after examples. Do not label a sentence “AI-like” without explaining what comprehension, rhythm, specificity, or voice problem it creates.

### Calibrate

1. Compare the AI draft with the user's edited version.
2. Record observable changes: deletion, addition, reordering, sentence compression, word replacement, qualification, or tone shift.
3. Infer the simplest personal-style rule that explains several changes.
4. Check for an alternative explanation such as factual correction, format constraints, a Chinese-language repair, or a one-off preference.
5. Add the evidence to the calibration log.
6. Promote a rule to established only when the user states it explicitly or repeated evidence supports it.
7. Do not promote a generic lint rule into the personal profile unless the user's own edits repeatedly support it.

## Chinese quality pass

Run this pass after preserving facts, intent, and personal voice. Use the detailed checks and boundaries in [references/chinese-language-lint.md](references/chinese-language-lint.md).

1. Find the smallest phrase that creates friction.
2. Explain the actual problem: obscured action, unnecessary abstraction, delayed meaning, repetitive scaffolding, uniform rhythm, or over-explanation.
3. Make the smallest rewrite that fixes that problem.
4. Check the rewrite against the style profile and restore any evidence-backed personal choice that the cleanup erased.
5. Read the affected passage aloud when rhythm matters.
6. Re-scan the finished passage. If a questioned frame adds no fact, qualification, relation, or useful emphasis, remove it rather than carrying it into the final answer.

Treat back-translation as a weak clue only. Never use smooth translation into English as proof that Chinese is unnatural. Do not use banned-word lists, punctuation quotas, or forced colloquiality as substitutes for judgment.

## Guardrails

- Rank priorities as: factual accuracy and intent > clarity > voice fidelity > decorative style.
- Do not manufacture autobiographical details, opinions, emotions, anecdotes, or certainty.
- Do not reproduce typos, grammar slips, inconsistent spacing, image placeholders, or uncontrolled run-on sentences as voice markers.
- Do not confuse “not sounding like AI” with excessive fragments, fake informality, rhetorical questions, em dashes, banned-word lists, or mandatory short sentences.
- Do not overfit one article. Style changes by audience, genre, and purpose; record those boundaries.
- Do not silently turn preferences into universal rules. Preserve evidence and confidence.
- Do not claim the output “sounds like the user” while the profile is uncalibrated. Say that it is a neutral V0 and name the missing evidence in one sentence.
- Ask at most one high-value question when a missing audience, purpose, or format would materially change the result. Otherwise make the smallest reversible assumption and state it.

## Self-check

Before returning text, verify:

1. Did any factual claim or commitment change during a style rewrite?
2. Can each distinctive choice be traced to an established or provisional rule?
3. Did surface mannerisms replace actual reasoning or specificity?
4. Does the structure suit this audience and format rather than merely resemble the samples?
5. Did the Chinese quality pass fix a real reading problem, or merely enforce a generic preference?
6. What user edit would falsify the strongest style assumption?

When evidence is thin, prefer a clean draft that is easy for the user to correct. Those corrections are the next training signal.
