<div align="center">

# BustaSQL

### One database IDE. Every engine. Running on your machine.

**A modern desktop IDE for Microsoft SQL Server, Azure SQL Database, MySQL/MariaDB and PostgreSQL — with schema and data compare, execution plans, direct grid editing and an AI assistant.**

[![Latest release](https://img.shields.io/github/v/release/sensodent/BustaSQL-Releases?label=latest%20release&color=ef6257)](https://github.com/sensodent/BustaSQL-Releases/releases/latest)
![Windows](https://img.shields.io/badge/Windows-x64-242424?logo=windows)
![Databases](https://img.shields.io/badge/SQL%20Server%20%C2%B7%20Azure%20SQL%20%C2%B7%20MySQL%20%C2%B7%20PostgreSQL-242424)
![Free](https://img.shields.io/badge/Download-Free-242424)

**[⬇ Download BustaSQL for Windows](https://github.com/sensodent/BustaSQL-Releases/releases/latest)**

**🌐 English** · [🇪🇸 Español](README.es.md)

</div>

---

## Meet BustaSQL

**BustaSQL** is a desktop database IDE that runs entirely on your computer: a local server bound to `127.0.0.1` and a fast interface in its own window. It uses your network and your corporate VPN, and **never sends your SQL or data to BustaSQL servers** — there are none.

Explore thousands of tables, write queries with real IntelliSense, compare schemas and data between environments, and edit results directly in the grid. **No need to juggle separate tools for each engine.**

<!-- Screenshots: add assets/bustasql-editor.png and assets/bustasql-compare.png, then uncomment.
![BustaSQL query editor](assets/bustasql-editor.png)
![BustaSQL Schema Compare](assets/bustasql-compare.png)
-->

## What's inside?

| Feature | What you get |
| --- | --- |
| **Engines** | SQL Server 2008 and later, Azure SQL Database, MySQL 8 / MariaDB and PostgreSQL 10+, also through **SSH tunnels** with host-key verification. |
| **Authentication** | SQL logins, **Microsoft Entra ID interactive (MFA)**, Entra *Default* (Azure CLI), Service Principal, access token and Windows NTLM. |
| **Object explorer** | Virtualized, lazy-loaded tree: schemas, tables, columns, keys, indexes, triggers, logins, users and roles, with CREATE/ALTER/DROP/SELECT/INSERT/EXEC scripts. |
| **Query editor** | Monaco editor with IntelliSense from real metadata (aliases, CTEs, other databases), snippets, formatting, go-to-definition and syntax validation without running. |
| **Execution** | Run all, selection or current statement; `GO` batches; multiple result sets; cancel per tab; open-transaction indicator with COMMIT/ROLLBACK; **run one query on several databases at once**. |
| **Results grid** | Virtualized grid with real back-pressure for millions of rows, column filters, copy as table (pastes into Teams, Outlook, Excel), JSON/XML viewers and CSV/TSV/JSON/Excel export. |
| **Direct editing** | Edit cells, paste ranges, insert and delete rows, preview the SQL, apply in one transaction with conflict detection. |
| **Schema Compare** | Semantic comparison of tables, keys, indexes, views, procedures, functions and more, with a dependency-ordered, transactional sync script and data-loss warnings. |
| **Data Compare** | Streaming, batched comparison with composite keys and WHERE filters, side-by-side view and INSERT/UPDATE/DELETE scripts. |
| **Execution plans** | Estimated and actual plans, costs, warnings, missing-index suggestions, IO/TIME statistics and `.sqlplan` export. |
| **Table designer** | Create and alter tables with reviewable scripts, including drag-to-reorder columns while preserving data. |
| **AI assistant** | Chat and inline edits with **Claude Code**, **Codex** or **Cursor** (the CLIs installed on your machine, with your account): explores your real schema, writes queries and runs them with your permission. |
| **Safety** | Environment tags (Development / Test / **Production** with a red border and stronger confirmations) and read-only connections. |

## Get started

1. **[Download the latest Windows installer](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** (`BustaSQL-Setup-X.Y.Z.exe`).
2. Run it. It installs for your user, **without administrator rights** and **without Node.js**.
3. Open BustaSQL, click **+** in the explorer and create a connection.

> The installer is not code-signed yet. Windows SmartScreen may show *"Windows protected your PC"*: choose **More info → Run anyway** only if you downloaded it from this repository.

BustaSQL is **free to download**. AI provider accounts, subscriptions and usage limits are **separate** and are used only if you enable the assistant.

## Privacy, credentials and updates

- BustaSQL runs locally. Connections go directly from your computer to your database servers.
- Passwords are stored in the **Windows Credential Manager** (DPAPI), never in plain text. Settings can be exported **without secrets**.
- The only data that leaves your machine to a third party is the context you share with the **AI assistant**, sent to the provider you choose (Anthropic, OpenAI or Cursor) with your own account.
- Your connections, history and saved queries live in `%LOCALAPPDATA%\BustaSQL` and are kept when you uninstall.
- BustaSQL checks this repository for updates at startup and every 4 hours, verifies the download against the SHA-512 checksum in `latest.yml`, and asks you to restart.

## Support & community

- [Report a bug, ask a question or suggest a feature](https://github.com/sensodent/BustaSQL-Releases/issues/new/choose)
- [FAQ](FAQ.md) · [Support](SUPPORT.md) · [Security](SECURITY.md)
- [Contributing](CONTRIBUTING.md) · [Code of Conduct](CODE_OF_CONDUCT.md) · [Accessibility](ACCESSIBILITY.md) · [License notice](LICENSE)

## Download and project status

**[Latest release](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** · [All releases](https://github.com/sensodent/BustaSQL-Releases/releases)

- **Available installer:** Windows x64.
- **Source code:** currently private. This public repository distributes the application installers and update files, not the source.
- BustaSQL is an independent project and is not affiliated with Microsoft, Oracle, the PostgreSQL Global Development Group, MariaDB, Anthropic, OpenAI, Cursor or the other named products.

---

<div align="center">

**Query it. Compare it. Ship it.**

**[Download BustaSQL](https://github.com/sensodent/BustaSQL-Releases/releases/latest)** · [Leer en español](README.es.md)

</div>
