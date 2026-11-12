# Handoff

## Goal

Resolve the assigned milestone using the role boundaries in `AGENTS.md`.

## Running it

- Node 22 or newer; Git and GitHub CLI authenticated for this repository.
- The primary OpenCode agent is `supervisor`, with `.bive/prompts/SUPERVISOR.md` as its system prompt.
- Read `ROADMAP.md` and the repository's issues and pull requests for the current assignment.
- No registry participation, external services, private data, or background workers are configured.

## Decisions

- The supervisor alone merges or closes pull requests, using merge commits. Coordinators review and hand over; delegates implement their assigned issues.

## Tasks

Await the owner's milestone assignment.
