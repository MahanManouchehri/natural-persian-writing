---
name: natural-persian-writing
description: Produce, rewrite, translate, review, or summarize meaningful Persian prose that sounds natural, preserves meaning, and matches its audience and purpose. Use for any Persian content: personal and formal letters, email, business, marketing, academic, legal and policy text, creative writing, translation, support, UI, technical documentation, and conversation. Do not activate merely because Persian appears in source code, data, an identifier, or text that is not being changed.
---

# Natural Persian Writing

Write Persian as a skilled native Iranian Persian writer would write it: clear, natural, precise, and appropriate to the situation. Preserve the user's intent, facts, named entities, required terminology, tone, and boundaries. Do not reproduce unnatural word order from another language.

This is a general writing skill, not a programming-only skill. It applies wherever meaningful Persian prose is created or changed.

## Choose the right register

Before writing, infer the audience, purpose, medium, relationship between writer and reader, and consequences of imprecision. Then choose a fitting register: conversational, warm and respectful, professional, formal, technical, academic, legal, persuasive, or literary.

- Use informal forms such as «می‌تونی» and «اگه» only in genuinely informal contexts.
- Keep formal writing direct and human. Formal Persian is not bureaucratic Persian.
- Keep UI, alerts, and short messages brief and actionable.
- Keep legal, policy, medical, financial, contractual, and security-sensitive content exact. Do not simplify away an obligation, exception, limitation, condition, scope, or warning.
- When the requested tone is unclear and it materially changes the result, ask one concise question; otherwise make the best contextual choice.

## Preserve meaning and fixed content

- Preserve names, dates, amounts, quotations, URLs, citations, product names, code identifiers, routes, JSON keys, and other fixed values exactly unless the user asks to change them.
- Preserve the source's degree of certainty, politeness, urgency, and commitment. Do not invent facts, promises, legal effects, or emotional intent.
- Keep established foreign words when they are names, direct quotations, technical terms, or clearer than an artificial translation. Translate ordinary borrowed words when natural Persian is clearer.
- Do not introduce cultural assumptions or locally specific claims that are absent from the source.

## Write natural Persian

- Use Persian sentence structure, natural verb placement, and active verbs where appropriate.
- Prefer clear, concrete words and the shortest form that retains the intended meaning.
- Avoid literal translation, unnecessary repetition, noun-heavy phrasing, and bureaucratic filler such as «می‌باشد»، «می‌گردد»، «اقدام به» and «در راستای» unless the context genuinely requires it.
- Use correct نیم‌فاصله and punctuation when practical, but do not alter quoted, branded, or format-sensitive text without need.
- Break dense content into short paragraphs, headings, or lists when that makes it easier to read.

## Translation workflow

When translating into Persian:

1. Identify the source's purpose, audience, register, facts, constraints, and implied tone.
2. Translate the meaning, not the source language's word order.
3. Preserve proper nouns, legal terms, quotations, figures, units, and links accurately.
4. Adapt politeness and formality naturally for Persian without adding content.
5. Re-read the result as original Persian prose; revise anything that sounds translated, vague, or culturally mismatched.

When translating from Persian, first clarify the target language and register if they are not obvious. Preserve the Persian source's meaning and level of formality; do not silently “improve” its claims.

## Writing and rewriting workflow

1. Identify the subject, intended reader, action or message, context, tone, and any fixed wording.
2. Choose the register and structure that fit the medium.
3. Write or revise in natural Persian while preserving meaning.
4. For sensitive content, recheck obligations, permissions, dates, amounts, exceptions, and factual claims.
5. Make the final result easy to read at the required length.

## Context-specific guidance

- **Letters and email:** Make the purpose and requested next step clear. Match the relationship and level of formality; avoid both cold bureaucracy and unwarranted familiarity.
- **Business and marketing:** Be credible and specific. Do not make unsupported performance, price, availability, or legal claims.
- **Academic writing:** Preserve evidence, citations, uncertainty, and disciplinary terminology. Do not overstate a conclusion.
- **Legal and policy text:** Preserve every condition, exception, defined term, obligation, prohibition, scope, liability, and guarantee. Accuracy comes before simplification.
- **Creative writing:** Respect the requested voice, rhythm, imagery, point of view, and emotional subtext. Do not flatten deliberate style into generic prose.
- **Support and UI:** Be concise, respectful, and useful. State the next action where helpful; omit internal implementation detail unless it helps the reader.
- **Technical content:** Preserve code and product contracts exactly while making the surrounding Persian clear. Read [references/persian-style-guide.md](references/persian-style-guide.md) for API, security, UI, and support wording.

## Final check

Before responding, verify that the Persian:

- reads as original Persian rather than a literal translation;
- fits the requested audience, medium, and formality;
- preserves facts, intent, terminology, and all important qualifications;
- has no unwanted bureaucratic or colloquial tone;
- is concise enough for its purpose; and
- introduces no new factual, legal, security, or emotional claim.

User instructions always take precedence. Preserve a deliberate writing style when the user asks for it, even when it differs from the default preference for simplicity.
