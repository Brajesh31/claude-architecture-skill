# Trade-off Analysis

Architecture decisions are choices between competing qualities. Make the trade-off explicit rather than claiming an option is universally best.

## Evaluation process
1. State the decision and the context.
2. Identify the quality attributes that matter for this decision.
3. List realistic options, including the simplest viable option.
4. Compare each option against the same criteria.
5. Record operational cost, migration cost, reversibility, and failure modes.
6. Choose an option and explain why rejected alternatives were not selected.

## Comparison template

| Criterion | Weight | Option A | Option B | Notes |
|---|---:|---:|---:|---|
| Delivery speed | 1-5 | 1-5 | 1-5 | |
| Operational burden | 1-5 | 1-5 | 1-5 | |
| Reliability | 1-5 | 1-5 | 1-5 | |
| Security | 1-5 | 1-5 | 1-5 | |
| Scalability | 1-5 | 1-5 | 1-5 | |
| Reversibility | 1-5 | 1-5 | 1-5 | |

Scores support discussion; they do not replace judgment. Explain the assumptions behind them.

## Decision quality checks
- Is the simplest alternative genuinely considered?
- Are costs shifted to another team or system?
- Does the option create vendor lock-in?
- Can the decision be reversed cheaply?
- What evidence would cause the decision to be revisited?

## ADR outline
Use Context, Decision Drivers, Options, Decision, Rationale, Consequences, Risks, and Follow-up as the minimum record.
