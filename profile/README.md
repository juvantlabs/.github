<div align="center">

<img src="https://juvant.io/assets/images/juvant-logo-transparent.png" alt="Juvant" width="240" />

<br/>
<br/>

### Open-source from [Juvant](https://juvant.io).

<br/>

[![Website](https://img.shields.io/badge/juvant.io-080B14?style=flat-square&logo=globe&logoColor=A855F7)](https://juvant.io)
[![Email](https://img.shields.io/badge/dev@juvant.io-080B14?style=flat-square&logo=mail.ru&logoColor=22D3EE)](mailto:dev@juvant.io)
[![X](https://img.shields.io/badge/@juvant__io-080B14?style=flat-square&logo=x&logoColor=white)](https://x.com/juvant_io)
[![License](https://img.shields.io/badge/MIT-080B14?style=flat-square)](https://opensource.org/licenses/MIT)

</div>

---

## What `juvantlabs` ships

`juvantlabs` is the open-source arm of [Juvant Srls](https://juvant.io). We
publish the frameworks, MCP servers, and tooling we use internally — released
under MIT so other companies can run their own Claude-powered agent stacks.

### Frameworks

- **[juvant-os](https://github.com/juvantlabs/juvant-os)** — Skill-first
  multi-agent operating system on Claude Code. Open `claude` in a folder, say
  *"Initialize Juvant OS for &lt;your-company&gt;"*, the Skill orchestrates
  the company. No CLI, no daemon, no installation.

### MCP servers

- **[m365-graph-mcp-server](https://github.com/juvantlabs/m365-graph-mcp-server)** —
  Microsoft Graph MCP server. OneDrive, SharePoint, and Calendar surfaces with
  read+write OAuth flow. Drop-in for `juvant-os`'s `ms-graph` abstract role.
- **[aruba-fattura-mcp-server](https://github.com/juvantlabs/aruba-fattura-mcp-server)** —
  Aruba Fatturazione Elettronica REST API v2 wrapper. Italian SDI e-invoicing
  surface for the `fattura_elettronica` abstract role in `juvant-os`.

### Tools and libraries

- **[engram](https://github.com/juvantlabs/engram)** — Python-native browser
  automation with cached LLM-resolved selectors. Use it when an MCP server
  doesn't exist yet and you need an agent to drive a web UI deterministically.
- **[juvant-tools](https://github.com/juvantlabs/juvant-tools)** —
  OSS-shareable utility scripts, dev tools, and CLI helpers extracted from
  internal use.

### Governance

- **[handbook](https://github.com/juvantlabs/handbook)** — org-level
  architectural decision records (ADRs) describing how `juvantlabs` operates:
  naming conventions, namespace structure, repo-type specs, contribution
  policy, license defaults.
- **[.github](https://github.com/juvantlabs/.github)** — this repo. Org-wide
  community health files (CONTRIBUTING, CODE_OF_CONDUCT, SECURITY, issue/PR
  templates) that apply by default to every `juvantlabs/*` repo.

### Operating model

We work in the open. Two distinct GitHub orgs:

- **`juvantlabs`** (here) — public, MIT-licensed OSS framework + tooling.
- **`juvantio`** — private, the Juvant Srls company instance running on top
  of `juvant-os`. Not contributable; serves as the canonical dogfood adopter.

Architectural decisions about the framework live in
[`juvant-os/docs/adr/`](https://github.com/juvantlabs/juvant-os/tree/main/docs/adr).
Architectural decisions about the **organization itself** (how we contribute,
how we license, how we name things) live in
[`handbook`](https://github.com/juvantlabs/handbook).

---

## Contributing

We welcome contributions to all `juvantlabs/*` repos. Start here:

- [CONTRIBUTING.md](./CONTRIBUTING.md) — PR flow, signoff, conventional commits,
  what we look for in a good change.
- [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md) — Contributor Covenant 2.1; the
  baseline for community interaction.
- [SECURITY.md](./SECURITY.md) — coordinated vulnerability disclosure for
  OSS repos.

For the framework-architectural questions (*"why is `JUVANT_OS.md` the
single Skill orchestrator?"*, *"why does subagent registration go through
`.claude/agents/` symlinks?"*), the answer is in `juvant-os/docs/adr/`.
For org-governance questions (*"why is this repo in juvantlabs and not
juvantio?"*, *"what's the naming convention for an MCP server repo?"*),
the answer is in [handbook](https://github.com/juvantlabs/handbook).

---

## Contact

- Email: [dev@juvant.io](mailto:dev@juvant.io)
- Security: [security@juvant.io](mailto:security@juvant.io)
- Website: [juvant.io](https://juvant.io)
- Location: Milan, Italy
