<!-- Link to the GitHub issue this PR delivers. Note: "Fixes" may be substituted for "Closes" --> Closes ArunskiOrg/<planning project>#<issue-number>

## Cross-referenced PRs

<!-- Optional. List other PRs that must merge together with this one, or in a specific order. Omit this section if none apply. -->

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
- [ ] Reviewer verified: all of the story's acceptance criteria are met, with no additional scope added beyond direct dependencies of those acceptance criteria

---

*PR template v1.3 — defined in [ArunskiOrg/.github](https://github.com/ArunskiOrg/.github/blob/main/.github/pull_request_template.md)*
