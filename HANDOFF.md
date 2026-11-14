# Handoff

## Goal

Resolve the assigned milestone using the role boundaries in `AGENTS.md`.

## Running it

- Node 22 or newer; Git and GitHub CLI authenticated for this repository.
- There is no default agent: the owner selects the OpenCode agent and model for each assignment. (The workspace
  previously started a `supervisor` agent with `.bive/prompts/SUPERVISOR.md` as its system prompt; that prompt is now
  a retired compatibility pointer with no authority.)
- Read `ROADMAP.md` and the repository's issues and pull requests for the current assignment.
- No registry participation, external services, private data, or background workers are configured.

## Decisions

- **Owner-approved coordinator teams (owner, 2026-11-13)**: prefer the strongest suitable verified-free usable
  coordinator; otherwise recommend a suitable usable coordinator from the current supervisor provider. Before launch
  or substitution, ask the owner to approve the concrete team, cost, availability evidence, alternatives, and fallback,
  then stop and wait. No silent coordinator substitution or inference that unknown pricing is free. Existing
  qualifications, allow-lists, delegate fallback, and role rights remain unchanged. See `docs/PROVIDERS.md` and the
  supervisor's project additions.
- The owner alone merges or closes pull requests, using merge commits. Coordinators review, open pull requests and
  hand over; delegates implement their assigned issues and never open a pull request.
- **Owner authority (owner, 2026-11-14)**: the human owner alone authorizes work and merges, merges or closes pull
  requests, approves teams and gates, arbitrates shared files, and releases tests; no agent approves or merges into
  `main`. A qualification or a green check never grants authority.
- **Read-only advisor (owner, 2026-11-14)**: an advisor answers one question about the current worktree, read-only,
  then stops: no writes, comments, reviews, commands, or launches. Advice is never authorization, and an advisor is
  not a standing manager or a rung of authority.
- **Hand-over launch (owner, 2026-11-14)**: advice-prepared launch text is a proposal until the owner records approval
  of the scope and the team.

## Tasks

Await the owner's milestone assignment.
