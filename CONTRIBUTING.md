# Contributing

## Branches

Use `<type>/<short-description>`, for example `feature/csv-diagnostic` or `chore/project-governance`.

## Change flow

1. Start from an approved issue/story.
2. Add a small, reviewable change.
3. Run relevant tests and policy checks.
4. Open a PR using the repository template.
5. Address review without weakening requirements.

## Commit convention

Use Conventional Commits: `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:` or `security:`.

## Domain quality

- Model money and asset quantities explicitly.
- Keep import adapters separate from the canonical ledger.
- Version business and tax rules by jurisdiction and effective date.
- Preserve idempotency and auditability.
- Do not place exchange-specific conditions inside the core domain.

## Public repository hygiene

Use synthetic data and placeholders. Before pushing, inspect staged changes for secrets, personal paths, emails, transaction IDs and internal URLs.
