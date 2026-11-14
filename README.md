# Milestone workspace

A minimal, reusable Bive workspace for the human owner, coordinators, delegates, and read-only advisors. It contains role instructions, report templates, and required-check workflows, but no project history or user data.

Read `AGENTS.md` and `HANDOFF.md` first, then the prompt of the role the owner assigns. There is no default OpenCode
agent (the workspace once defaulted to the `supervisor` agent): the owner selects the agent and the model for each
assignment. `.bive/prompts/SUPERVISOR.md` is a retired compatibility pointer; it grants no authority.

## Checks

Run `node --check .github/scripts/check-merge-gate.mjs`, `node --check .github/scripts/merge-gate-lib.mjs`, and `node --test tests/*.test.ts` with Node 22 or newer.

## Repository settings

Use merge commits only. On each active milestone branch require pull requests, `tests`, and `merge-gate`, including for administrators; prohibit deletion and force pushes. On `main` require pull requests and `tests`. Protect the branches after initial setup, and verify the settings through GitHub's API. A green check alone is not branch protection.

Creating a repository from this template copies files, not issues, pull requests, labels, or branch protection. Configure each repository independently.
