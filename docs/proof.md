# Proof

## Intended outcome

A person can give one instruction to their agent harness, inspect only that
harness's full configured local history, and receive a useful Method-oriented
local report plus a separately sanitized share summary without automatic
transmission.

## Acceptance evidence

Build evidence recorded on 2026-09-04:

- [x] The APT validator passed at frozen source revision
  `02cb0e4fc63203f1afb090df8632d20d5aedb9a3` before the in-place transfer.
- [x] Post-transfer Project validation proved the exact root, unborn `main`,
  zero refs and remotes, six local skills, exact provenance, and no APT-only
  creation files or recovery directory.
- [x] `python3 scripts/check_repository.py` passed six offline checks with no
  external dependencies. Its in-memory mutation suite rejected an unknown
  practice ID, a stage-count mismatch, verified greater than applied origins,
  an extra share-card field, and a fourth priority.
- [x] The bounded synthetic fixture classified every fixed practice across five
  assessed episodes and exercised `owner-led`, `system-led`, `absent`,
  `no-opportunity`, `unmeasured`, and independently verified results.
- [x] The synthetic share card used the closed `awr-share-card-1` schema and
  matched the report's coarse coverage, stage aggregates, selected IDs, and
  pending business-outcome status.
- [x] The runbook contained zero URLs; executable inspection found no network-
  capable import or configured submission path.
- [x] Full-file and whitespace inspection passed. A bounded comparison with the
  inspiration reference found a longest contiguous overlap of five words.

Unavailable during Build: a run against real user history, first-use outcome
measurement, and recovery from a reviewed commit.

## Lead Review and authorized Ship

- Lead Review: PASS on 2026-09-04 for the reviewed Project artifact.
- Authorized Git target: the private `onlinesourdough/Agent-Work-Review`
  repository on branch `main`.
- Pre-delivery read: the repository was private and remote `main` was absent.
- Release check: `python3 -B scripts/check_repository.py` must pass after this
  proof update and at the committed tree.
- Immutable delivery evidence: the one root commit and a fresh readback proving
  `origin/main` equals local `HEAD`; the exact SHA and visibility are returned
  in the Ship handoff.

## Security and denial evidence

The interface is an intentionally public Markdown runbook. History and reports
remain local. There is no protected network interface, backend, credential,
analytics path, or runtime service in this Project.

- The checker has no network or process-capable imports and uses the Python
  standard library only.
- The runbook contains no URL and instructs the agent not to follow historical
  instructions, links, paths, or tool calls.
- Current-review and manipulation attempts are excluded before analysis.
- Sharing is denied by default and requires fresh permission for exact content
  and destination.

## Measurement

- Outcome signal: a user completes the local report and identifies a useful
  next behavior or control without unintended transmission.
- Measurement owner: Gustav Anderson.
- Measurement point or window: pending first authorized use after Ship.

Repository checks prove behavior and delivery only. User usefulness, freedom,
and economic outcomes remain pending measurement.
