# Security Policy

This repository contains **skills** — Markdown instruction sets for AI coding agents. It ships no runtime code or packages, so the main security surface is the *content* of the skills themselves.

## Reporting a concern

If you find a skill that instructs an agent to do something harmful, insecure, or destructive — for example, recommending an insecure pattern as best practice, leaking secrets, or running dangerous commands — please report it.

- Open a [GitHub issue](https://github.com/divshekhar/super-engineer/issues) for non-sensitive concerns, or
- Use [GitHub private vulnerability reporting](https://github.com/divshekhar/super-engineer/security/advisories/new) for anything sensitive.

Please include the skill name, the specific guidance in question, and why it's a problem.

## Using skills safely

Skills tell an autonomous agent how to act. Before adopting any skill:

- **Read it.** Treat a skill like code you're about to run — because an agent will act on it.
- **Review commands** it asks the agent to execute, especially anything that installs tools, modifies git history, or touches credentials.
- **Run agents with appropriate permissions.** Don't grant an agent broader access than the task needs.

We review contributed skills for correctness and safety, but you are responsible for what you run in your own environment.
