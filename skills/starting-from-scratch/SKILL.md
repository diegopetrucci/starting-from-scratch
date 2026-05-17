---
name: starting-from-scratch
description: Review a codebase and say what should change if it were being started again from scratch. Use when the user wants a reset-style retrospective, architecture do-over, or "what would you change if you restarted this project?" analysis. Start by asking whether to analyze a single commit, the branch against its base, or the whole project.
license: MIT
metadata:
  author: Diego Petrucci
  version: "1.1"
---

# Starting From Scratch

Answer from the perspective of restarting the project, not just fixing the current branch.

## Workflow

1. Ask the user which scope to analyze: a single commit, the current branch against its base, or the whole project.
2. Inspect the chosen scope deeply enough to understand the decisions, tradeoffs, and repeated pain points behind it.
3. Identify the highest-leverage things to do differently if starting over: architecture, tooling, boundaries, workflows, testing, naming, or scope.
4. Prioritize structural changes over local cleanup.
5. Report concrete changes, why each matters, and what cost or problem it would avoid.

## Constraints

- Do not assume the scope. Ask first.
- Do not give generic best practices unless they are clearly supported by the project's history or current shape.
- Prefer a short, opinionated answer over a long audit.
