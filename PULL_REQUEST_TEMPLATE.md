<!--
PR title: follow conventional commits — <type>(<scope>): <subject>
Examples:
  fix(hooks): bash 3.2 SQL escape regression
  feat(v0.6.5): wizard rendering rule clause 2
  docs(adr): ADR 0010 — compiled agent registration
-->

## Summary

One paragraph: what changes and *why*. Reviewers should grasp the motivation
in 30 seconds.

## Changes

- File or area touched — what changed
- File or area touched — what changed
- ...

## Test plan

- [ ] Local lint / type check / format passes
- [ ] Tests added / updated (if applicable); paste output of relevant runs:
- [ ] CI green on push

## Breaking changes

If any: list them, plus the migration path for adopters.
If none: write *"none"*.

## Architectural impact

Does this PR touch a framework invariant, wizard step, MCP tool surface,
or org-level convention?

- [ ] No — this is implementation detail with no architectural reach
- [ ] Yes — linked ADR: ___

## Notes for the reviewer

Anything non-obvious worth flagging — design tradeoffs you considered,
follow-up work intentionally deferred, areas where you'd appreciate a
second pair of eyes.
