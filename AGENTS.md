# Repo Agent Bootstrap

This repository is governed by the user's local Repo Operator system.

## Terminal entry points
```bash
~/repo-tools/agent/repo-work <repo>
~/repo-tools/agent/repo-work --help
~/repo-tools/agent/repo-status
```
Read repo-local authority first. Global Repo Work OS and active tools live under `~/repo-tools/reference-authorities/repo-work-os` and `~/repo-tools/manifests/ACTIVE_SCRIPTS.md`. Hallmark lives under `~/repo-tools/reference-authorities/hallmark`.

## Operating law
- Lock exact repo/worktree/branch/SHA/remote before mutation.
- Unattended work only on isolated `work/*` worktrees.
- Never substitute or mutate another canonical repo.
- Validation and exact-SHA GitHub checks must pass before merge eligibility.
- Merge to main/default is permitted ONLY when every required check is green: never with `--admin`, never force-pushed, never on a RED or UNPROVEN result. A blocker that cannot go green on its own — a credential, an account setting, a product decision — is reported as a NAMED STOP, never merged around.
- Use Claude Design routing for material UI/UX work when useful; not backend-only work.
