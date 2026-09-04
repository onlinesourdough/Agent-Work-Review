# Recovery

## Recovery owner

Gustav Anderson owns restoration of the public method. The person running a
review always owns the immediate privacy stop: end the review and decline any
sharing action. `onlinesourdough` is the method, brand, and repository namespace,
not a separate company or recovery owner.

## Current path

This Project is a public, static Git repository on `main`. It has no backend,
scheduled process, mutable service state, or automatic submission endpoint.
Recovery remains document-based:

1. Stop the executing agent before any sharing action.
2. Preserve the user's session store unchanged.
3. Discard an unsafe generated report from the user's chosen workspace only
   with the user's explicit deletion authority.
4. Correct a repository defect with a reviewed follow-up commit that restores
   the intended content without rewriting public history.
5. When a rebuild is needed, start from a known reviewed commit. The initial
   public recovery point is
   `554b93e59ef69ef97bc5113b9298ce1c5614411e`.
6. Run `python3 -B scripts/check_repository.py` and repeat the bounded synthetic
   simulation before returning the runbook to use.

Changing the repository to private cannot undo copies or observations made
while it was public. It is not represented as rollback or recovery from public
disclosure.

## Rehearsal

- Privacy kill switch: specified as stopping locally before transmission.
- Repository rebuild: **PASS** on 2026-09-04. A clean clone from the public
  credential-free HTTPS URL, with Git credential helpers disabled, resolved to
  `554b93e59ef69ef97bc5113b9298ce1c5614411e` and passed
  `python3 -B scripts/check_repository.py` with six checks and five rejected
  share-card mutations. The exact temporary directory was removed afterward.
- Outcome measurement: **PENDING** until the first real authorized use.
- Remaining risk: a third-party harness may ignore instructions; users should
  review its filesystem and network permissions before running the method.
