# Guide Me

A Claude skill for guiding users to Claude Code resources.

## Setup

```bash
git clone https://github.com/wangjing0/claude-code-guide.git
cd claude-code-guide
```

Then install the skill (pick one):

```bash
# Option 1 — install from the packaged file
claude skill install guide-me.skill

# Option 2 — copy the source folder directly
cp -r guide-me ~/.claude/skills/
```

Restart Claude Code. The skill is ready.

## Skills

### guide-me

Answers questions about Claude Code by fetching live information from official Anthropic docs and community resources at runtime.

**Install globally:**
```bash
claude skill install guide-me.skill
```

**Or copy the folder directly:**
```bash
cp -r guide-me ~/.claude/skills/
```

**Usage:** Ask any Claude Code question naturally — the skill triggers automatically, or invoke it explicitly with `/guide-me`.

**Example in Claude Code:**
```bash
/guide-me What is the difference between CLAUDE.md and MEMORY.md?
```

**Sources it queries:**
- [Claude Code docs](https://code.claude.com/docs/en/overview)
- [Anthropic blogs](https://claude.com/blog)
- [r/ClaudeCode](https://www.reddit.com/r/ClaudeCode/) and [r/ClaudeAI](https://www.reddit.com/r/ClaudeAI/)
- [r/Anthropic](https://www.reddit.com/r/Anthropic/) and [r/claude](https://www.reddit.com/r/claude/)

## Files

```
claude-code-guide/
├── guide-me/                 # Skill source
│   ├── SKILL.md
│   └── references/
│       └── docs-index.md
└── guide-me.skill            # Packaged for distribution
```
