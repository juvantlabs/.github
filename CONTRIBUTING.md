# Contributing to juvantlabs

Thanks for considering a contribution. `juvantlabs` ships open-source frameworks
and tooling under MIT — we welcome PRs, issues, and discussion across all
`juvantlabs/*` repos.

This file describes the **default** contribution flow. Individual repos may add
a `CONTRIBUTING.md` of their own with repo-specific guidance; that file always
wins over this one.

## Where to start

- **Bug reports / feature requests**: open an issue in the relevant repo using
  the templates in [.github/ISSUE_TEMPLATE/](./ISSUE_TEMPLATE/). Search existing
  issues first.
- **Small fixes** (typos, broken links, shellcheck/lint findings): open a PR
  directly. No issue needed.
- **Substantive changes** (new feature, architectural shift, breaking API): open
  an issue first to align on direction. Larger changes may motivate an ADR
  (see "Architectural changes" below).

## Pull request flow

1. **Fork** the repo (or branch within if you have write access).
2. **Branch naming**: `feat/<scope>`, `fix/<scope>`, `docs/<scope>`, `ci/<scope>`,
   `refactor/<scope>`, `test/<scope>`. Match the conventional-commit prefix.
3. **Conventional commits**: subject lines follow
   `<type>(<scope>): <subject>` — e.g. `fix(hooks): bash 3.2 SQL escape regression`,
   `feat(v0.6.4): wizard rendering rule clause 2`. Body explains the *why* in
   prose, not just the *what*.
4. **Sign off your commits** if the repo's CONTRIBUTING.md asks for it (most
   `juvantlabs/*` repos do not require DCO signoff yet, but check before
   pushing).
5. **CI**: every PR runs the repo's lint workflow. Fix failures locally before
   pushing again — green CI is a hard requirement for merge.
6. **Tests**: if the repo has tests (most do, under `tests/`), add coverage for
   new behavior. Bug fixes should include a regression test that fails without
   the fix.
7. **PR description**: use [the template](./PULL_REQUEST_TEMPLATE.md). Include
   summary + test plan + any breaking-change callouts.

## What "good" looks like

- **Small, focused PRs** are merged faster. If you're touching more than ~5
  files for a single fix, consider splitting.
- **Why-first commit messages**. Reviewers should understand the motivation
  in 30 seconds.
- **No unsolicited refactors**. If you spot adjacent ugliness, file a separate
  issue rather than expanding the PR scope.
- **Backwards compatibility** matters. Breaking changes need a `BREAKING:`
  trailer in the commit body and a `## Migration` section in the PR
  description.
- **Match the project's voice**. Terse, evidence-led, opinionated where
  warranted. We're an engineering org; prefer prose that explains tradeoffs
  to prose that hand-waves.

## Architectural changes

If your change touches:

- A framework invariant (`SYSTEM_INVARIANTS.md` in `juvant-os`)
- A wizard step that adopters depend on (`JUVANT_OS.md` in `juvant-os`)
- An MCP server's tool surface (any `juvantlabs/*-mcp-server`)
- Cross-cutting concerns (org-wide naming, license defaults)

… open an ADR proposal first. Two homes:

- **Framework ADRs** — for changes inside `juvant-os` itself, propose in
  [`juvant-os/docs/adr/`](https://github.com/juvantlabs/juvant-os/tree/main/docs/adr)
  as a successor or new ADR.
- **Org-level ADRs** — for changes about how `juvantlabs` operates (namespace,
  contribution flow, license defaults), propose in
  [`juvantlabs/handbook`](https://github.com/juvantlabs/handbook).

ADRs use the [Nygard form](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions):
Status / Context / Decision / Consequences / Implementation / References.

## License

By contributing you agree your contribution is licensed under the repo's
license — typically MIT (the `juvantlabs` default). If a repo specifies a
different license, that file wins. We do not require a CLA.

## Code of Conduct

Participation in `juvantlabs/*` projects is governed by the
[CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md). Report unacceptable behavior to
[dev@juvant.io](mailto:dev@juvant.io).

## Questions

- Email: [dev@juvant.io](mailto:dev@juvant.io)
- For private security disclosures: [security@juvant.io](mailto:security@juvant.io)
  — see [SECURITY.md](./SECURITY.md).
