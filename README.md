# super-engineer

> A community-driven collection of [Claude Code](https://claude.com/claude-code) **skills** that level up how AI agents build, ship, and maintain software.

Skills are reusable, version-controlled instruction sets that teach an AI coding agent how to do a task *the way a senior engineer would*. This repo is a home for high-quality, opinionated skills — bring yours, use ours, and let's raise the floor on agent-assisted engineering together.

<p align="left">
  <a href="LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-blue.svg"></a>
  <a href="CONTRIBUTING.md"><img alt="PRs Welcome" src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg"></a>
  <img alt="Skills" src="https://img.shields.io/badge/skills-1-orange.svg">
</p>

---

## What is a skill?

A **skill** is a folder containing a `SKILL.md` file. The Markdown holds the instructions an agent reads when the skill is triggered — conventions, checklists, code patterns, and guardrails. When you type the skill's trigger (e.g. `/project-setup`) in Claude Code, the agent loads those instructions and follows them.

Think of each skill as the distilled playbook of an expert, made executable by an agent.

## Skills in this repo

| Skill | Trigger | What it does |
|-------|---------|--------------|
| [project-setup](project-setup/SKILL.md) | `/project-setup` | Scaffolds a production-grade project (TS/Python/Go/Rust) with top-1% engineering standards: strict configs, branded types, constants architecture, pre-commit gates, and a full `skills/` reference library. Includes a 1,900-line engineering operating manual covering concurrency, databases, security, performance, observability, and testing. |

> Adding a skill? Add a row here and open a PR. See [Contributing](#contributing).

## Installation

### Option 1 — Use a single skill

Copy the skill folder into your project's `.claude/skills/` directory (or your personal `~/.claude/skills/`):

```bash
git clone https://github.com/divshekhar/super-engineer.git
cp -r super-engineer/project-setup ~/.claude/skills/project-setup
```

Then invoke it in Claude Code:

```
/project-setup
```

### Option 2 — Clone the whole collection

```bash
git clone https://github.com/divshekhar/super-engineer.git ~/.claude/super-engineer
```

Point your agent at the skills you want, or symlink individual ones into `~/.claude/skills/`.

> Skill loading details differ slightly across agents and Claude Code versions. See the [Claude Code skills docs](https://docs.claude.com/en/docs/claude-code) for the current mechanism.

## Repository layout

```
super-engineer/
├── project-setup/          ← a skill (one folder per skill)
│   └── SKILL.md            ← the skill's instructions
├── SKILL_TEMPLATE.md       ← copy this to start a new skill
├── CONTRIBUTING.md         ← how to add a skill
├── CODE_OF_CONDUCT.md
├── LICENSE                 ← MIT
└── README.md
```

Each skill lives in its own top-level folder containing, at minimum, a `SKILL.md`.

## Contributing

Contributions are the whole point. Whether you're fixing a typo, sharpening a checklist, or submitting an entirely new skill — you're welcome here.

1. Read [CONTRIBUTING.md](CONTRIBUTING.md).
2. Copy [`SKILL_TEMPLATE.md`](SKILL_TEMPLATE.md) into a new folder `your-skill-name/SKILL.md`.
3. Write your skill, add a row to the table above, and open a PR.

New skill ideas? Open an [issue](https://github.com/divshekhar/super-engineer/issues) with the `skill-proposal` label.

## Community standards

By participating you agree to uphold our [Code of Conduct](CODE_OF_CONDUCT.md).

## License

[MIT](LICENSE) © 2026 divshekhar and the super-engineer contributors.

Every skill you contribute is licensed to the project under MIT. By submitting a PR you confirm you have the right to do so.
