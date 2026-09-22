# Security Policy

## Supported versions

The project is pre-release. Only the latest commit on the default branch is considered supported.

## Reporting a vulnerability

Do not open a public issue containing exploit details, credentials or personal data. Use GitHub's private vulnerability reporting when enabled. Until that channel is available, contact the repository owner privately through the GitHub profile without including sensitive payloads in the first message.

## Open-source threat model

Assume attackers can read all source code, workflows, examples and configuration. Security must rely on access control, cryptography, isolation and validation—not obscurity.

## Never commit

- seed phrases, private keys or signing material;
- API tokens, OAuth secrets, cookies or database credentials;
- `.env` files or cloud service-account files;
- real transaction exports, wallet descriptors or customer identifiers;
- production URLs containing embedded credentials;
- payment cards, invoices or advertising account data.

If a secret is committed, removing the file is insufficient: revoke and rotate it, review access logs, then purge history only through an approved incident procedure.

## Product security boundaries

- Wallet integration is watch-only unless a future, separately approved security and regulatory phase changes this boundary.
- Uploaded files are untrusted: enforce size/type limits, parse defensively and isolate processing.
- Monetary quantities use exact decimal/integer representations; never binary floating point.
- Every calculated result must retain source and rule-version traceability.
- Logs must not contain full transaction exports or personal identifiers.

## Dependency and CI rules

- Use lockfiles and reproducible builds.
- Pin GitHub Actions to immutable commit SHAs.
- Review new dependencies for maintenance, license and known vulnerabilities.
- CI receives read-only permissions unless a narrowly documented write permission is required.
- Forked pull requests never receive production secrets.

## Responsible scope

AutoBTC is not a wallet, exchange, custodian or investment adviser. Features that cross these boundaries require explicit legal, security and owner approval before implementation.
