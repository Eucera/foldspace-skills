# Foldspace Skills

Agent skills for building [Foldspace](https://foldspace.readme.io) actions with AI coding assistants. These skills guide your AI agent through a structured workflow — from requirement gathering and codebase scanning to implementation and review — so Foldspace actions are correctly wired, error-handled, and styled to match your application.

## Available Skills

| Skill | Slash Command | Description |
|-------|---------------|-------------|
| [create-foldspace-action](create-foldspace-action/SKILL.md) | `/create-foldspace-action` | Walks through implementing Text-Only Actions, Chatterblocks, and Shared State |

## Installation

### Cursor

**Option A — Let the agent install it for you**

Open Cursor Agent and type:

```
/create-skill create foldspace action from https://github.com/Eucera/foldspace-skills
```

The agent will fetch the skill from this repository and install it into your personal skills directory.

**Option B — Manual install**

Clone the repository into your Cursor skills directory:

```bash
git clone https://github.com/Eucera/foldspace-skills.git ~/.cursor/skills/foldspace-skills
```

Or copy just the skill you need:

```bash
mkdir -p ~/.cursor/skills/create-foldspace-action
curl -o ~/.cursor/skills/create-foldspace-action/SKILL.md \
  https://raw.githubusercontent.com/Eucera/foldspace-skills/main/create-foldspace-action/SKILL.md
```

Once installed, the skill activates automatically when you ask to create Foldspace actions, or you can invoke it directly with `/create-foldspace-action`.

### Claude Code

Clone the repository into your Claude Code skills directory:

```bash
git clone https://github.com/Eucera/foldspace-skills.git ~/.claude/skills/foldspace-skills
```

Or copy just the skill you need:

```bash
mkdir -p ~/.claude/skills/create-foldspace-action
curl -o ~/.claude/skills/create-foldspace-action/SKILL.md \
  https://raw.githubusercontent.com/Eucera/foldspace-skills/main/create-foldspace-action/SKILL.md
```

Once installed, invoke the skill with `/create-foldspace-action` or let Claude pick it up automatically when you ask to build Foldspace actions.

## Usage

After installation, start a conversation in your project and either:

- Type `/create-foldspace-action`
- Or ask naturally: *"Create a Foldspace action for inviting users"*

The agent will walk you through a 7-step workflow:

1. **Requirement Gathering** — Provide action IDs, descriptions, and input schemas
2. **Codebase Reconnaissance** — The agent scans your project for patterns, styles, and conventions
3. **Product Planning** — Review a proposal for each action (Text-Only vs Chatterblock)
4. **Agent Initialization Verification** — Confirms the Foldspace SDK and agent are set up in your code
5. **Implementation** — Production-ready code with validation and error handling
6. **Post-Implementation Review** — Wiring check to verify everything is connected correctly
7. **Shared State Upsell** — Optional: sync your app's UI with the Foldspace agent in real time

## Resources

- [Foldspace Documentation](https://foldspace.readme.io)
- [Installing the SDK](https://foldspace.readme.io/docs/installing-the-sdk)
- [Cursor Skills Documentation](https://docs.cursor.com/context/skills)
- [Claude Code Skills Documentation](https://docs.anthropic.com/en/docs/claude-code/skills)
