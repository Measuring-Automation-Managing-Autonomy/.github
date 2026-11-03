# Security Policy

**Status:** draft · **Owned by:** MAMA Stewardship Council (Security/risk perspective)

## Supported components

| Repository | Component | Supported |
|---|---|---|
| `mama-integrations` | `mama-integrations` Python adapter | yes (0.x) |
| `mama-metrics` | metric-card validator (`tools/validate_cards.py`) | yes (0.x) |
| `mama-framework`, `.github` | documentation only | n/a — report content errors as issues |

## Reporting a vulnerability

**Do not open a public issue for a security vulnerability.**

Use GitHub's private vulnerability reporting: on the affected repository, go to **Security → Report a vulnerability**. If private reporting is unavailable for a repository, contact the organization owner [@emmanuel-a-otchere](https://github.com/emmanuel-a-otchere) directly.

Include: affected repository and version, a description of the issue, steps to reproduce or a proof of concept, and any known impact. Please do not include exploit code for third-party systems or any real organizational data.

## What to expect

- Acknowledgment within 5 business days.
- An assessment and remediation plan within 14 days for accepted reports.
- Coordinated disclosure: we publish advisories via GitHub Security Advisories after a fix ships, crediting reporters who wish to be named.
- No MAMA artifact is a certified or accredited security control; tool output must not be treated as a security assessment of anyone's systems (see [GOVERNANCE.md §6](GOVERNANCE.md#6-public-claims)).

## Scope notes

MAMA tools are local-first by design: they import/export files (YAML/JSON/CSV) and do not centralize telemetry or sensitive ledgers. Reports about data exfiltration, dependency compromise, or supply-chain risk in MAMA-published packages are in scope and taken especially seriously.
