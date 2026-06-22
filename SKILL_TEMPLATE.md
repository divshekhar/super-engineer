# <Skill Name>

## Trigger: `/<skill-name>` or "<natural language phrase that should invoke this>"

<One paragraph: what this skill does, who it's for, and what outcome it produces.
Keep it concrete. An agent should know from this alone whether the skill applies.>

---

# AGENT BEHAVIOR RULES

Before doing anything, the agent must:

1. <First required action — e.g. detect context, ask clarifying questions, confirm scope>
2. <Second required action>
3. <Confirm the plan with the user before making changes, if applicable>

Never:

- <An action the agent must not take>
- <Another guardrail>
- <Report success before the validation checklist passes>

---

# INSTRUCTIONS

## Step 1: <Name>

<What to do. Include commands, code, and decision rules. Be specific.>

```bash
# example command
```

## Step 2: <Name>

<Continue. Use tables for decisions:>

| Situation | Do this | Don't |
|-----------|---------|-------|
| ...       | ...     | ...   |

## Step N: Validation

Do NOT report "done" until all of these pass:

```
□ <Checklist item>
□ <Checklist item>
□ <Checklist item>
```

---

# REFERENCE (optional)

<Deeper background, anti-patterns, or an operating manual the steps above draw from.
Use WRONG/RIGHT contrasts:>

```python
# WRONG: <why it's wrong>
...

# RIGHT: <the fix>
...
```

---

<!--
Before opening your PR:
- [ ] Folder is kebab-case and matches the skill name.
- [ ] Trigger is stated clearly at the top.
- [ ] Added a row to the table in README.md.
- [ ] Examples are correct and runnable.
- [ ] Removed this template comment and any unused placeholder sections.
-->
