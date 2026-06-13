# Contributing to AI Game Prompts

Thank you for your interest in contributing! This document provides guidelines and information for contributors.

## 🎯 What We're Looking For

### New Games
- Original text-based interactive games
- Follow the structure in `games/01-dawn-continent.md`
- Include both English and Chinese versions (or at least one)
- Token cost should be under 20K for mobile compatibility

### Improvements
- Bug fixes in existing game files
- Clarifications to rules or protocols
- Additional examples for AI guidance
- Translation improvements

### Documentation
- Tutorials for creating new games
- Model compatibility testing results
- User guides for players

## 📝 How to Contribute

### 1. Fork the Repository
Click the "Fork" button at the top right of the repository page.

### 2. Create a Branch
```bash
git checkout -b feature/your-feature-name
```

### 3. Make Your Changes
Follow the existing structure and style.

### 4. Test Your Changes
- If adding a game, test it with at least one AI model
- Ensure all links work
- Check token count (should be reasonable for target models)

### 5. Commit Your Changes
```bash
git add .
git commit -m "Add: [brief description of your change]"
```

### 6. Push to Your Fork
```bash
git push origin feature/your-feature-name
```

### 7. Submit a Pull Request
Go to the original repository and click "New Pull Request".

## 🎮 Adding a New Game

### File Naming
- Use format: `XX-game-name.md` where XX is a two-digit number
- Example: `02-mystery-mansion.md`

### Required Sections
1. **Metadata** (type, token cost, recommended models)
2. **Player Profile Collection** (opening questions)
3. **World Setting** (core rules and physics)
4. **Core Mechanics** (resources, abilities, etc.)
5. **Opening Script** (exact text for AI to use)
6. **State Review Protocol** (checkpoint format)
7. **Save/Load Protocol** (if applicable)
8. **AI Red Lines** (anti-AI-writing rules)
9. **Self-Check List** (for AI to verify before each turn)

### Style Guidelines
- Use colloquial, short sentences
- Avoid AI-speak and translationese
- Provide concrete examples (not abstract rules)
- Focus on "show, don't tell"
- Include at least 3-4 example outputs for AI to learn from

### Token Budget
- Target: 15K tokens per game file
- Maximum: 20K tokens (for complex games)
- Leave room for conversation history

## 🌐 Translation Guidelines

### English ↔ Chinese
- Maintain parallel structure
- Adapt cultural references appropriately
- Keep technical terms consistent
- Test both versions with AI models

## 🐛 Reporting Bugs

Use GitHub Issues with the following template:

```markdown
**Describe the bug**
A clear description of what the bug is.

**To Reproduce**
Steps to reproduce the behavior:
1. Load game X
2. Do Y
3. See error

**Expected behavior**
What you expected to happen.

**Screenshots**
If applicable, add screenshots.

**Environment:**
- AI Model: [e.g., Qwen3 Max, Claude 4.6]
- Context Window: [e.g., 256K tokens]
- Game: [e.g., 01-dawn-continent]

**Additional context**
Add any other context about the problem here.
```

## 💡 Suggesting Features

Use GitHub Issues with the label "enhancement".

## 📋 Code of Conduct

- Be respectful and inclusive
- Focus on constructive feedback
- Assume good intentions
- Help newcomers learn the ropes

## ❓ Questions?

Open a GitHub Discussion or contact the maintainers.

---

Thank you for helping make text-based gaming accessible to everyone! 🎮
