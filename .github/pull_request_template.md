## Problem

What problem does this change solve?

## Outcome

What should be observably better after this merges?

## Scope

What is intentionally included, and what is intentionally not included?

## Authority / boundaries

Does this change affect agent execution, devices, accounts, external systems, credentials, user data, or other consequential actions?

If yes, describe the authorization boundary and fail-closed behavior.

## Verification

List the exact checks actually run and their results.

- [ ] Tests
- [ ] Build / validation
- [ ] Manual or integration verification, if applicable
- [ ] Failure / recovery path checked, if applicable

Evidence:

```text
command / check:
result:
```

## Risk and rollback

What could break, and how can this change be reverted or disabled safely?

## Evidence classification

- [ ] Confirmed
- [ ] Historical
- [ ] Inferred
- [ ] Missing

## Final review

- [ ] No secrets, credentials, or personal data are included.
- [ ] Unrelated changes are excluded.
- [ ] Claims match the verification evidence.
- [ ] Human authorization remains explicit for consequential execution.
