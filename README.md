# AI Game Prompts Repository

> **Transform any AI into a text-based game engine** — pure Markdown, no code, playable on mobile.

[中文文档](./README_zh.md)

## What is this?

This is a **prompt-only repository** containing structured Markdown files that turn any general-purpose AI (mobile or web) into an interactive text game engine. No apps to install, no code to run — just prompts that AI can read and execute.

## Features

- **Universal Compatibility**: Works with any AI model (Qwen, Claude, GPT, Kimi, Doubao, etc.)
- **Mobile-First**: Designed for mobile AI apps — users just share the repo link
- **Pure Markdown**: No code, no dependencies, just structured prompts
- **Modular Design**: Add new games by dropping one `.md` file into `games/`
- **Anti-AI-Writing Rules**: Built-in safeguards against common AI writing pitfalls

## Repository Structure

```
/
├── README.md                       ← You are here (English entry)
├── README_zh.md                    ← 中文入口
├── LICENSE                         ← MIT License
├── CONTRIBUTING.md                 ← Contribution guidelines
├── GAME_CREATION_GUIDE.md          ← Guide for creating new games
├── meta/
│   ├── 00-how-to-use.md            ← Loading protocol (AI must read)
│   └── 01-engine-core.md           ← Core engine rules (all games)
└── games/
    └── 01-dawn-continent.md        ← Game 01: Dawn Continent (Survival RPG)
```

## Quick Start

### For Players

1. Copy this URL: `https://github.com/badhope/ai-game-prompts`
2. Open your favorite AI app (Qwen, Claude, ChatGPT, Kimi, etc.)
3. Tell the AI: "Read this repository and start the game"
4. The AI will guide you through the rest

### For AI Models

When you see this message, follow the loading sequence:

1. **Read this README** to understand the repository structure
2. **Read `meta/00-how-to-use.md`** — the loading protocol
3. **Ask the user** which game they want to play
4. **Read the game file** (e.g., `games/01-dawn-continent.md`)
5. **Start the game** according to the game's opening protocol

> **Critical**: Do NOT start any game before reading `meta/00-how-to-use.md`.

## Available Games

| # | Game Name | Type | Token Cost | Recommended Model |
|---|---|---|---|---|
| 01 | Dawn Continent | Open-world survival / Multiplayer competition / Emergent narrative | ~15K | 32K+ context |

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

1. Create a new file in `games/` named `0X-game-name.md`
2. Follow the structure in `01-dawn-continent.md` as a template
3. Add the game to the "Available Games" table in this README
4. Submit a pull request

See [GAME_CREATION_GUIDE.md](./GAME_CREATION_GUIDE.md) for detailed instructions.

## Core Design Principles

### Fixed (Never Change)
- Resource system (wood/stone/iron/food/water)
- Currency system (credit points + source stones)
- Ability system (6 attributes + 24 skills)
- Tech tree (5 levels)
- Food chain (5 tiers)
- Financial/trading system
- Judgment system
- Faction system (8 types + internal factions)

### Dynamic (Changes Every Game)
- Factions (randomly generated each game)
- Anomalies (completely random, no fixed list)
- Plot/events (emergent, not scripted)
- Endings (player-driven, not preset)
- NPC personalities (7 archetypes)
- World dynamics (seasons/economy/politics/ecology)

## Anti-AI-Writing Rules

All games enforce these 5 core red lines:

1. **No explaining/summarizing/preaching** — Only describe what happens
2. **No deciding for players/revealing probabilities** — Only describe current state
3. **No AI-speak/translationese/grand narratives** — Use colloquial, short sentences
4. **No preset conspiracies/truths/endings** — Emergent narrative only
5. **No linear storytelling/templates** — Dead ends, useless choices, ordinary NPCs

## License

MIT License — see [LICENSE](./LICENSE) for details.

## Contributing

We welcome contributions! See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## Support

- **Issues**: Use GitHub Issues for bug reports and feature requests
- **Discussions**: Use GitHub Discussions for questions and ideas

## Acknowledgments

- Inspired by text-based RPGs and interactive fiction
- Anti-AI-writing rules based on University of Maryland + DeepMind research (61,608 AI stories)
- Designed for mobile-first AI app users

---

**Ready to play?** Share this repo with your AI and say: "Read this and start the game."
