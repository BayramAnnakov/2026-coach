# 2026-coach

Executive coaching skill that helps you plan your 2026 using research-backed process goals.

## Why Process Goals?

According to [Williamson et al. (2022)](https://doi.org/10.1080/1750984X.2022.2116723) meta-analysis of 27 studies:

| Goal Type | Effect Size | What It Means |
|-----------|-------------|---------------|
| **Process goals** | d=1.36 | Focus on daily behaviors you control 100% |
| Performance goals | d=0.44 | Short-term milestones |
| Outcome goals | d=0.09 | Long-term results |

**Process goals are 15x more effective than outcome goals.**

Why they work:
- **Total control** - You can always send 20 messages
- **Builds self-efficacy** - Small wins compound
- **Reduces anxiety** - Focus on input, not output
- **Fast feedback** - Know daily if you're on track

## Installation

```bash
git clone https://github.com/BayramAnnakov/2026-coach ~/.claude/skills/2026-coach
```

## Usage

In Claude Code:
```
/2026-coach
```

The skill also works in Claude.ai and other Agent Skills-compatible assistants.

## What It Does

### 1. Discovery Phase
Guides you through 4 rounds of strategic questions:
- **Current State:** Role, stage, resources, constraints
- **Vision:** Where you want to be by Dec 2026
- **Strategy:** What worked/didn't in 2025, biggest bets
- **Process:** Available time, key behaviors, distractions

### 2. Goal Hierarchy
Builds a structured goal system:
```
Outcome Goal (Annual): Clear north star
├── Q1 Milestone
├── Q2 Milestone
├── Q3 Milestone
└── Q4 Milestone
    └── Weekly Process Goals
        └── Daily Behaviors (checkable)
```

### 3. Process Goal Conversion
Transforms outcomes into controllable behaviors:
- "Hit $100K MRR" → "Send 20 outbound messages daily"
- "Write a book" → "Write 500 words before breakfast"
- "Get fit" → "Exercise 30 mins before 9am"

### 4. Creates Tracking Files
- `2026_PLAN.md` - Annual strategic plan with quarterly roadmap
- `COACHING_CONTEXT.md` - Context for ongoing AI coaching sessions
- `WEEK_XX.md` - Weekly process goals with daily checklists

## Environment Compatibility

| Environment | Behavior |
|-------------|----------|
| Claude Code | Uses `AskUserQuestion` for interactive multi-choice discovery |
| Claude.ai | Falls back to conversational questions |
| Other agents | Works with any Agent Skills-compatible assistant |

## Companion Skills

For tracking your process goals:
- [ActivityWatch Analysis Skill](https://github.com/BayramAnnakov/activitywatch-analysis-skill) - Track focus time, app switching, deep work sessions

## File Structure

```
2026-coach/
├── SKILL.md                              # Main skill definition
├── README.md                             # This file
└── references/
    ├── annual-plan-template.md           # Year plan template
    ├── weekly-plan-template.md           # Weekly checklist template
    └── coaching-context-template.md      # AI coaching context template
```

## Validation

This skill passes the [Agent Skills specification](https://agentskills.io/specification):

```bash
npm install -g skills-ref
skills-ref validate ~/.claude/skills/2026-coach
# Valid skill: /Users/.../.claude/skills/2026-coach
```

## License

MIT

## Author

[Bayram Annakov](https://github.com/BayramAnnakov)

---

*Perfect timing: It's January 2026 - everyone is goal-setting. Don't wait for "when you have time."*
