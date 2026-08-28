# Support loop memory schema

This file defines **how** Chara may remember support-loop feedback. It does not contain Yuriy's actual personal history.

## Public repository rule

This repository is public. Therefore this file is a schema only.

Do not store actual support-loop entries here while the repository is public.

Actual feedback should remain in the conversation or in a private state store explicitly approved by Yuriy.

## Minimal private record

If a private state store becomes available, one interaction may be represented with only these fields:

```text
date: YYYY-MM-DD
topic: short category
intervention: short action signature
reaction: useful | exactly_right | neutral | annoying | too_medical | too_generic | too_much
next_rule: repeat_if_relevant | avoid_for_now | simplify | change_topic | continue_observation
```

Example:

```text
date: 2026-08-29
topic: work_shutdown
intervention: evening_task_dump
reaction: useful
next_rule: repeat_if_relevant
```

## Do not store

Do not use the loop memory as a health diary or anxiety log.

Do not store:

- raw medical information;
- diagnoses or inferred diagnoses;
- lab values;
- body measurements;
- medication details;
- detailed sleep logs;
- detailed food logs;
- family or relationship details;
- financial information;
- work secrets or unfinished task text;
- verbatim emotional disclosures unless Yuriy explicitly asks to preserve them.

Prefer a compact action signature over the content behind it.

## Interpretation rules

1. No response is not a negative reaction.
2. One reaction is a weak signal, not a permanent preference.
3. Repeated similar reactions can become a working preference.
4. A later explicit statement from Yuriy overrides older inferred patterns.
5. Preferences should be treated as revisable when context changes.
6. Never infer a medical or psychological condition from the feedback log.

## Duplicate guard

Before generating a support message, compare the proposed intervention with recent interventions.

Do not send the same action again merely with different prose.

Repeat only when at least one of these is true:

- Yuriy explicitly asks for it;
- a new observation makes the action relevant again;
- the previous intervention was positively received and enough context has changed;
- the message is a deliberate continuation of an experiment already in progress.

Otherwise prefer a different lever, simple continuation, or silence.

## Purpose

Memory exists to reduce noise, avoid repetition, and learn what kind of support is useful.

It is not a scoring system for Yuriy and should never become one.
