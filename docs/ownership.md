# Ownership

## Canonical Project

- Name: Agent Work Review
- Outcome: provide a public, standalone, local-first review of agent-working
  history through the onlinesourdough Method.
- Canonical repository: [onlinesourdough/Agent-Work-Review](https://github.com/onlinesourdough/Agent-Work-Review)
- Method source of truth: [agent-work-review.md](../agent-work-review.md)
- Lifecycle owner: Gustav Anderson.
- Public identity: `onlinesourdough` is the method, brand, and repository
  namespace; it is not a separate company.

## Responsibilities

| Responsibility | Source of truth | Owner | Failure or escalation route |
| --- | --- | --- | --- |
| Review method and privacy boundary | [Runbook](../agent-work-review.md) | Gustav Anderson | Stop locally; open no sharing path |
| Repository contract | [Checker](../scripts/check_repository.py) | Gustav Anderson | Treat a failed check as blocking |
| Source history | The person's configured local harness store | Person running the review | Do not copy it into this repository |
| Local report | The person's chosen local workspace | Person running the review | Keep it local and disclose limitations |
| Any later sharing | Exact approved content and destination | Person running the review | No action without fresh explicit permission |

## Boundary

This repository owns the runbook, examples, validator, and Project records. It
does not own, collect, or transmit a user's history or report. A later website
may publish the canonical runbook unchanged; it does not gain ownership of the
method.

## Historical provenance

- Creation source: `https://github.com/onlinesourdough/Agentic-project-template.git@02cb0e4fc63203f1afb090df8632d20d5aedb9a3`
- This reference records the source used at creation. It is not a runtime
  dependency or a competing source of Project truth.
