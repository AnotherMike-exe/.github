# .github

Default community health files for every repository owned by
[AnotherMike-exe](https://github.com/AnotherMike-exe).

GitHub uses a file from this repo when a repository has no file of its own
with the same name. Resolution order: the repository's own `.github/` folder,
then its root, then its `docs/` folder, then this repo.

| File | Purpose |
|---|---|
| `CONTRIBUTING.md` | How to propose changes |
| `CODE_OF_CONDUCT.md` | Expected behavior |
| `SECURITY.md` | How to report a vulnerability privately |
| `SUPPORT.md` | Where to ask questions |
| `.github/ISSUE_TEMPLATE/` | Bug and feature forms, and the chooser that routes questions to Discussions |
| `PULL_REQUEST_TEMPLATE.md` | PR checklist |
| `.github/FUNDING.yml` | Sponsor button |

## Where each file has to sit

Two of these have a fixed location, and GitHub silently ignores them anywhere else:

- GitHub reads issue forms and their `config.yml` **only** from
  `.github/ISSUE_TEMPLATE/`. It skips a top-level `ISSUE_TEMPLATE/` folder, and the
  chooser then shows nothing.
- GitHub reads `FUNDING.yml` **only** from `.github/`. At the root it gives no sponsor
  button.

GitHub finds the rest — `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `SECURITY.md`,
`SUPPORT.md`, `PULL_REQUEST_TEMPLATE.md` — in the root, in `.github/`, or in `docs/`.
They stay at the root here, where a visitor sees them.

To override a file for one project, add a file with the same name to that
project. Issue templates override as a set: a project with its own
`.github/ISSUE_TEMPLATE/` ignores this folder entirely.

This repo must stay **public**, or GitHub ignores it. A license cannot be defaulted
from here — every project needs its own `LICENSE` file.
