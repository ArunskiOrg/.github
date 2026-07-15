# .github

Org-wide shared and default files for ArunskiOrg. This repo is consumed by other repos, not developed against directly — treat changes here as load-bearing.

## Contents

| Path | Purpose |
|---|---|
| `.github/workflows/pr-standards.yml` | Reusable workflow enforcing PR title format and required PR template sections. Called via `uses: ArunskiOrg/.github/.github/workflows/pr-standards.yml@main` from each product repo's own `pr-standards.yml` caller. |
| `.github/workflows/sync-pr-template.yml` | Pushes `pull_request_template.md` out to the product repos listed in its matrix whenever the template changes on `main`. |
| `.github/pull_request_template.md` | Canonical PR template; source of truth synced to product repos. |
| `.github/ISSUE_TEMPLATE/` | Org-wide default issue forms (bug, capability, decision, epic, feature, risk, spike, story, task) — used as the fallback by any repo without its own issue templates. |
| `CODEOWNERS` | Default code ownership for this repo. |
| `.github/dependabot.yml` | Dependabot config for this repo's own GitHub Actions dependencies. |

## Related repos

- [`org-standards`](https://github.com/ArunskiOrg/org-standards) — org-wide ADRs, dev standards, and the decision-log docs site
- [`dotfiles`](https://github.com/ArunskiOrg/dotfiles) — personal machine config backup (Claude Code config, shell, PowerShell)

## History

Split out of `RandomOrganizer2026` (now archived) on 2026-07-15, preserving commit history for `.github/` and `CODEOWNERS` via `git filter-repo`, then merged with this repo's pre-existing issue-template history.
