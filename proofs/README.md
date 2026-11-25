# Proofs — accordproject/template-archive PR #973

This branch is an orphan proof branch tied to
<https://github.com/accordproject/template-archive/pull/973>.

PR: `docs(cicero-core): remove nonexistent parse() reference from class JSDoc (#881)`
Author: `@Aditya060806`
Base: `accordproject/template-archive:main`
Head: `Aditya060806/template-archive:docs/issue-881-remove-nonexistent-parse-jsdoc`
Head commit: `92d8eb3c8320d7432b1857c7b5228984fcd593f7`
State at publish: `OPEN`, `isDraft=true`, `mergeable=MERGEABLE`.

## What's in here

| File | What it shows |
| --- | --- |
| [`01-issue-881.json`](./01-issue-881.json) | Full JSON of the originating issue (title, body, labels, author, state) — the source of truth for Option 2. |
| [`01-issue-881.txt`](./01-issue-881.txt) | `gh issue view 881 --comments` output showing the reporter's soft-claim and the Stale-bot note. |
| [`02-pr-973-diff.patch`](./02-pr-973-diff.patch) | `gh pr diff` output — the exact three-file JSDoc change on the PR. |
| [`03-pr-973-view.txt`](./03-pr-973-view.txt) | `gh pr view` output showing title, DRAFT state, body, +4/-7, auto-merge disabled. |
| [`04-pr-973-state.json`](./04-pr-973-state.json) | `gh pr view --json state,isDraft,mergeable,…` — the merge-gate snapshot. |
| [`05-commit-message.txt`](./05-commit-message.txt) | Full commit message of `92d8eb3c` including the DCO sign-off and `Ran-and-results` trailer. |
| [`06-diffstat.txt`](./06-diffstat.txt) | `git diff upstream/main...HEAD --stat` — three files, +4/-7 confirms scope. |
| [`07-local-verification.md`](./07-local-verification.md) | Loop-captured lint + license + build + test results for `packages/cicero-core`. |

## How to re-verify

```sh
# Merge gate
gh pr view https://github.com/accordproject/template-archive/pull/973 \
  --repo accordproject/template-archive \
  --json state,isDraft,mergeable

# Scope
gh pr diff https://github.com/accordproject/template-archive/pull/973 \
  --repo accordproject/template-archive

# Local tests (from the repo root, after checking out the head commit)
cd packages/cicero-core && npm ci && npm test
```
