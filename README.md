# Admin Panel App build harness

Public workflow instructions only. Application source stays in a private repository and is checked out with a repository-scoped read-only deploy key. Manual dispatch only; no pull-request builds.

Build stdout/stderr, diagnostics and binaries are encrypted with age before upload. Only the recipient private key on the owner's inf machine can decrypt them. No plaintext artifacts, source archives, build caches, or releases are published here. Encrypted artifacts expire after seven days. Platform/toolchain metadata and repository identity remain visible in workflow logs.

The private app repository provides the one-command dispatch, encrypted-result collection and authenticated download-portal publishing. Default builds are Android debug and iOS simulator, not signed store releases.
