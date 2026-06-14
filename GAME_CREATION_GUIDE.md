# AI Game Prompts — Game Creation Guide

This guide walks you through creating a new text-based interactive game for the AI Game Prompts repository.

## 📋 Before You Start

### Understand the Philosophy
- **Emergent narrative**: No preset plots, truths, or endings
- **Anti-AI-writing**: Avoid common AI writing pitfalls
- **Mobile-first**: Keep token cost reasonable (15-20K max)
- **Universal compatibility**: Work with any AI model

### Study the Template
Read `games/01-dawn-continent.md` thoroughly. It's your reference for:
- Structure and organization
- Level of detail required
- Example outputs for AI to learn from
- Anti-AI-writing rules implementation

## 🏗️ Game Structure

### Required Sections

#### 1. Metadata Header
```markdown
# Game XX · Game Name

> **Type**: [genre] / [subgenre]
> **Pacing**: [turn structure]
> **Token cost**: ~XXK (recommended XXK+ models)
> **Style anchors**: [3-5 keywords]
```

#### 2. Player Profile Collection (Point 1)
- Ask 5 questions (name, age, gender, background, occupation)
- Make it clear these are for immersion only, not game mechanics
- Provide default values if player doesn't answer

#### 3. World Setting (Point 2)
- Core physics and rules
- Time system
- Resource locations
- Communication systems
- Unbreakable rules (no cheats, no resurrection, etc.)

#### 4. Fixed Events Timeline (Point 3)
- List 5-7 "iron-clad" events that must happen
- Specify what players can influence vs. what's fixed
- Include foreshadowing methods

#### 5. Emergent Narrative Rules (Point 4)
- Core principles (AI is engine, not author)
- How AI generates events (5 factors to consider)
- **3-4 concrete example outputs** (critical!)
- Anomaly generation rules
- Ending generation rules

#### 6. Causal Chain System (Point 5)
- Event marker format
- Reference rules (how often to cite past choices)
- Butterfly effect implementation

#### 7. Resource System (Point 6)
- Base resources (5-6 types)
- Currency system (2-3 tiers)
- Upgrade paths
- Resource-ecology-disaster linkages

#### 8. Judgment System (Point 7)
- Hidden difficulty scoring (1-10)
- Success scoring (1-10)
- Output rules (no probability透露)

#### 9. Ability System (Point 8)
- Base attributes (6 types, hidden from player)
- Learnable skills (20-30 skills)
- Experience mechanics

#### 10. System Functions (Point 9)
- Panel contents (what's shown)
- Panel restrictions (what's hidden)

#### 11. Financial/Trading System (Point 10)
- Trading channels (3-5 types)
- Banking (if applicable)
- Loans and interest

#### 12. Tool/Tech Tree (Point 11)
- Tech levels (5 tiers)
- Crafting rules
- Unlock conditions

#### 13. Food Chain/Ecology (Point 12)
- Ecological tiers (5 levels)
- Hunting difficulty
- Food states
- Ecological linkages

#### 14. History/World Lore (Point 13)
- Historical eras (2-3)
- Mysterious phenomena (no explanations)

#### 15. Disaster System (Point 14)
- Scheduled disasters (every 10 days)
- Disaster announcement wording
- Disaster stacking rules

#### 16. Faction System (Point 15)
- Faction types (6-8 types)
- Internal sub-factions
- Hidden agendas
- Faction trials
- Faction dissolution rules

#### 17. Anomaly System (Point 16)
- Random generation rules
- No fixed list
- No explanations
- No forced connections

#### 18. World Dynamics (Point 17)
- Seasonal cycles
- Ecological migration
- Economic fluctuations
- Political changes
- Resource depletion

#### 19. Hidden Mechanisms (Point 18)
- List 7-10 hidden mechanics
- When players discover them
- Discovery methods

#### 20. NPC Personalities (Point 19)
- 7 personality archetypes
- Behavior patterns
- Relationship rules

#### 21. Pacing/Plot Structure (Point 20)
- 5-act structure
- Pacing red lines (no early spoilers)

#### 22. AI Red Lines (Point 21)
- 5 core rules with examples
- This is the most important section

#### 23. Opening Script (Point 22)
- Exact text for AI to output
- Include sensory details
- End with 2-4 options + free input

#### 24. State Review Protocol (Point 23)
- Checkpoint format (every 5 turns)
- What to include

#### 25. Save/Load Protocol (Point 24)
- Save code format
- Load instructions

#### 26. Self-Check List (Point 25)
- 8 questions AI asks itself before each turn

### Optional Sections
- Mini-games
- Special mechanics unique to your game
- Extended lore

## ✍️ Writing Style

### Do
- Use short, colloquial sentences
- Show, don't tell
- Provide concrete sensory details
- Give players meaningful choices
- Include 3-4 example outputs for AI to learn from

### Don't
- Use AI-speak ("命运的齿轮", "抉择的十字路口")
- Use translationese ("在当今快节奏的数字时代")
- Use grand narratives ("宇宙在呼吸", "负熵梯度")
- Explain, summarize, or preach
- Reveal probabilities or future events
- Preset conspiracies or truths

## 🧪 Testing Your Game

### Before Submitting
1. **Token count**: Ensure it's under 20K
2. **AI compatibility**: Test with at least 2 different AI models
3. **Example outputs**: Verify AI can learn from your examples
4. **Red lines**: Ensure AI follows all 5 core rules
5. **Emergent narrative**: Verify no preset plots or truths

### Test Checklist
- [ ] AI asks player profile questions first
- [ ] AI uses exact opening script
- [ ] AI provides 2-4 options + free input each turn
- [ ] AI doesn't explain or summarize
- [ ] AI doesn't reveal probabilities
- [ ] AI doesn't use AI-speak
- [ ] AI references event markers naturally
- [ ] AI maintains pacing (no early spoilers)
- [ ] AI follows state review protocol
- [ ] AI handles save/load correctly

## 🌐 Translation

### If Creating Bilingual Version
1. Create `XX-game-name.md` (English)
2. Create `XX-game-name_zh.md` (Chinese)
3. Maintain parallel structure
4. Adapt cultural references appropriately
5. Test both versions

## 📤 Submission

1. Follow the contribution guidelines in `CONTRIBUTING.md`
2. Include a brief description of your game
3. Mention which AI models you tested with
4. Note any known limitations

## 🎯 Success Criteria

Your game will be accepted if:
- ✅ Follows the required structure
- ✅ Token cost is reasonable (under 20K)
- ✅ Includes 3-4 example outputs
- ✅ Passes the test checklist
- ✅ Avoids all AI writing pitfalls
- ✅ Provides an engaging player experience

---

**Ready to create?** Start with a simple concept and build up. Good luck! 🎮
