# Agent Authority

## Authority levels

| Level | Meaning |
|---|---|
| L0 | Read, analyze and report |
| L1 | Draft files, plans and proposals |
| L2 | Modify a dedicated branch and open a PR |
| L3 | External side effect requiring explicit owner authorization |
| L4 | Prohibited for agents |

## Default matrix

| Action | Level | Rule |
|---|---:|---|
| Research and analysis | L0 | Cite sources and confidence |
| Draft copy, code or policy | L1 | Mark assumptions |
| Create branch/PR | L2 | Explicit task authorization required |
| Merge or deploy | L3 | Owner approval required |
| Publish organic content | L3 | Owner approval required |
| Activate ads or subscriptions | L4 | Owner performs manually |
| Enter payment credentials | L4 | Never |
| Move or custody cryptoassets | L4 | Never |
| Change budget authorization | L3 | Exact written owner decision |

## Fail-closed rule

Missing, ambiguous, expired or conflicting approval means no external action and no spending.
