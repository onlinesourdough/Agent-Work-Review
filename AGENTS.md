# Agent Work Review

Build and operate the smallest independent Project that creates this outcome:

> Create a public, standalone, local-first review that lets people inspect recorded agent-working history and receive a practical onlinesourdough Method-oriented report without automatically transmitting history or results.

## Start

Read this file and [README.md](README.md) for the repository's independent
lifecycle and product boundary. Read the canonical [review runbook](agent-work-review.md)
when running a history review or changing its method, privacy, evidence, or
report contracts. Contributor maintenance does not authorize history access.
Use project-local Spec when scope, ownership, boundaries, proof, or contracts
are materially unclear; reuse accepted inputs for an already bounded change.
Handle mechanical local edits directly with the relevant validator and review.

Ask one question only when a missing owner decision materially changes the
Project. Keep resolved context intact and record technical inferences locally.

## Route

| Work | Skill |
| --- | --- |
| Technical scope, boundaries, proof, or contracts | `.agents/skills/spec-project/SKILL.md` |
| New or materially changed technology decision | `.agents/skills/choose-technology/SKILL.md` |
| Implementation | `.agents/skills/build-project/SKILL.md` |
| Correctness, security, simplicity, and proof review | `.agents/skills/review-project/SKILL.md` |
| Authorized delivery, deployment, activation, or recovery | `.agents/skills/ship-project/SKILL.md` |
| Periodic whole-repository health check | `.agents/skills/audit-project/SKILL.md` |

Use the [local skill index](.agents/skills/README.md) when adding or relocating
skills or resolving a specialist capability gap.

Keep one lifecycle record across Spec, Build, Review, revisions, and any
authorized Ship. The Project repository is canonical after creation.

## Before completion

Verify behavior through the real interface or validator. Run
`python3 scripts/check_repository.py` plus the relevant format, lint, contract,
and security checks. Check failure, denial, duplicate, and recovery behavior as
relevant. Keep the README and [proof record](docs/proof.md) current with actual
evidence.

## Ownership and recovery

Record current responsibility in [docs/ownership.md](docs/ownership.md),
acceptance evidence in [docs/proof.md](docs/proof.md), and the tested recovery
path in [docs/recovery.md](docs/recovery.md). Keep secrets and private data out
of source, logs, exports, and client builds.
