# english-practice

An [Agent Skill](https://skills.sh) for practicing conversational English with any AI coding agent.

Supports: **Hermes Agent**, **Claude Code**, **Codex**, **Cursor**, and 60+ more via [`npx skills`](https://github.com/vercel-labs/skills).

## What it does

Turns your AI agent into a natural English conversation partner. **Mix Chinese and English freely** — the agent understands everything, gently corrects your English phrasing, and keeps the conversation flowing. No pressure, no "try harder."

## Install

```bash
npx skills add xpinyu/english-practice
```

Or target specific agents:

```bash
npx skills add xpinyu/english-practice -a claude-code -a cursor -a hermes-agent
```

## Usage

Just start chatting. The skill activates when you say things like:

- "Let's practice English"
- "练英语"
- "帮我练英语"

The agent will give corrections in this format:

> **Your version:** "I very like this movie."
> **Better:** "I really like this movie."
> **Note:** "Very like" isn't natural — use "really like" or "like ... a lot."

## Features

- **中英混合** — Chat in Chinese, English, or both in the same sentence
- Gentle corrections (1-2 per message max)
- Progressive difficulty (adapts to your level)
- Natural conversation on any topic
- Works across 67+ AI agents

## License

MIT
