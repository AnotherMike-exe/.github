# Contributing

Thanks for helping. These projects are maintained by one person, so small,
focused changes get reviewed fastest.

## Before you start

- **Questions** go to the project's Discussions, not issues. See [SUPPORT.md](SUPPORT.md).
- **Bugs and features** — search open issues first, then use the issue form.
- **Large changes** — open an issue or discussion before writing code, so we
  can agree on the approach.
- **Security problems** — do not open a public issue. See [SECURITY.md](SECURITY.md).

## Making a change

1. Fork the repo and create a branch from `main`.
2. Keep one logical change per pull request.
3. Follow the project's existing style. If the project has a `CLAUDE.md`,
   `ARCHITECTURE.md`, or `docs/`, read them first.
4. Update documentation when behavior changes.
5. Run the project's tests and linters before you push.
6. Open a pull request and fill in the template.

## History

`main` uses a linear history. Rebase on `main` instead of merging it into
your branch:

```bash
git fetch origin
git rebase origin/main
```

## Naming

PascalCase is the default for directories, documentation files, repository
names, container names, and classes or types. Where a language or tool has a
binding convention, that convention wins — for example `snake_case` for
Python modules and functions and for ESPHome/YAML keys, and `camelCase` for
JavaScript/TypeScript functions and variables. Constants use
`UPPER_SNAKE_CASE`.

## License

By contributing, you agree that your contribution is licensed under the
project's license (see its `LICENSE` file).
