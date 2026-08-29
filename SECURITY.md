# Security Policy

## Reporting a vulnerability

Do not disclose suspected vulnerabilities, credentials, private infrastructure
details, or exploit evidence in a public issue.

Use the affected repository's private vulnerability reporting or security
advisory interface when available. If it does not provide one, use the
[derMonaco Labs private security advisory form](https://github.com/dermonaco-labs/.github/security/advisories/new).

Include only the information needed to reproduce and assess the issue:

- affected repository and component;
- observed behavior and potential impact;
- safe reproduction steps;
- affected versions or commit identifiers;
- suggested mitigation, if known.

Never include or test active secret values. Report the credential type, scope,
and exposure location immediately. Organization maintainers are responsible for
revocation, rotation, containment, and log cleanup.

## Response priorities

- Active credential exposure or unauthorized access: contain immediately.
- Critical or high-impact vulnerability: assess before normal feature work.
- Lower-severity hardening issue: track with an owner and review date.

Security fixes must preserve existing validation evidence. Do not silence a
finding by deleting tests or broadly excluding files from scanning.
