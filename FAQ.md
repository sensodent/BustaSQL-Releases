# Frequently Asked Questions

### Is BustaSQL free?

Yes, the application installer is free to download. AI provider subscriptions and usage limits are independent and may involve separate charges if you use the assistant.

### Is BustaSQL open source?

No. **BustaSQL's source is currently private.** This public repository contains releases, update files and community documentation. See [LICENSE](LICENSE).

### Which databases are supported?

Microsoft SQL Server 2008 and later, Azure SQL Database, MySQL 8 / MariaDB and PostgreSQL 10+. Any of them can also be reached through an SSH tunnel (password, key or agent) with host-key verification.

### Which authentication methods work with SQL Server and Azure SQL?

SQL logins, Microsoft Entra ID interactive (MFA, opens your system browser), Entra *Default* (Azure CLI `az login`, environment variables), Entra password, Service Principal, access token and Windows NTLM (domain, user and password). Passwordless Windows integrated authentication (SSPI/Kerberos) is not available yet.

### Which operating system is supported?

The published installer is for **Windows x64**. It installs per user and does not need administrator rights or Node.js.

### Windows SmartScreen warns me about the installer. Is it safe?

The installer is not code-signed yet, so SmartScreen shows *"Windows protected your PC"*. Only run installers downloaded from the [official releases page](https://github.com/sensodent/BustaSQL-Releases/releases), then choose **More info → Run anyway**.

### Does BustaSQL send my SQL or data anywhere?

No. BustaSQL runs a local server bound to `127.0.0.1` and connects directly to your databases. The only exception is the optional **AI assistant**: the context it reads (editor text, schema, results it queries) is sent to the provider you select — Anthropic (Claude Code), OpenAI (Codex) or Cursor — using your own account.

### Where are my passwords and settings stored?

Passwords are stored in the Windows Credential Manager (DPAPI), never in plain text. Connections, history and saved queries are stored in `%LOCALAPPDATA%\BustaSQL` and are kept when you uninstall.

### What does the AI assistant need?

Claude Code, Codex and/or Cursor Agent installed and signed in on your computer (`claude`, `codex login`, `agent login`). BustaSQL does not manage accounts or API keys; usage counts against your plan.

### How do I update?

BustaSQL checks for updates at startup and every 4 hours, downloads them in the background and asks you to restart. You can also download any version from the [releases page](https://github.com/sensodent/BustaSQL-Releases/releases).

### Where do I ask for help?

See [SUPPORT.md](SUPPORT.md), the [issue templates](https://github.com/sensodent/BustaSQL-Releases/issues/new/choose), and [SECURITY.md](SECURITY.md) for private vulnerability reporting.
