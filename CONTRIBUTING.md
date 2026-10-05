# Contributing

Thanks for helping turn ideas into bounded, testable, trustworthy work.

This repository is the public coordination surface for **Trusted Transformation Infrastructure**: systems where authority is explicit, execution is bounded, and outcomes can be inspected.

## Choose the right entry point

Use **Signal an idea** when you have a problem, observation, hypothesis, or direction that still needs evidence.

Use **Build together** when you already have a real use case, a contribution you can make, clear authority and boundaries, and success criteria for a pilot.

Use **Record a proof** after a bounded test or pilot has actually been run and there is evidence worth preserving.

## Working model

```text
IDEA
  ↓
EVIDENCE
  ↓
DECISION
  ↓
AUTHORIZATION
  ↓
BOUNDED EXECUTION
  ↓
VERIFICATION
  ↓
PROOF RECORD
```

GitHub issues and pull requests are coordination and evidence surfaces. They are **not authorization to operate devices, accounts, infrastructure, or external systems**.

## Contribution standards

A strong contribution should:

- solve a clearly stated problem;
- minimize scope while preserving a meaningful outcome;
- identify who has authority over consequential actions;
- preserve human control where actions are sensitive or irreversible;
- define observable success criteria;
- avoid collecting or exposing unnecessary personal or sensitive data;
- include recovery or rollback behavior where failure is plausible;
- distinguish verified facts from assumptions.

## Pull requests

Keep pull requests focused and reviewable.

Before opening a PR:

1. explain the problem and intended outcome;
2. describe the smallest safe change;
3. include verification evidence appropriate to the change;
4. call out security, privacy, compatibility, migration, or rollback implications;
5. avoid unrelated cleanup.

A PR should never claim tests, builds, deployments, or device behavior succeeded unless the relevant verification was actually run.

## Security and privacy

Never post credentials, API keys, tokens, private keys, personal data, or sensitive vulnerability details in a public issue or pull request.

See [SECURITY.md](SECURITY.md) for vulnerability reporting guidance.

## Agent and automation contributions

Automation must fail closed around consequential execution.

The expected boundary is:

```text
intent → evidence → decision → authorization → execution → observation → verification
```

No issue, comment, webhook, label, model output, or automated classification should by itself authorize execution.

## Evidence quality

When reporting results, classify evidence clearly:

- **confirmed** — directly observed and reproducible;
- **historical** — previously verified, but not rechecked now;
- **inferred** — supported by reasoning but not directly observed;
- **missing** — required evidence is not yet available.

Prefer durable evidence: test output, reproducible steps, commit SHAs, screenshots where appropriate, logs with secrets removed, or measured before/after results.

## Conduct

Be specific, constructive, and respectful. Challenge assumptions and systems, not people.

The goal is not maximum activity. The goal is **useful proof**.
