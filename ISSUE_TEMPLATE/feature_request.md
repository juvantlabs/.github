---
name: Feature request
about: Propose a new capability for a juvantlabs/* repository
title: '[FEAT] '
labels: enhancement
assignees: ''
---

## Repository

`juvantlabs/<repo-name>`

## Problem statement

What's the use case? Who's the user? What can they not do today that they
should be able to do?

Don't propose a solution yet — describe the problem in user terms first.

## Proposed solution

Now describe the change you have in mind. Include:

- API surface (if applicable): new flags, new endpoints, new wizard steps
- Behavior: what changes from the user's perspective
- Backwards compatibility: does this break existing adopters? If yes, what's
  the migration path?

## Alternatives considered

What else did you think about? Why is this the better path?

## Architectural impact

Does this require an ADR?

- For framework-internal changes (touch `JUVANT_OS.md`, `SYSTEM_INVARIANTS.md`,
  any agent definition, the schema, or the matrix): yes — propose in
  [`juvant-os/docs/adr/`](https://github.com/juvantlabs/juvant-os/tree/main/docs/adr).
- For org-level changes (naming, license defaults, contribution flow): yes —
  propose in [`juvantlabs/handbook`](https://github.com/juvantlabs/handbook).
- Pure implementation detail with no architectural impact: skip the ADR.

## Effort estimate

Your guess at lines-of-code / time. Helps us scope.
