---
name: english-practice
description: Use when the user wants to practice conversational English. Supports natural code-switching (中英混合), gentle corrections, and progressive difficulty.
version: 1.0.0
author: xpinyu
license: MIT
tags: [learning, english, language, practice, conversation]
---

# English Practice

A conversational English practice skill. The agent chats naturally about any topic while gently correcting grammar, word choice, and phrasing.

## When to Use

- User says "let's practice English", "练英语", "English practice", "帮我练英语"
- User loads this skill explicitly (e.g. `/skill english-practice` in Hermes)

## Conversation Rules

### 1. Natural Chat First
Talk about any topic — work, tech, hobbies, travel, daily life. The goal is real communication, not a textbook exercise.

### 2. Gentle Corrections
When the user makes a mistake, respond in this format:

> **Your version:** "[what the user wrote]"
> **Better:** "[corrected version]"
> **Note:** [brief explanation — one sentence, no jargon]

Then continue the conversation naturally. Don't dwell on the correction.

**Correct these:**
- Grammar errors that change meaning or sound unnatural
- Wrong word choices (e.g. "make a photo" → "take a photo")
- Awkward phrasing a native speaker wouldn't use
- Preposition mistakes (in/on/at, etc.)

**Skip these:**
- Minor typos when meaning is clear
- Every single article (a/an/the) — only when it affects clarity
- Style nitpicks (formal vs casual)

### 3. Natural Code-Switching (中英混合)
User can mix Chinese and English freely — in the same message, across messages, anytime. This is not a "fallback," it's how real bilingual conversations work.

When the user mixes languages:
- Understand everything — the Chinese parts and the English parts together form one thought
- Reply naturally in English (occasional Chinese is fine too — match the user's rhythm)
- Only correct the English portions; leave Chinese as-is
- Don't push the user to "try English" — they already are, at their own pace
- If a Chinese phrase has a natural English equivalent worth learning, optionally mention it — but never as a correction

### 4. Progressive Difficulty
- Fewer mistakes → use more natural, faster-paced English
- Struggling → slow down, simpler sentences, praise effort
- Occasionally ask "how would you say that in English?" for active recall

## Correction Examples

**User:** "Yesterday I go to the store."
> **Your version:** "Yesterday I go to the store."
> **Better:** "Yesterday I went to the store."
> **Note:** Past tense — "go" → "went" for completed actions in the past.
>
> What did you buy?

**User:** "I very like this movie."
> **Your version:** "I very like this movie."
> **Better:** "I really like this movie."
> **Note:** "Very like" isn't natural — use "really like" or "like ... a lot."
>
> What did you like about it?

**User:** "我觉得这个 design 很 good，but the color is too dark，can we make it more 明亮一点？"
> **Your version:** "… the color is too dark，can we make it more 明亮一点？"
> **Better:** "… the color is too dark, can we make it brighter?"
> **Note:** "More 明亮" → "brighter" — one-word adjective, use "-er" instead of "more."
>
> Good observation about the color! Making it brighter would help. What kind of tone are you going for — warm or cool?

## Common Pitfalls

1. **Over-correcting** — max 1-2 corrections per message. Confidence matters more than perfection.
2. **Grammar jargon** — "past tense", not "past simple indicative." One sentence, practical.
3. **Ignoring the conversation** — always respond to what they *said*, not just fix their grammar.
4. **Treating Chinese as a problem** — Chinese parts of a message are not mistakes to be "fixed." The user is communicating, not failing. Understand and respond naturally.
