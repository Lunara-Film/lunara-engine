# Working agreement — Lunara Engine

Effective 2026-10-17, by Dalton's explicit instruction. This repository is a
standalone Streamlit recommendation application, separate from the WordPress
Theme and plugins. Its current hosting relationship is not established here.

## Dalton's confirmation — effective 2026-10-23

Dalton's confirmation of a website implementation task (for example "yes",
"go ahead", "do it" or "begin/create it") authorizes the requested work through
task-branch commits, PRs, passing checks, agent merge, manual deployment and
live verification. Do not ask for a second deployment confirmation or require
a new approval naming the final version. Reuse the confirmation in the current
conversation; instructions to hold, prepare only, leave a draft, or not deploy
take precedence. Ask only about a real missing decision, access, changed
destination or work beyond that confirmed scope.

Keep branch protections, required CI and exact-head PR merges. Manual
deployment means the agent uses the existing host action; it does not mean
Dalton must click it. Auto-deploy stays off unless he specifically changes it.
A confirmation never makes a merge evidence of deployment: verify and report
both states separately.

## Agent merge authority

Agents have standing permission to commit, push, open/update PRs and merge
completed, verified work within Dalton's approved task. Do not require Dalton
to click Merge or reconfirm a routine merge. An explicit instruction to hold a
particular PR takes precedence. Follow the shared
[Lunara merge policy](https://github.com/Lunara-Film/lunara-theme-blocks/blob/main/docs/AGENT-MERGE-POLICY.md).

- Branch from current `main`; never commit directly to main.
- Review the complete diff, identify the exact repository/base/PR/head SHA,
  and preserve unrelated drafts and unfinished work.
- Run relevant validation and any applicable CI for the final candidate.
  This repository has no CI workflow as of this agreement; disclose that fact
  and record local verification rather than claiming CI passed. Runtime changes
  need appropriate Python checks and a local application check. Documentation
  changes need a diff and link review, not a fabricated runtime test.
- Merge through the PR with an exact-head guard and a supported merge method.
  Do not bypass protections, weaken checks or force push. Read back the merged
  commit and verify any main checks. Do not merge branches back and forth just
  to change ahead/behind counts.
- Record the result in the shared Theme `docs/SESSION-LOG.md`; preserve history.

## Runtime and deployment boundary

Keep CSV data, provider configuration and credentials intact. This policy
follows Dalton's confirmed task scope through release. Establish the actual
host, deployment trigger and intended destination before publishing runtime
changes. His confirmation of that release is sufficient; do not demand a
second approval naming the final version. It does not authorize unrelated
WordPress changes or add this repository to the active WordPress release set.

When resuming an old branch, read the current default-branch agreement.
Historical notes do not override current merge authority. Feature/editorial
decisions and credentials remain separate from source-control permission.
