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

Unavailable during Build: a run against real user history and first-use outcome
measurement. Recovery from a reviewed commit was exercised after publication,
as recorded below.

## Lead Review

- Project Review and publish-safety Review both passed on 2026-09-04 for exact
  commit `554b93e59ef69ef97bc5113b9298ce1c5614411e`.
- Post-Ship Review found that this proof record and the recovery record still
  described pre-publication state. This two-document correction responds to
  that finding and passed lead re-review on 2026-09-04.

## Delivery

Delivery status: **PASS**.

- The initial public commit is
  `554b93e59ef69ef97bc5113b9298ce1c5614411e` on `main` in the public
  `onlinesourdough/Agent-Work-Review` repository.
- Fresh reads after publication proved that local `HEAD`, fetched
  `origin/main`, and live remote `main` all resolved to that commit. GitHub
  reported visibility `PUBLIC` and default branch `main`.
- Anonymous HTTP reads without authentication headers or tokens succeeded for
  the repository page, rendered README, and raw `agent-work-review.md`.
- The anonymous raw runbook began with `# Agent Work Review runbook`, contained
  zero configured URLs, and had SHA-256
  `7d68b205c1b2c9dbc0044394ee98c7d4f7545ad3089c0aff6b61f398f5b628e9`.
- `python3 -B scripts/check_repository.py` passed after publication: six
  checks, five rejected share-card mutations, offline, with no external
  dependencies.

## Stable distribution follow-up

This Build follow-up starts from public repository commit
`8974be45d757167eb77f60cbf45f970a8dd96585`; it does not rewrite the initial
publication evidence above.

- Website release `gustavonline/onlinesourdough@e0a45377b3ebb42ee05df5300caf9a6a13c1aea5`
  publishes the repository-owned runbook at
  `https://onlinesourdough.com/agent-work-review.md`.
- A live anonymous GET on 2026-09-04 returned HTTP 200 with media type
  `text/markdown; charset=utf-8` and exactly 18,952 bytes. The response was
  byte-for-byte identical to the unchanged local `agent-work-review.md` and had
  SHA-256
  `7d68b205c1b2c9dbc0044394ee98c7d4f7545ad3089c0aff6b61f398f5b628e9`.
- The public human entry point at
  `https://onlinesourdough.com/agent-work-review/` returned HTTP 200 with media
  type `text/html; charset=utf-8`.
- The website owns these distribution and entry points. This repository
  remains the method owner and source of truth.

## Recovery

Recovery status: **PASS** for the static repository rebuild path.

- A fresh temporary directory was created on 2026-09-04 and the public HTTPS
  repository was cloned with Git credential helpers disabled.
- The clean clone checked out
  `554b93e59ef69ef97bc5113b9298ce1c5614411e` and its offline repository checker
  passed with the same six checks and five rejected mutations.
- The validated temporary directory was removed after the rehearsal.
- Repository recovery is a reviewed follow-up commit that restores correct
  content, or a reproducible rebuild from a known reviewed commit. Making a
  public repository private cannot reverse prior disclosure and is not claimed
  as recovery.

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

## Outcome

Outcome status: **PENDING**.

- Outcome signal: a user completes the local report and identifies a useful
  next behavior or control without unintended transmission.
- Measurement owner: Gustav Anderson.
- Measurement point or window: pending the first real authorized use.

Repository checks prove behavior and delivery only. User usefulness, freedom,
and economic outcomes remain pending measurement.
