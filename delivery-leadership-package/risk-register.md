# Risk Register

| # | Risk | Owner | Likelihood (L/M/H) | Impact (L/M/H) | Mitigation | Trigger to escalate |
|---|---|---|---|---|---|---|
| R1 | Sponsor's rate file includes invalid values | Dev Team | L | H | Run 'npm run type-check' and fix compilation errors locally | Build Fails type-check |
| R2 | Dev server does not run | Dev Team | L | H | Run 'npm run type-check' and fix compilation errors locally | Dev shell fails to load, type-check fails |
| R3 | Dependency Flagged and must be mitigated before release | Dev Team | M | M | Halt project work, identify a fix and apply | Report from platform team triggers remediation and is reported to dev team |
| R4 | Scope creep with additional requirements | Business Team | H | M | Discuss tradeoffs and adjust priorities, shift expectations and final goals | Request from project sponsor |
| R5 | Prod functionality is compromised and users are affected | Business and Dev Teams | M | H | Immediately postpone additional work and prioritize a fix | Prod Defect Reported |

## How I'll use this register

I will check this register daily until the project is delivered with the whole team. Priorities can be discussed and shifted as needed and as approved by the business.
