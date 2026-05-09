# Security Policy

## Reporting a vulnerability

If you discover a security issue in any `juvantlabs/*` repository, please
report it privately:

- **Email**: [security@juvant.io](mailto:security@juvant.io)
- **Subject prefix**: `[SEC] <repo-name>`
- **Acknowledgement SLA**: 72 hours
- **Public disclosure**: coordinated with the reporter after a fix is shipped
  (typically 90 days from acknowledgement, sooner if the fix is faster)

Do **not** open a public GitHub issue for security findings.

## Scope

In scope (current `juvantlabs/*` OSS repos):

- [`juvant-os`](https://github.com/juvantlabs/juvant-os) — multi-agent OS framework
- [`m365-graph-mcp-server`](https://github.com/juvantlabs/m365-graph-mcp-server) — MCP server
- Any other `juvantlabs/*` repo not explicitly listed Out of Scope below

Out of scope:

- Issues in third-party dependencies — report directly to the dependency
  maintainer (we'll happily file a downstream issue once the upstream
  releases a fix)
- Issues in derivative per-company instances (mirror-pushed from
  `juvantlabs/juvant-os` into private `juvantio/*` or third-party
  organizations) — report to the company that operates the instance
- Issues in Claude Code itself or other Anthropic products — report to
  Anthropic via their security disclosure process

## What to include in a report

- Repository + commit SHA where the issue reproduces
- Steps to reproduce, with minimal example
- Expected vs actual behavior
- Severity assessment (your read; we'll calibrate jointly)
- Disclosure timeline preferences

## Acknowledgement

We credit reporters in the fix's CHANGELOG entry and (when relevant) in a
SECURITY.md update unless the reporter prefers to remain anonymous.
