# Contributing

## Scope

The `dermonaco-labs` organization contains personal homelab infrastructure,
deployment configuration, applications, and operational documentation. Changes
should remain small, reviewable, reversible, and appropriate to the target
repository.

## Workflow

1. Create a focused branch from the repository's default branch.
2. Run the repository's documented local checks.
3. Open a pull request with the reason for the change, validation evidence, and
   rollback or recovery notes when operations could be affected.
4. Resolve review conversations and wait for required checks before merging.
5. Use squash merge unless a repository documents a different requirement.

Direct pushes and force pushes to protected default branches are not part of the
normal workflow.

## Security

- Never commit credentials, tokens, private keys, kubeconfigs, unredacted
  production values, or decrypted secret files.
- Treat generated logs, test output, migration archives, and screenshots as
  potentially sensitive.
- Use repository-supported encrypted secret storage and short-lived identity
  federation where available.
- Report suspected vulnerabilities through the
  [private security-reporting process](SECURITY.md), not through a public issue.

## Commits and pull requests

Use clear commit subjects. Conventional Commits are preferred where a repository
does not define a stricter convention, for example `fix(ci): validate rendered
manifests`.

A pull request should contain:

- a concise summary and motivation;
- tests and validation performed;
- security or secret-handling impact;
- deployment and rollback impact;
- post-deploy monitoring signals, or a reason none are required.

Repository-local instructions override this shared baseline when they are more
specific.
