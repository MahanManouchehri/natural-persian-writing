---
name: natural-persian-writing
description: Write, rewrite, review, summarize, document, or otherwise modify meaningful Persian prose in a natural, clear, native-sounding, context-appropriate style. Use for Persian in technical and API documentation, Swagger/OpenAPI descriptions, README files, docstrings and comments, UI copy, validation and error messages, notifications, support messages, admin text, product and business writing, formal documents, and conversational responses. Do not activate merely because code or data contains Persian text that is not being generated or edited.
---

# Natural Persian Writing

Produce Persian that reads as if it was originally written by a competent native Iranian Persian writer. Preserve meaning, technical precision, intent, terminology, and the required level of formality, but do not preserve unnatural English sentence structure.

Formal Persian is not the same as bureaucratic Persian. Simpler Persian is not necessarily more casual Persian.

## Choose the register

Before writing, infer from the task and surrounding project:

- the intended reader and where the text appears;
- the text's purpose and required formality;
- whether it is developer-facing or end-user-facing;
- the technical and domain terms that must remain unchanged;
- whether simplifying it could weaken a technical, security, contractual, or legal guarantee.

Choose the matching register: conversational, customer-friendly, semi-formal, professional, technical, formal, or legal. Do not ask the user when the context already answers these questions. Do not force one tone across all contexts.

## Preserve meaning and project contracts

- Preserve code identifiers, routes, parameter and field names, database columns, enum values, constants, event and job names, permission and role identifiers, error codes, HTTP status codes, and JSON keys exactly.
- Follow established project vocabulary. If the project consistently uses terms such as `Conversation`, `Notification`, `Department`, `Supporter`, `Claim`, or `Release`, keep them consistent and improve the Persian sentence around them.
- Keep standard English technical terms when they are clearer, tied to the codebase, or established in the project. Translate ordinary English adjectives and verbs when Persian is clearer.
- Do not keep ordinary words such as `active`, `private`, `current actor`, or `read` merely because the source mixed them into Persian. Prefer natural equivalents such as «فعال»، «خصوصی»، «کاربر فعلی» and «خوانده‌شده» unless the English word is an exact code value or established domain term.
- Preserve authorization, ownership, state-transition, visibility, and security semantics. Do not invent or strengthen a claim without implementation or source evidence.
- When an important ambiguity affects accuracy, inspect the relevant implementation or source documentation before rewriting.

## Write natural Persian

- Express the meaning with Persian syntax instead of translating the source word by word.
- Prefer direct verbs, active voice, and sentences whose main point is clear on first reading.
- Remove unnecessary repetition, noun chains, passive constructions, filler, and bureaucratic phrases such as «می‌بایست»، «می‌باشد»، «می‌گردد»، «اقدام به» and «در راستای» unless a legal or protocol context truly requires them.
- Keep UI copy short and actionable. Keep support messages respectful and approachable. Keep technical documentation professional, neutral, concise, and easy to scan.
- In legal, contractual, and policy text, accuracy takes priority over simplification. Preserve obligations, prohibitions, exceptions, defined terms, scope, liability, and guarantees.
- Conversational spellings such as «می‌تونی» and «اگه» are appropriate only when the surrounding conversation is genuinely informal.

## Rewriting workflow

1. Identify the subject, action, object, conditions, permissions, result, failure behavior, audience, and fixed terminology.
2. Select the appropriate register.
3. Detect literal translation, English word order, unnecessary English verbs or adjectives, excessive passive voice, and bureaucratic filler.
4. Rewrite with natural Persian syntax while preserving the original contract and terminology.
5. Remove unnecessary complexity and repetition.
6. Recheck technical details, status codes, security boundaries, state transitions, conditions, and exceptions.
7. Read the result as a native speaker would. If it sounds translated, vague, needlessly formal, or mismatched to its context, revise it.

## Format-specific behavior

For any API or Swagger documentation, authorization or security wording, UI copy, validation or error message, support message, formal text, or conversational rewrite, read [references/persian-style-guide.md](references/persian-style-guide.md) before writing. Do not skip this reference when one of these formats is present.

In API prose, describe the observable operation rather than translating its verb literally. For example, a Mark-as-Read operation «Notification موردنظر را برای کاربر فعلی به حالت خوانده‌شده درمی‌آورد». State authorization as an understandable rule, such as «هر کاربر فقط به Notificationهای خودش دسترسی دارد». Describe an IDOR attempt as a request rejected with `403 Forbidden`; never say that IDOR «برابر 403» است.

Do not rename established headings such as `Purpose`, `Authorization`, or `Responses` unless the user requests it or the project convention uses Persian headings.

## Final check

Before finalizing meaningful Persian prose, verify that:

- it sounds written in Persian rather than translated into Persian;
- its formality matches the context;
- its meaning and technical precision remain intact;
- identifiers and established terminology are unchanged and consistent;
- English remains only where useful;
- security behavior and status-code conditions are accurate;
- it is concise enough for where it will appear;
- no new factual claim was introduced.

Explicit user instructions take precedence. Project-specific terminology and legitimate style requirements may select a different register, but unrelated project instructions do not disable basic Persian readability.
