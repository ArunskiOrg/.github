<!-- Link to the GitHub issue this PR delivers. Use "Closes" or "Fixes" (interchangeable, both auto-close the issue) only on the one PR that finishes the story. If the story spans multiple PRs, use "Refs" on every other one (no auto-close) and list them all under Cross-referenced PRs below. --> Closes ArunskiOrg/<planning project>#<issue-number>

## Cross-referenced PRs

<!-- Optional, except mandatory on a Closes/Fixes PR whose story spans multiple PRs: list every sibling PR for the story here, in merge order if one is required, even without a strict dependency. Omit this section otherwise. -->

## What changed

<!-- Describe the changes made. Focus on the "why" of each decision, not a line-by-line summary — the diff covers what changed. -->

## How to test locally

<!-- Step-by-step instructions to run and verify the change on a developer's machine. Include any env vars, seed data, or services that must be running. -->

## How to test in QA

<!-- Steps specific to the QA environment. If identical to local, write "Same as local." -->

## Tests completed

<!-- List the automated tests added or modified, and any manual test cases run. -->
- [ ] Unit tests pass (`pytest` / `npm test`)
- [ ] Linter passes (`ruff` / `tsc`)
- [ ] Coverage threshold met (90% line + branch)
- [ ] Manual smoke test performed

## Standards checklist

- [ ] PR title matches `#<story-number>: <description>`
- [ ] Tests use Given / When / Then structure
- [ ] Any new app-to-app interface has an OpenAPI contract
- [ ] Deployment items added to the canonical deployment plan
- [ ] Reviewer verified: all of the story's acceptance criteria are met, with no additional scope added beyond direct dependencies of those acceptance criteria

---

*PR template v1.6 — the canonical PR summary checklist, defined in [ArunskiOrg/.github](https://github.com/ArunskiOrg/.github/blob/main/.github/pull_request_template.md). The detailed rules behind each item are canonical in [`dev-standards.md`](https://github.com/ArunskiOrg/org-standards/blob/main/docs/standards/dev-standards.md) (ArunskiOrg/org-standards).*
