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

---

## Installation

### Option A: Claude Code (Easiest)

Just tell Claude Code to install the skill:

```
Install the skill from https://github.com/BayramAnnakov/2026-coach
```

Claude Code will handle the git clone automatically. Then use:
```
/2026-coach
```

**Alternative - manual install:**
```bash
git clone https://github.com/BayramAnnakov/2026-coach ~/.claude/skills/2026-coach
```

### Option B: Claude.ai / Claude Desktop (No Installation)

**You don't need to install anything!** Just copy-paste this prompt:

```
Please act as my executive coach and help me plan my 2026 using the process goals methodology.

Research shows process goals are 15x more effective than outcome goals (Williamson et al. 2022):
- Outcome goal: "Make $100K" (you don't control this)
- Process goal: "Send 20 messages daily" (you control this 100%)

Please guide me through:
1. Discovery - Ask me about my current situation, vision for 2026, what worked/didn't in 2025
2. Create one clear outcome goal (my north star)
3. Break it into quarterly milestones
4. Convert to weekly process goals (behaviors I control)
5. Create daily checklists

At the end, create these files for me:
- 2026_PLAN.md - my annual plan
- COACHING_CONTEXT.md - context for future coaching sessions
- WEEK_01.md - first week's process goals with checkboxes
```

### Option C: VS Code / GitHub Copilot

Copy the skill to your project's skills folder:

```bash
# Recommended location (VS Code / Copilot)
git clone https://github.com/BayramAnnakov/2026-coach .github/skills/2026-coach

# Or legacy location (also supported)
git clone https://github.com/BayramAnnakov/2026-coach .claude/skills/2026-coach
```

### Option D: Manual Download

1. Go to https://github.com/BayramAnnakov/2026-coach
2. Click the green **"Code"** button → **"Download ZIP"**
3. Unzip and move the folder to one of these locations:

| Platform | Location |
|----------|----------|
| Claude Code (personal) | `~/.claude/skills/2026-coach/` |
| Claude Code (project) | `.claude/skills/2026-coach/` |
| VS Code / Copilot | `.github/skills/2026-coach/` |

**Finding hidden folders:**
- **Mac:** Press `Cmd+Shift+.` in Finder
- **Windows:** View → Show → Hidden items
- **Linux:** Press `Ctrl+H` in file manager

---

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

---

## Compatibility

| Platform | How to Use | Install Required? |
|----------|------------|-------------------|
| **Claude Code** | `/2026-coach` | Yes (Option A) |
| **Claude Desktop** | Paste prompt | No (Option B) |
| **Claude.ai (web)** | Paste prompt | No (Option B) |
| **VS Code + Copilot** | Auto-discovered | Yes (Option C) |
| **Cursor** | Auto-discovered | Yes (Option C) |
| **ChatGPT / other AI** | Paste prompt | No (Option B) |

---

## Companion Skills

For tracking your process goals:
- [ActivityWatch Analysis Skill](https://github.com/BayramAnnakov/activitywatch-analysis-skill) - Track focus time, app switching, deep work sessions

---

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

---

## FAQ

**Q: Do I need to know how to code?**
A: No! Use Option B (just copy-paste the prompt) - works instantly.

**Q: Does this work with ChatGPT?**
A: Yes! Copy the prompt from Option B. It works with any AI assistant.

**Q: What if Claude Code can't clone the repo?**
A: Use Option D (manual download) or paste the prompt from Option B.

**Q: Where do my plan files get saved?**
A: The AI will ask you where to save them, or display them in chat for you to copy.

**Q: How do I update the skill?**
A: Run `git pull` in the skill folder, or re-download and replace the files.

---

## License

MIT

## Author

[Bayram Annakov](https://github.com/BayramAnnakov)

---

*Perfect timing: It's January 2026 - everyone is goal-setting. Don't wait for "when you have time."*

---

## Sources

- [Agent Skills Specification](https://agentskills.io/specification)
- [Claude Code Skills Docs](https://code.claude.com/docs/en/skills)
- [VS Code Agent Skills](https://code.visualstudio.com/docs/copilot/customization/agent-skills)
