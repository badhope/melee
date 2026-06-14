# AI Game Prompts Repository

> **Turn any AI into a text-based game engine** — pure Markdown, no code, playable on mobile.

[中文文档 / Chinese](./README_zh.md)

## What is this?

This is a **prompt-only repository** containing structured Markdown files that turn any general-purpose AI (mobile or web) into an interactive text game engine. No apps to install, no code to run — just prompts that the AI reads and executes.

**Repository language policy:**
- **AI-loaded files** (`meta/*.md`, `games/*.md`) are written in **English** — English is the most accurate language for AI to follow complex prompt rules.
- **Human-facing docs** (README, CONTRIBUTING, GAME_CREATION_GUIDE) are **bilingual** (English + Chinese), so humans of either language can read them.
- **The AI responds to the player in the player's own language.** Internal reasoning stays in English; the narrative, options, and status blocks mirror whatever language the user types in. This rule is defined in `meta/00-how-to-use.md` (Section 4 · Language Rule).

## Features

- **Universal compatibility**: works with any AI model (Qwen, Claude, GPT, Kimi, Doubao, …)
- **Mobile-first**: designed for mobile AI apps — players just share the repo link
- **Pure Markdown**: no code, no dependencies, just structured prompts
- **Modular design**: add a new game by dropping one `.md` file into `games/`
- **Anti-AI-writing rules**: built-in safeguards against common AI writing pitfalls
- **Language mirror**: the AI responds in the user's language automatically

## Repository Structure

```
/
├── README.md                       ← You are here (English entry)
├── README_zh.md                    ← 中文入口 (Chinese entry)
├── LICENSE                         ← MIT License
├── CONTRIBUTING.md                 ← Contribution guidelines (English)
├── CONTRIBUTING_zh.md              ← 贡献指南 (Chinese)
├── GAME_CREATION_GUIDE.md          ← Guide for creating new games (English)
├── GAME_CREATION_GUIDE_zh.md       ← 游戏创建指南 (Chinese)
├── meta/
│   ├── 00-how-to-use.md            ← Loading protocol (AI must read) · English
│   └── 01-engine-core.md           ← Core engine rules (all games) · English
└── games/
    └── 01-dawn-continent.md        ← Game 01: Dawn Continent (Survival RPG) · English
```

## Quick Start

### For Players

1. Copy this URL: `https://github.com/badhope/ai-game-prompts`
2. Open your favorite AI app (Qwen, Claude, ChatGPT, Kimi, Doubao, …)
3. Tell the AI: "Read this repository and start the game." (Or, in your own language.)
4. The AI will guide you through the rest — in **your** language.

### For AI Models

When you see this message, follow the loading sequence:

1. **Read this README** to understand the repository structure.
2. **Read `meta/00-how-to-use.md`** — the loading protocol (including the language-mirror rule in Section 4).
3. **Detect the user's language** from their first message. That language is the response language for the entire session.
4. **Ask the user** which game they want to play.
5. **Read the game file** (e.g. `games/01-dawn-continent.md`).
6. **Start the game** following the game's opening protocol.

> **Critical**: do NOT start any game before reading `meta/00-how-to-use.md`.

## Available Games

| # | Game Name | Type | Token Cost | Recommended Model |
|---|---|---|---|---|
| 01 | Dawn Continent | Open-world survival / multiplayer competition / emergent narrative | ~15K | 32K+ context |

*More games coming soon!*

## Model Compatibility

| Model | Context Window | Status |
|---|---|---|
| Qwen Qwen3 Max | 256K tokens | Fully compatible |
| Claude 4.6 Sonnet/Opus | 200K tokens | Fully compatible |
| GPT-5.5 | 128K tokens | Compatible |
| Kimi | 1.33M tokens | Fully compatible |
| Doubao | 256K chars | Enable "continuous chat" mode |

## Adding a New Game

1. Create a new file in `games/` named `0X-game-name.md` (English).
2. Follow the structure of `01-dawn-continent.md` as a template.
3. Add the game to the "Available Games" table in this README.
4. Submit a pull request.

See [GAME_CREATION_GUIDE.md](./GAME_CREATION_GUIDE.md) for detailed instructions.

## Core Design Principles

### Fixed (never change)
- Resource system (wood / stone / iron / food / water)
- Currency system (credit points + source stones)
- Ability system (6 attributes + 24 skills)
- Tech tree (5 levels)
- Food chain (5 tiers)
- Financial / trading system
- Judgment system
- Faction system (8 types + internal sub-factions)

### Dynamic (changes every game)
- Factions (randomly generated each game)
- Anomalies (fully random, no fixed list)
- Plot / events (emergent, not scripted)
- Endings (player-driven, not preset)
- NPC personalities (7 archetypes)
- World dynamics (seasons / economy / politics / ecology)

## Anti-AI-Writing Rules

All games enforce these 5 core red lines:

1. **No explaining / summarizing / preaching** — only describe what happens
2. **No deciding for players / revealing probabilities** — only describe current state
3. **No AI-speak / translationese / grand narrative** — use colloquial, short sentences
4. **No preset conspiracies / truths / endings** — emergent narrative only
5. **No linear storytelling / templates** — dead ends, useless choices, ordinary NPCs

## License

MIT License — see [LICENSE](./LICENSE) for details.

## Contributing

We welcome contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## Support

- **Issues**: use GitHub Issues for bug reports and feature requests
- **Discussions**: use GitHub Discussions for questions and ideas
- **Discord**: [Coming Soon]

## Acknowledgments

- Inspired by text-based RPGs and interactive fiction
- Anti-AI-writing rules based on University of Maryland + DeepMind research (61,608 AI stories)
- Designed for mobile-first AI app users

---

**Ready to play?** Share this repo with your AI and say: "Read this and start the game."
