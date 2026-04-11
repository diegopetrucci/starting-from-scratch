---
name: start-over-review
description: Review a project's full history and current state, then answer what should change if starting over from scratch. Use when the user wants a reset-style retrospective grounded in the whole project rather than just the current branch or latest diff.
license: MIT
metadata:
  author: Diego Petrucci
  version: "1.0"
---

# Start Over Review

Answer from the perspective of restarting the project, not just fixing the current branch.

## Workflow

1. Inspect the full project context: current code, recent commits, major historical changes, and any repeated pain visible in the repo.
2. Identify the highest-leverage things to do differently if starting over: architecture, tooling, boundaries, workflows, testing, naming, or scope.
3. Prioritize structural changes over local cleanup.
4. Report concrete changes, why each matters, and what cost or problem it would avoid.

## Constraints

- Do not limit the review to `HEAD` or the open branch unless the user explicitly asks.
- Do not give generic best practices unless they are clearly supported by the project's history or current shape.
- Prefer a short, opinionated answer over a long audit.
