# Claude Code Guide

Claude Code skill for Claude Code resources.

## Setup

```bash
git clone https://github.com/wangjing0/claude-code-guide.git
cd claude-code-guide
```

Then install the skill (pick one):

```bash
# Option 1 — install from the packaged file
claude skill install claude-code-guide.skill

# Option 2 — copy the source folder directly
cp -r claude-code-guide ~/.claude/skills/
```

Restart Claude Code. The skill is ready.

## Skills

### claude-code-guide

Answers questions about Claude Code by fetching live information from official Anthropic docs and community resources at runtime.

**Install globally:**
```bash
claude skill install claude-code-guide.skill
```

**Or copy the folder directly:**
```bash
cp -r claude-code-guide ~/.claude/skills/
```

**Usage:** Ask any Claude Code question naturally — the skill triggers automatically, or invoke it explicitly with `/claude-code-guide`.

**Example in Claude Code:**
```bash
/claude-code-guide What is the difference between CLAUDE.md and MEMORY.md?
```

**Sources it queries:**
- [Claude Code docs](https://code.claude.com/docs/en/overview)
- [Anthropic blog](https://claude.com/blog)
- [r/ClaudeCode](https://www.reddit.com/r/ClaudeCode/) and [r/ClaudeAI](https://www.reddit.com/r/ClaudeAI/)

## Files

```
claude-code-guide/
├── claude-code-guide/        # Skill source
│   ├── SKILL.md
│   └── references/
│       └── docs-index.md
└── claude-code-guide.skill   # Packaged for distribution
```
