# Skills

AI agent skills that operationalize the techniques from the [Seam Up](../docs/01-thesis.md) methodology. Each skill gives an AI coding agent a structured workflow for one step of the Seam Up process.

## The workflow

The skills follow a natural sequence, though you don't have to use all of them or use them in order:

```
Product spec
    │
    ▼
┌─────────────┐
│ distill-spec │  Translate to engineering spec
└─────┬───────┘
      │
      ▼
┌──────────┐
│ research │  Explore codebase, surface questions, draft ideas (personal)
└─────┬────┘
      │
      ▼
  [ shaping session ]  ← team collaboration
      │
      ▼
┌─────────────┐
│ scope-split │  Document scopes, decisions, tradeoffs, seams (shared)
└─────┬───────┘
      │
      ▼
  [ build phase ]  ← individual work within scopes
      │
      ▼
┌─────────────┐
│ seam-change │  Propose changes when seams shift mid-build
└─────────────┘
```

## Skills

| Skill | Purpose | Artifact layer |
|-------|---------|---------------|
| [distill-spec](distill-spec/SKILL.md) | Translate a product spec into a focused engineering spec | Shared |
| [research](research/SKILL.md) | Explore the codebase against a spec, surface questions and design ideas for shaping | Personal |
| [scope-split](scope-split/SKILL.md) | Document scope boundaries, design decisions, tradeoffs, and seam agreements | Shared |
| [seam-change](seam-change/SKILL.md) | Draft a proposal when a seam agreement needs to change mid-build | Shared |

## Installation

Skills use the `SKILL.md` format with YAML frontmatter. They are written in plain markdown with no references to specific tool APIs, so they work with any AI coding tool that supports skill files.

### Claude Code

Add each skill's `SKILL.md` as a custom instructions file in your project or user settings. You can either copy the files or reference them directly:

```sh
# Add to your project's .claude/ directory
mkdir -p .claude/skills
cp skills/*/SKILL.md .claude/skills/

# Or add individual skills as custom instructions
# In Claude Code, use /add-custom-instructions and point to the SKILL.md file
```

Alternatively, add the skill content to `.claude/settings.json` under `customInstructions` or reference the files in your project's `CLAUDE.md`.

### OpenCode

Copy or symlink each skill directory into `~/.config/opencode/skills/`:

```sh
# Copy all skills
cp -r skills/* ~/.config/opencode/skills/

# Or symlink individual skills
ln -s "$(pwd)/skills/distill-spec" ~/.config/opencode/skills/distill-spec
```

### Other tools

Each skill is a standalone `SKILL.md` file with YAML frontmatter containing `name` and `description` fields. Copy or point your tool at the file however it expects skill or instruction definitions. The format is simple enough that any tool that reads markdown can use them.

## Methodology

These skills are companions to the [Seam Up book](../docs/01-thesis.md). The book explains the reasoning; the skills provide the operational workflows. Start with the book if you want to understand why these practices work.
