---
name: personal-writing-style
description: Apply and iteratively calibrate the user's evidence-backed Chinese writing style. Use when drafting or rewriting long-form book notes, product and design reflections, personal-growth essays, and experience-led explainers; diagnosing why a draft does not sound like the user; or updating the style after the user edits AI-generated text. Preserve the user's warm, colloquial, example-driven voice without copying errors or inventing personal experience. Do not use to imitate another identifiable author or to invent unsupported preferences.
---

# Personal Writing Style

Build a reproducible voice from evidence. Treat style as a versioned set of choices, not a list of generic “human-sounding” tricks.

## Load the evidence

Read [references/style-profile.md](references/style-profile.md) completely before writing. Read [references/calibration-log.md](references/calibration-log.md) when diagnosing or updating the style.

Classify each rule by evidence:

- **Established**: explicitly chosen by the user or repeated across at least three representative samples.
- **Provisional**: observed in one or two samples; test but do not enforce rigidly.
- **Unknown**: unsupported. Do not fill it with stereotypes or generic anti-AI advice.

Prefer samples written independently by the user. Down-weight copied passages, AI-assisted drafts, one-off formats, and writing the user no longer endorses. Select the professional-reflection or life-reflection mode defined in the profile; do not flatten both into one template.

## Choose the operation

### Draft

1. Preserve the user's intended claim, audience, format, and factual constraints.
2. Apply established rules first and provisional rules only when they fit the task.
3. Use a neutral, clear baseline wherever the profile is unknown.
4. Return the finished text without a style lecture unless the user asks for analysis.

### Rewrite

1. Separate content changes from style changes.
2. Preserve facts, commitments, quoted material, and intended meaning unless the user authorizes changes.
3. Rewrite structure, rhythm, diction, transitions, examples, and emphasis according to the profile.
4. Flag any substantive claim that would need to change for the piece to work; do not hide it as a stylistic edit.

### Diagnose

Compare the draft against the profile and identify the smallest high-impact mismatch. Prioritize recurring differences over cosmetic markers such as punctuation or forced slang. Give concrete before/after examples.

### Calibrate

1. Compare the AI draft with the user's edited version.
2. Record observable changes: deletion, addition, reordering, sentence compression, word replacement, qualification, or tone shift.
3. Infer the simplest rule that explains several changes.
4. Check for an alternative explanation such as factual correction, format constraints, or a one-off preference.
5. Add the evidence to the calibration log.
6. Promote a rule to established only when the user states it explicitly or repeated evidence supports it.

## Guardrails

- Rank priorities as: factual accuracy and intent > clarity > voice fidelity > decorative style.
- Do not manufacture autobiographical details, opinions, emotions, anecdotes, or certainty.
- Do not reproduce typos, grammar slips, inconsistent spacing, image placeholders, or uncontrolled run-on sentences as voice markers.
- Do not confuse “not sounding like AI” with excessive fragments, fake informality, rhetorical questions, em dashes, or banned-word lists.
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
5. What user edit would falsify the strongest style assumption?

When evidence is thin, prefer a clean draft that is easy for the user to correct. Those corrections are the next training signal.
