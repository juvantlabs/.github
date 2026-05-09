# .github — juvantlabs

Org-wide community health files for the [`juvantlabs`](https://github.com/juvantlabs)
GitHub organization (the open-source arm of [Juvant Srls](https://juvant.io)).

Files in this repository apply automatically to all `juvantlabs/*` repositories
that do not provide their own version. Per-repo files always win; this repo is
the **default** when a repo doesn't specify.

## Contents

| File | Purpose |
|---|---|
| `profile/README.md` | Org profile shown at [github.com/juvantlabs](https://github.com/juvantlabs) |
| `CONTRIBUTING.md` | How to contribute to any `juvantlabs/*` repo |
| `CODE_OF_CONDUCT.md` | Community standards (Contributor Covenant 2.1) |
| `SECURITY.md` | Coordinated vulnerability disclosure for OSS repos |
| `ISSUE_TEMPLATE/` | Bug report + feature request templates |
| `PULL_REQUEST_TEMPLATE.md` | PR template with signoff + conventional commits |

## Org-level governance

Architectural decisions about how `juvantlabs` operates as an organization
(naming conventions, namespace structure, repo-type specs, license defaults)
live in a separate repo: [`juvantlabs/handbook`](https://github.com/juvantlabs/handbook).

This `.github` repo is for community-health automation; the `handbook` is for
durable governance decisions in [Nygard ADR form](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions).
The two complement each other.

## License

Files in this repo are MIT-licensed (the juvantlabs default for OSS).
