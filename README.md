# .github

Default community health files for every repository owned by
[AnotherMike-exe](https://github.com/AnotherMike-exe).

GitHub uses a file from this repo when a repository has no file of its own
with the same name. Resolution order: the repo's `.github/`, then its root,
then its `docs/`, then this repo.

| File | Purpose |
|---|---|
| `CONTRIBUTING.md` | How to propose changes |
| `CODE_OF_CONDUCT.md` | Expected behavior |
| `SECURITY.md` | How to report a vulnerability privately |
| `SUPPORT.md` | Where to ask questions |
| `ISSUE_TEMPLATE/` | Bug and feature forms; routes questions to Discussions |
| `PULL_REQUEST_TEMPLATE.md` | PR checklist |
| `FUNDING.yml` | Sponsor button |

To override a file for one project, add a file with the same name to that
project. Issue templates override as a set: a project with its own
`.github/ISSUE_TEMPLATE/` ignores this folder entirely.

This repo must stay **public**, or GitHub ignores it.
