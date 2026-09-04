# Recovery

## Recovery owner

Gustav Anderson owns restoration of the public method. The person running a
review always owns the immediate privacy stop: end the review and decline any
sharing action. `onlinesourdough` is the method, brand, and repository namespace,
not a separate company or recovery owner.

## Current path

This Build has no deployment, backend, scheduled process, or remote. Recovery
is therefore local and document-based:

1. Stop the executing agent before any sharing action.
2. Preserve the user's session store unchanged.
3. Discard an unsafe generated report from the user's chosen workspace only
   with the user's explicit deletion authority.
4. Restore Project files from the last reviewed commit after Ship, or from the
   lead-reviewed Build handoff before the first commit.
5. Run `python3 scripts/check_repository.py` and repeat the bounded synthetic
   simulation before returning the runbook to use.

## Rehearsal

- Privacy kill switch: specified as stopping locally before transmission.
- Repository rebuild: deterministic from reviewed source plus the standard-
  library checker.
- Last recovery rehearsal: pending lead Review and first authorized Ship.
- Remaining risk: a third-party harness may ignore instructions; users should
  review its filesystem and network permissions before running the method.
