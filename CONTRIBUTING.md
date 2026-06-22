# Contributing to super-engineer

Thanks for being here. This repo gets better every time someone shares a skill they'd actually use. This guide explains how to contribute one.

## Ways to contribute

- **Add a new skill** — the main event.
- **Improve an existing skill** — sharper checklists, better examples, fixes for outdated advice.
- **Fix bugs** — broken commands, dead links, typos.
- **Propose ideas** — open an issue with the `skill-proposal` label.

## Quick start: add a skill

1. **Fork** the repo and create a branch: `git checkout -b add-<skill-name>`.
2. **Create a folder** named after your skill in kebab-case (e.g. `api-design`, `react-testing`).
3. **Copy the template:** `cp SKILL_TEMPLATE.md <skill-name>/SKILL.md` and fill it in.
4. **Register it** by adding a row to the "Skills in this repo" table in [README.md](README.md).
5. **Open a PR** using the pull request template.

```bash
git clone https://github.com/divshekhar/super-engineer.git
cd super-engineer
mkdir my-skill
cp SKILL_TEMPLATE.md my-skill/SKILL.md
# ...write your skill...
```

## What makes a good skill

A skill is accepted when it would genuinely help an agent do a real task better than it would unprompted. We optimize for **signal**, not volume.

A great skill is:

- **Opinionated** — it makes decisions, it doesn't list options. "Use UUID v7 for public IDs" beats "consider various ID strategies."
- **Actionable** — concrete steps, checklists, and copy-pasteable code, not vague principles.
- **Self-contained** — an agent can follow it without external context.
- **Correct** — examples run; advice reflects current best practice. Outdated guidance gets rejected.
- **Stack-honest** — if it's language-specific, say so. If it's universal, prove it with examples across stacks.
- **Trigger-clear** — state exactly when the skill should fire.

A skill is **not** a good fit if it's a thin wrapper around a single command, duplicates an existing skill without improving it, or is purely promotional.

## SKILL.md requirements

Every `SKILL.md` must include:

1. **A title** — `# <Skill Name>`.
2. **A trigger line** — how the skill is invoked, e.g. `## Trigger: \`/skill-name\``.
3. **A one-paragraph summary** — what it does and who it's for.
4. **Agent behavior rules** — what the agent must and must not do.
5. **The actual instructions** — steps, checklists, examples.

Keep individual files focused. If a skill grows huge, that's fine when the content earns it (see `project-setup`), but prefer clarity over length.

## Style

- Write for an agent reading top-to-bottom. Put rules before examples.
- Use fenced code blocks with language hints.
- Prefer tables for decision matrices and "when to use X" comparisons.
- Use `✗`/`✓` or `WRONG`/`RIGHT` to contrast anti-patterns with the fix.
- Keep lines reasonable; Markdown should render cleanly on GitHub.

## Review process

1. A maintainer reviews for fit, correctness, and clarity.
2. We may request changes — most skills go through a round or two.
3. Once merged, your skill is live and you're credited in the PR history.

## Licensing of contributions

By submitting a contribution you agree that it is licensed under the project's [MIT License](LICENSE), and you confirm you have the right to contribute it (it's your work, or you have permission to share it).

## Code of Conduct

All participation is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). Be kind, be constructive.

---

Questions? Open an issue. We're glad you're here.
