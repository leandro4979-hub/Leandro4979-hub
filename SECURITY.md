# Security Policy

Security reports are taken seriously, especially where agent execution, authorization, privacy, local services, device control, credentials, or automation boundaries are involved.

## Do not disclose sensitive vulnerabilities publicly

Do **not** include exploit details, secrets, credentials, private keys, tokens, personal data, or sensitive system information in public issues, discussions, pull requests, or comments.

If GitHub's **private vulnerability reporting** option is available for this repository, use that channel.

If no private reporting channel is visible, open a minimal public issue titled:

```text
[Security Contact] Private reporting channel requested
```

Include no exploit details. Only state that you have a security concern and need a private reporting path.

## What to include privately

A useful report contains:

- affected repository, component, branch, and version or commit SHA;
- vulnerability class and realistic impact;
- minimum reproducible steps;
- required permissions or preconditions;
- whether exploitation crosses an authorization boundary;
- whether credentials, personal data, devices, or external systems are exposed;
- suggested mitigation if known.

## Scope priorities

Highest priority issues include:

- authorization bypasses;
- fail-open behavior around agent execution;
- command or tool injection;
- secret leakage;
- unsafe device or account control;
- path traversal or sandbox escape;
- privilege escalation;
- insecure local-network exposure;
- audit-log tampering or verification bypass;
- cross-user data exposure.

## Safe research expectations

Please avoid:

- accessing data that is not yours;
- changing or deleting third-party data;
- persistence beyond what is required to demonstrate the issue;
- denial-of-service activity;
- social engineering;
- publishing sensitive details before a fix can be evaluated.

## Security model

The intended control boundary is:

```text
INTENT
  ↓
EVIDENCE
  ↓
DECISION
  ↓
AUTHORIZATION
  ↓
EXECUTION
  ↓
OBSERVATION
  ↓
VERIFICATION
```

Any path that skips required authorization or produces a false verified state should be treated as a security defect.
