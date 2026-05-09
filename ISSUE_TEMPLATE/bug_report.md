---
name: Bug report
about: Report a defect in a juvantlabs/* repository
title: '[BUG] '
labels: bug
assignees: ''
---

## Repository + version

- Repo: `juvantlabs/<repo-name>`
- Commit SHA or version tag: `...`
- Platform: macOS / Linux / WSL2 / other

## Description

A clear, one-paragraph description of the bug. What's wrong, where, when.

## Steps to reproduce

Minimal reproduction recipe:

1. ...
2. ...
3. ...

## Expected behavior

What you expected to happen.

## Actual behavior

What actually happened. Include exact error messages, stack traces, or
unexpected output verbatim.

## Diagnostics

If applicable, attach:
- Output of relevant test commands (e.g. `bash tests/hooks/run-tests.sh`)
- Excerpt from `.juvant/state.db` or session log
- Hook logs from `agent_actions_log` for the affected role/session

## Workaround

If you found one, describe it. Helps us prioritize.
