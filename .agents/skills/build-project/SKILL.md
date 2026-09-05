---
name: build-project
description: Implement and verify a project change whose outcome, ownership, boundaries, and acceptance are clear. Use for source, validator, runbook, or runtime implementation.
---

# Project Build

Build the smallest complete artifact or behavior that can be verified through
its real interface, validator, plan, health check, or rehearsal.

If the intended behavior, boundary, or independent lifecycle is still
consequentially unclear, use `spec-project` first.

Work inside the existing lifecycle goal. Use the harness's matching persistent
goal/task state or explicit outcome contract. For an AIOS-originated worker,
keep its one bounded goal active across Build, Review feedback, permitted
revisions, and requested authorized Ship. Never open or complete a goal merely
because the lifecycle phase changed.

## Use the resolved shape

Consume the Spec's resolved technology decision. A working stack goes directly
to Build when the change does not materially alter it. For a new or materially
changed decision, use the result from
[choose-technology](../choose-technology/SKILL.md); do not reopen selection.

This Project owns a static runbook, synthetic examples, and an offline Python
validator. Preserve that shape unless the accepted contract changes it. Do not
scaffold a runtime or add dependencies for document-only work.

## Keep documentation current

Documentation is part of every implementation result. Identify the README,
runbooks, instructions, skills, contracts, commands, configuration, operation,
recovery, and proof affected by the change. Update the canonical local source
in the same result when its truth changes; do not defer it to `audit-project`.
Verify local links and skill routes, and verify documented commands,
configuration, and interfaces against the repository and the checks that prove
them. Leave unaffected documentation alone.

## Work through complete results

Name the behavior and evidence for each complete result. Reproduce a defect
before fixing it and retain a regression check when it protects meaningful
behavior. Use the existing validator for mechanical document changes; do not
manufacture failing wording tests. For method or validator changes, exercise
bounded synthetic episodes and the applicable counting, privacy, denial,
duplicate, and recovery contracts. Never access real history merely to test a
contributor change.

Run the narrow check and `python3 scripts/check_repository.py`, plus other
checks required by the affected boundary. Exercise the real interface when
mocks cannot prove the result; label static or synthetic evidence as such.

Continue through the required results until the whole requested outcome is
implemented and verified. Review each risky result at the useful checkpoint and
run the final repository-wide review. When an authorized implementation review
fails, fix the finding and repeat the affected checks instead of returning
routine repair work to the user.

## Implement the proportional security contract

Implement only the protection resolved by Spec. Public and local-only Projects
do not gain authentication by default. For a protected boundary, prefer
maintained framework, identity-provider, or protocol primitives over custom
authentication or cryptography, and enforce authorization on the trusted
server or worker per action and resource.

- Fail closed in production when required security configuration is missing or
  invalid; startup or deployment validation must not silently disable the
  protection.
- Keep credentials, signing material, tokens, and session data out of source,
  client builds, logs, and unsafe exports.
- Validate external input and bound payload size, resource use, reads, retries,
  concurrency, and cost according to the interface's abuse risk.
- Make security-relevant failures visible through redacted, safe telemetry
  without disclosing credentials or unnecessary private data.
- If JWT was selected, use a maintained library and the Spec's configured
  algorithms, issuer, audience, time claims, key rotation, expiry, revocation,
  and replay controls. Do not create an ad-hoc token format.

Prove the relevant real boundary with a permitted request plus missing,
invalid, expired or replayed, and authenticated-but-forbidden cases as
applicable. Include a production-misconfiguration case when protection depends
on runtime configuration. Run relevant dependency, configuration, and static
checks that the selected stack supports.
Do not invent a universal scanner command.

If the contract introduces side effects, make retries idempotent and define
failure visibility and tested recovery. This does not authorize telemetry or
transmission of local history or reports.

Finish Build with a working repository, updated local truth, and exact evidence
for both behavior and affected documentation. Do not stop because one result
passed if more work remains. Keep the lifecycle goal active or paused for
Review; complete it only after the full requested outcome, including
authorized Ship when requested, has passed.
