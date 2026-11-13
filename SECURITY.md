# Security Policy

## Supported versions

| Version | Security support |
| --- | --- |
| Latest stable [release](https://github.com/sensodent/BustaSQL-Releases/releases/latest) | Supported for reports |
| Older releases | Upgrade and verify the issue persists |

## Report a vulnerability privately

**Do not create a public issue or discussion containing an exploit, connection strings, credentials, private data or sensitive logs.**

1. Visit the repository [Security tab](https://github.com/sensodent/BustaSQL-Releases/security) and use **Report a vulnerability** if GitHub private vulnerability reporting is enabled.
2. If it is not available, use a private contact method on the [repository owner's GitHub profile](https://github.com/sensodent), if provided. If no private channel exists, you may open a public issue asking the maintainer to establish one, **without sharing any vulnerability details**.

Helpful information: affected version, Windows version, database engine, impact and safe reproduction details. Share sensitive proof-of-concept material only in a confirmed private channel.

Examples in scope:

- Credential storage (Windows Credential Manager, Entra token cache) and settings export.
- The local server on `127.0.0.1` (authentication, CSRF and origin checks).
- Update integrity (`latest.yml`, installer download and verification).
- Read-only and Production-environment protections being bypassed.
- AI assistant permissions (actions run without the user's approval, or data sent beyond what is documented).
- SSH tunnels and host-key verification.

For vulnerabilities in database engines, drivers, Claude Code, Codex, Cursor or other third-party services alone, use the respective vendor's security program.

Reports are prioritized by impact and reproducibility. No fixed response or remediation time is guaranteed.
