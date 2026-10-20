# Troubleshooting and safe reports

## A coding CLI is unavailable or authentication fails

Check whether the official CLI starts normally outside Coterie and whether its account has access and available quota. Follow the provider's instructions for installation and authentication. Do not share tokens, account exports or CLI credential files.

## A task is waiting or blocked

Read its displayed status and reason. Dependencies, approval requirements, provider capacity and account limits may affect when work can proceed. Include the exact visible reason when reporting a problem.

## A check fails or cannot run

Record the command, its result and the relevant error. Distinguish an environment problem from a failing assertion. Use an existing project check where possible and report if the same command also fails outside Coterie.

## Worktrees or merges need attention

Use a recoverable baseline and inspect the repository state before making manual changes. Avoid deleting or moving worktree metadata while a run is active. Include the visible error and a minimal reproduction rather than uploading your entire repository.

## What to include in a public issue

- Coterie build and Windows version.
- Relevant official CLI versions.
- Small, repeatable steps and expected versus actual behaviour.
- Redacted screenshots or the smallest relevant log excerpt.
- Whether the issue happens with one task, independent tasks or a dependency chain.

Remove private source code, personal directory names, emails, credentials and customer data. If you cannot share a minimal example safely, contact [coterie@offlinestudio.eu](mailto:coterie@offlinestudio.eu).

For potential vulnerabilities use [the private security-reporting process](../SECURITY.md).
