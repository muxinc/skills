# Mux Agent Skills

Skills that teach AI coding agents how to build with [Mux](https://mux.com) using today's published documentation.

## What's included

```
skills/mux-docs/
└── SKILL.md    # Live docs discovery: routes agents to Mux's current
                # LLM-ready docs (mux.com/llms.txt, collection indexes,
                # per-page markdown) so answers come from today's
                # published docs, not snapshots or model memory
```

Mux publishes every docs page as LLM-ready markdown, indexed at [mux.com/llms.txt](https://www.mux.com/llms.txt). The `mux-docs` skill teaches agents to fetch the relevant page at answer time — API shapes, guides, Mux Data, Mux Robots, pricing — and to self-heal through `llms.txt` when URLs move. No documentation content lives in this repo, so nothing here goes stale.

## Installation

### Claude Code plugin

This repository is a Claude Code plugin marketplace:

```
/plugin marketplace add muxinc/skills
/plugin install mux@mux
```

### skills CLI

```bash
npx skills add muxinc/skills
```

### Mux CLI

The [Mux CLI](https://github.com/muxinc/cli) ships the `mux-docs` skill embedded in every binary. `mux skills install` copies it into `~/.claude/skills` for automatic loading, and `mux skills update` refreshes local copies after upgrading the CLI.

### Manual

Copy `skills/mux-docs/` into your agent's skills directory (e.g. `~/.claude/skills/`). The skill is a single `SKILL.md` with no dependencies and works in any agent that supports the [Agent Skills](https://agentskills.io) format.

## Usage

Once installed, your agent uses the skill automatically for Mux questions:

- "What's the request body to create a live stream?"
- "How do I get a thumbnail at the 30-second mark?"
- "Which Mux Robots task generates chapters?"

Answers cite the docs page they came from.

## License

MIT
