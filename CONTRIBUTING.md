# Contributing to Th1nkDev projects

Thanks for your interest in our work. Most Th1nkDev repositories are private client or product code; this guide applies to every repository of the [th1nkdev-io](https://github.com/th1nkdev-io) organisation unless the repository has its own `CONTRIBUTING.md`.

> 🇫🇷 Une version courte en français se trouve [en bas de cette page](#-en-français).

## Before you start

- **Security issues** never go in a public issue. Follow [SECURITY.md](SECURITY.md).
- **Questions and help** — see [SUPPORT.md](SUPPORT.md).
- **Bigger changes** — open an issue first so we can agree on the approach before you write code.
- Everyone taking part follows our [Code of Conduct](CODE_OF_CONDUCT.md).

## Workflow

1. Branch from the repository's default branch (often `dev`). Use a short, descriptive name: `feat/qr-ordering`, `fix/pdf-pagination`.
2. Keep each pull request focused on one subject. Several small PRs beat one large one.
3. Write commits in the [Conventional Commits](https://www.conventionalcommits.org) style, one subject per commit:
   `feat(orders): real-time status on the floor plan`
4. Open a pull request using the template, describe **what** changed and **why**, and link the issue.
5. A maintainer reviews it. CI must be green before merge.

## Quality bar

These are the same standards we hold our own engineering to:

- **Typed code** — TypeScript in strict mode where the project uses it; no `any` without a reason.
- **Tests** — new behaviour comes with tests; fixed bugs come with a test that would have caught them.
- **Lint and format** — run the project's lint and format scripts before pushing.
- **Internationalisation** — user-facing text goes through the i18n files, in every supported language.
- **Accessibility** — interfaces stay keyboard-usable and meet WCAG AA contrast.
- **No secrets** — never commit `.env` files, keys, tokens or real customer data. Use the example config files.
- **Documentation** — update the README or docs when behaviour or setup changes.

## Supply-chain hygiene

- Do not add a dependency without a clear need; prefer well-maintained packages and pin versions through the lockfile.
- Never commit generated bundles, minified code or binaries that are not part of the source.
- Configuration files (`*.config.*`, `.vscode/tasks.json`, Git hooks) are reviewed with extra care: any obfuscated or unexpected code in them will be rejected.

## Licence

Unless a repository states otherwise, contributions are made to Th1nkDev or to the client that owns the repository, under the terms of the agreement that governs that work.

---

## 🇫🇷 En français

- Les failles de sécurité ne se signalent jamais dans un ticket public : voir [SECURITY.md](SECURITY.md).
- Pour un changement important, ouvrez d'abord un ticket pour convenir de l'approche.
- Une branche par sujet depuis la branche par défaut, des commits au format Conventional Commits, une PR ciblée qui explique le quoi et le pourquoi.
- Code typé, tests, lint, textes passés par l'i18n dans toutes les langues, accessibilité, aucun secret ni donnée réelle commités.
- Les fichiers de configuration, tâches d'éditeur et hooks Git sont relus avec une attention particulière : tout code obscurci ou inattendu est refusé.
