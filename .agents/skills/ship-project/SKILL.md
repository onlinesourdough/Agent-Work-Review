---
name: ship-project
description: Deliver reviewed project changes to an authorized target and verify delivery, recovery, and outcome separately. Use for publication, deployment, activation, or operational recovery; preparation alone grants no delivery authority.
---

# Project Ship

Ship only reviewed work. A green build is not a deployment result.

Resume the active lifecycle goal after Review PASS; do not create a Ship goal.
For AIOS-originated work, resume the same project-worker goal and return final
evidence to the AIOS lead.

## Establish the release unit

Identify:

- exact commit and immutable artifact
- target environment and deployment owner
- required checks and authority
- configuration and secret ownership
- external service plan, quota, license, and billing owner when material
- migration and compatibility order
- critical journey and failure signal
- rollback, replay, disable, restore, or reconciliation path
- operational owner
- outcome signal, measurement owner, and next measurement point
- recovery point and recovery time expectations when state or continuity makes
  them material

Ask before a production release, external publication, workflow activation,
destructive migration, or other consequential action unless the user already
gave specific authority.

## Git delivery gate

Apply this gate only when a Git branch and remote are part of the requested
Ship.

Local-only Projects and Projects without a remote do not need this Git gate.

1. Pin the reviewed exact commit, its tree, its reviewed base, and the target
   branch/upstream. Delivery authority for one target does not authorize any
   other branch, remote, tag, release, merge, setting, or deployment.
2. Re-attest the exact Git root, branch, upstream, and credential-free remote
   identity. Confirm that the working tree and index are clean and that the
   commit's diff against the reviewed base is the expected diff. Stop on an
   unexpected file, staged change, commit, worktree, branch, upstream, remote,
   or reviewer substitution.
3. Perform a fresh fetch of the exact upstream and resolve the fetched live
   branch object. Stop when the local commit is behind or diverged, when the
   remote moved from the reviewed expectation, or when access or authority is
   uncertain. An ahead commit may proceed only when it is the reviewed commit
   and the exact delivery authority covers the target.
4. Use a normal non-force push of only that reviewed commit to the authorized
   branch and only with exact authority. Do not auto-merge, rebase, or force to
   make delivery fit; return to Review when new integration work is required.
5. Fetch and read the live target again after delivery. Prove that
   local HEAD equals the fresh fetched live branch object and report both exact
   hashes. A successful push command without this live readback is not delivery
   proof.

## Keep delivery proportional

- Run the repository's real checks. Install from a lockfile only when the
  reviewed solution has dependencies and installation is authorized; this
  static Project's checker uses the Python standard library.
- Use CI to make required build, test, validation, and security evidence
  repeatable. Automate deployment only when authority, verification, and
  recovery are equally explicit.
- Give CI and runtime credentials least privilege.
- Keep secrets out of code, logs, artifacts, and untrusted change execution.
- Pin third-party workflow actions to reviewed immutable versions.
- Confirm that the selected external plans and quotas support the release, and
  assign usage or billing alerts when an overage can interrupt service or
  materially change cost.
- Add environments, artifacts, migrations, and automation only when the
  solution actually has them.

## Release and verify

1. Build the exact artifact from the reviewed commit.
2. Apply configuration and compatible state changes in the documented order.
3. Deploy or publish without activating when the platform allows separation.
4. Read the actual platform result.
5. Verify expected version, health, critical journey, interfaces, assets, logs,
   failure visibility, and recovery in the target environment.
6. Activate only after the gate passes.
7. Stop, disable, roll back, or recover when verification fails.

For this static Project, prove the published runbook matches the reviewed
canonical bytes and validate a rebuild from the reviewed recovery point. The
Resources Project owns distribution; source publication does not authorize
changing its deployment. Use [ownership](../../../docs/ownership.md) and
[recovery](../../../docs/recovery.md) for the current responsibilities and path.
If an accepted contract introduces a runtime, verify its real caller journey,
dependency failure, retry/reconciliation, failure visibility, and recovery as
applicable before activation.

A backup is recovery evidence only after its restore path has been tested.
Document retention and access ownership. Keep secrets out of repositories,
artifacts, and ordinary backups.

## Report three independent results

- **Delivery — PASS or FAIL:** the reviewed artifact was built and deployed,
  published, or applied correctly.
- **Recovery — PASS, FAIL, or NOT APPLICABLE:** rollback, restore, rebuild,
  replay, or reconciliation was verified for the solution's risk.
- **Outcome — PASS, FAIL, or PENDING:** the agreed business or operational
  signal was measured. Tests can prove behavior and delivery, not an outcome
  whose measurement window has not elapsed.

Do not call a solution production-ready when required recovery evidence is
missing. Report the commit, artifact, environment, platform result, smoke
evidence, all three statuses, and any remaining operational risk. Complete the
project goal only after its delivery, recovery, outcome obligations, and
handoff pass; the owning lead completes its goal after all final evidence.
