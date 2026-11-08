# Pattern Selection

Choose patterns to solve demonstrated problems. A pattern adds concepts, failure modes, and operational overhead.

## Selection guide
- Start with a modular monolith when one deployable unit and clear internal boundaries meet the requirements.
- Use layered architecture when separation of transport, application, domain, and infrastructure concerns improves changeability.
- Use event-driven messaging when producers and consumers need temporal decoupling or independent scaling.
- Use CQRS only when read and write models have materially different needs.
- Use microservices when independent ownership, deployment, scaling, or fault isolation justify distributed-system costs.
- Use caching only with a clear invalidation and consistency strategy.

## Warning signs
Avoid microservices as a default, premature event sourcing, generic repositories that hide domain behavior, distributed transactions without a business need, and abstractions with only one trivial implementation.

## Decision tree
1. Can one team own and deploy the system safely as one unit? Prefer a modular monolith.
2. Do parts need independent scaling or release cadence? Evaluate service boundaries.
3. Is asynchronous decoupling required? Evaluate messaging and delivery guarantees.
4. Are read/write performance or model needs fundamentally different? Evaluate CQRS.
5. Is full history and replay a business requirement? Only then evaluate event sourcing.

## Validation
For every selected pattern, document the problem it solves, its new operational costs, failure behavior, and a simpler rejected alternative.
