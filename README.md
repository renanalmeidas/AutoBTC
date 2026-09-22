# AutoBTC

AutoBTC is an open-source platform for importing, normalizing, reconciling and auditing Bitcoin and cryptoasset transaction histories.

The initial product thesis is a self-service diagnostic: a user uploads an exchange CSV or provides read-only blockchain data and receives a traceable report of duplicates, missing acquisition costs, internal transfers and inconsistent records.

## Project status

**Discovery and governance.** No production financial processing is implemented.

## Non-negotiable boundaries

- AutoBTC does not request or store seed phrases or private keys.
- AutoBTC does not custody, transfer or trade cryptoassets.
- Outputs are technical aids, not legal, tax, accounting or investment advice.
- Real-world spending is disabled by default and requires the owner's explicit manual approval.
- Secrets, personal financial records and production datasets must never be committed.

## Repository map

```text
docs/product/       Product vision and measurable outcomes
docs/governance/    Scrum, authority, approvals and spending rules
docs/agents/        Versioned contracts for specialized agents
docs/templates/     Stories, technical specs, campaigns and handoffs
config/             Machine-readable project policy
```

Start with [AGENTS.md](AGENTS.md), [SECURITY.md](SECURITY.md) and [the product vision](docs/product/VISION.md).

## Current budget state

```yaml
authorized_total: 0.00
real_spend_enabled: false
human_payment_only: true
```

No agent approval overrides these values.

## License

Code is licensed under MIT. Brand assets, names and trademarks are not granted by the software license unless explicitly stated.
