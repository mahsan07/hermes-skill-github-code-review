---
name: hermes-skill-github-code-review
description: Review pull requests for correctness, security, tests, and maintainability. Use when a user asks for this workflow or a closely related task.
---

# GitHub Code Review

Review pull requests or diffs with an evidence-first approach. Focus on correctness, security, regressions, tests, and maintainability.

## Workflow

1. Read the PR description, changed files, surrounding code, and relevant tests.
2. Trace changed behavior through callers, inputs, outputs, persistence, and error paths.
3. Check authentication, authorization, secrets, injection, unsafe deserialization, and sensitive logging.
4. Check test coverage and whether tests verify the changed behavior rather than implementation trivia.
5. Report findings with severity, file/line, impact, and a concrete remediation.
6. State what was checked and any remaining uncertainty.

Do not modify, approve, merge, or comment on the remote PR unless the user explicitly asks for that action.
