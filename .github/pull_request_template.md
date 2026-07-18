<!-- Linked issue. Example: `Closes ArunskiOrg/rag-sample-app#42` - [github docs](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue)

Elements:
- KEYWORD options:
  1. Auto-closing action: "Closes" for stories; "Fixes" for bugs
     - auto-closes the issue
     - Use an auto-closing action on exactly one PR per story - the PR that definitively finishes the story
     - Do NOT apply this action to any PR related to evergreen stories
  2. Referencing action: "Refs"
     - Does not close the issue
     - If a story is labeled "evergreen", use this action exclusively (no Closes or Refs)
     - if a story spans multiple PRs, all but one PR uses "Refs"
- REPOSITORY:
  - Every project has a planning repo that holds its ADRs and github issues.
  - Identified by naming convention. Example: `rag-sample-app` uses `rag-sample` as its planning repo
  - if the PR is in the same project where the story is defined, omit `ArunskiOrg/<REPOSITORY>`. The format becomes `<KEYWORD> #<ISSUE-NUMBER>`
- ISSUE-NUMBER: the issue that this PR addresses  
-->
<KEYWORD> ArunskiOrg/<REPOSITORY>#<ISSUE-NUMBER>

## Cross-referenced PRs
<!-- Mandatory when a story spans multiple PRs; otherwise omitted. List all related PRs for the story. Show dependencies where they exist.

Example: `This PR closes the issue; merge all others first: backend PR ArunskiOrg/rag-sample-app#34 depends on Design PR ArunskiOrg/rag-sample#42; and related PRs without strict dependency order: ArunskiOrg/.github#12, ArunskiOrg/org-stardards#5` -->

## What changed
<!-- Describe the changes made. Focus on function and impact, not a line-by-line summary — the diff covers what changed. -->

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
- [ ] Project-specific deployment plan updated to reflect deployment changes, as in [rag-sample](https://github.com/ArunskiOrg/rag-sample/blob/main/project-management/deployment-plan.md)
- [ ] Acceptance criteria met by this specific PR
  - [ ] No additional scope beyond direct dependencies of those acceptance criteria
  - <list PR-relevant acceptance criteria (summarized)>

---

*PR template v1.6 — the canonical PR summary checklist, defined in [ArunskiOrg/.github](https://github.com/ArunskiOrg/.github/blob/main/.github/pull_request_template.md). The detailed rules behind each item are canonical in [`dev-standards.md`](https://github.com/ArunskiOrg/org-standards/blob/main/docs/standards/dev-standards.md) (ArunskiOrg/org-standards).*
