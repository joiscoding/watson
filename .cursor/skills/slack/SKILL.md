---
name: slack
description: Draft Slack posts in Jo's voice. Use when the user asks for a Slack post, internal announcement, ship note, win share, or customer update for Slack.
model: Opus 4.7 Low Fast
---

# Slack posts

Voice: first person, lowercase, casual, excited. Short punchy paragraphs. Specific names, numbers, and customer references. Generous with `!!` and emojis (`:tada:`, `:ahhhhhhh:`, team custom emojis). Humble and gracious, shouts out teammates by first name. 100 to 200 words.

## Guidance

Do not force a template. Let the post shape follow the news. A common shape is: hook line with emojis, one paragraph on why it matters (deal, customer, signal), one paragraph of background, one paragraph on what shipped and who did what, then a `-----` divider and a short personal reflection. Not every post needs every section.

Lowercase by default, including proper nouns when casual (`netflix`, `austin`). Capitalize acronyms (`IDE`, `CLI`, `PR`). Double `!!` is the default emphasis. Use parenthetical asides for color and numbers. Name teammates by first name.

## Rules

Preserve the user's facts. Do not invent customer names, deal sizes, teammates, PR links, or numbers. Ask if missing.

Follow the repo writing-style rule: never use the dash character `-` inline. Use commas, parentheses, or `•`. The `-----` Slack divider before the personal close is the one exception.

## DO NOT

Do not use corporate or sales language ("excited to announce", "leveraging", "stakeholders"). Do not pad with throat clearing ("just wanted to share", "quick update"). Do not overdo emojis, 2 to 4 across the whole post is plenty.

## Examples

- [examples/dynamic-plugin-loading.md](examples/dynamic-plugin-loading.md), full ship + customer win + personal close, the canonical shape.

Use the closest example for structure and density. Match the user's provided facts first, then borrow phrasing patterns from the examples.
