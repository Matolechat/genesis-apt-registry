# Genesis Connectors — signed APT packages

[MIA NOTE] 2026-10-09 — This site distributes only signed packages, index metadata and public signing key. Source/publisher secrets stay private.

**Development preview release:** `genesis 0.1.0~dev0-1`.
This command-line client does not imply that customer login, billing, compute jobs or public Genesis API are live.

## Supported repositories

- `apt/termux`: Android Termux (standard `com.termux` prefix; `aarch64` index, all-architecture Python package).
- `apt/debian`: Debian/Ubuntu-style Linux (`amd64` index, all-architecture Python package).

Archive signing GPG fingerprint:

```
7F89283A652B2C8756F0535BFBB4F7D5040DCB12
```

The archive key is the public `genesis-archive-keyring.gpg` file.

Configure your APT source with `signed-by` and use HTTPS. **Never use `trusted=yes`.**
An APT repository is not automatically added by installing or running an MCP client.

Each candidate release must be checked for source identity, tests, pinned hashes, and signed `InRelease` receipts.
Actual publication and on-device installations are independently verified.

Publisher: Genesis Connectors.
