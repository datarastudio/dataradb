# DataraDB

**A native desktop database client for macOS and Windows — manage MySQL, PostgreSQL, MongoDB, Redis, SQLite, Oracle, and MSSQL from one unified interface.**

DataraDB is part of the [Datara](https://datara.studio) suite of developer tools.

---

## Supported Databases

| Engine | Notes |
|--------|-------|
| MySQL | Includes MariaDB |
| PostgreSQL | Full schema + function support |
| SQLite | Open local files or create new databases |
| MongoDB | Collection management, document viewer, JSON import/export |
| Redis | Key-value browser with type-aware display |
| Oracle | Schema and query support |
| Microsoft SQL Server | Full feature parity with other relational engines |

---

## Features

### Connection Management
- Save and manage named connections across all supported database engines
- Test a connection before saving
- Export and import connection configurations
- **SSH tunnel support** — connect to databases via an SSH jump host
- **DataraSSH integration** — if you use DataraSSH, your saved SSH hosts are automatically available as tunnel sources
- SSL/TLS configuration per connection

### Query Editor
- Execute SQL with paginated, scrollable results
- **Query history** — every executed query is recorded and searchable per connection
- **Saved queries** — bookmark frequently used queries with a name for quick access
- Cancel long-running queries mid-execution
- Save query results as a file

### AI Query Assistant
- **Generate queries** from a plain-English prompt — describe what you want and get a working SQL statement
- **Fix queries** — paste a broken query and an error message; the AI rewrites it
- **Voice input** — transcribe an audio prompt to generate queries hands-free
- **Sync diff summarisation** — get a plain-English summary of structure or data differences between two databases

### Schema Management
- Browse databases, tables, views, stored procedures/functions, and triggers in a sidebar tree
- **Visual table designer** — create and alter tables through a form UI; preview the generated SQL before executing
- Drop, truncate, and cascade-drop tables
- Create, rename, and drop databases and collections
- View the raw `SHOW CREATE TABLE` statement for any table

### Data Editing
- Insert, update, and delete rows directly in the result grid
- Reset auto-increment counters

### Database Sync *(Pro)*
- **Structure comparison** — diff the schema of two databases and preview every difference
- **Data comparison** — compare table contents row by row across two connections
- **Script generation** — produce a ready-to-run SQL migration script from any comparison
- **Script execution** — apply the sync script directly from the app, with optional transaction wrapping
- **AI summary** — get a human-readable explanation of what a sync will change
- Configurable options: include/exclude specific tables, handle drops, null mismatches, and more

### Data Import & Export
- **SQL export** — dump a full database or individual tables to a `.sql` file
- **SQL import** — parse and replay an existing SQL file statement-by-statement, with per-statement error reporting
- **Excel import** — map spreadsheet columns to database table columns with a preview step
- **JSON import/export** — for MongoDB collections
- **Binary export** — download binary column data directly to disk

### User Management *(MySQL / PostgreSQL / MariaDB)*
- List all database users
- Create users with configurable host restrictions
- Drop users
- Change passwords
- Grant and revoke database-level privileges
- Flush privileges

### Process Monitor
- View all active server processes/queries
- Kill any running process by ID

### Password Hash Utility
- Hash a plaintext string using bcrypt, SHA-256, SHA-512, Argon2id, or MD5
- Configurable cost rounds and Argon2 variants
- Useful for verifying stored hashes during debugging

### Security
- Sensitive connection credentials are encrypted at rest
- App-level password lock with bcrypt verification
- SSH tunnel IPC uses a loopback-only server with HMAC-derived tokens

---

## Platform Support

| Platform | Architecture |
|----------|-------------|
| macOS    | Apple Silicon (arm64), Intel (amd64) |
| Windows  | amd64, arm64 |

---

## Download

Pre-built installers are available on the [Releases](https://github.com/datarastudio/dataradb/releases) page.

- **macOS** — signed and notarized `.dmg`
- **Windows** — NSIS `.exe` installer (amd64 and arm64)

---

## Pricing

| | Free | Pro |
|---|---|---|
| Saved connections | 1 | Unlimited |
| Query editor | ✅ | ✅ |
| Schema management | ✅ | ✅ |
| Data import / export | ✅ | ✅ |
| User management | ✅ | ✅ |
| SSH tunnels | ✅ | ✅ |
| AI query assistant | ✅ | ✅ |
| Database sync & compare | — | ✅ |
| Migration script execution | — | ✅ |

Activate a Pro license key in **Settings → License**.

---

## Part of the Datara Suite

DataraDB works seamlessly alongside **DataraSSH** — enable the integration in Settings and your saved SSH hosts from DataraSSH become available as tunnel sources in DataraDB, with no credentials to re-enter.

---

## License

DataraDB is proprietary software. All rights reserved. © Datara.
