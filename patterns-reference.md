# Architecture Patterns Reference

| Pattern | Useful when | Main cost or risk |
|---|---|---|
| Layered architecture | Responsibilities need clear separation | Layers can become pass-through boilerplate |
| Modular monolith | One deployable unit with strong domain boundaries | Requires discipline around module dependencies |
| Hexagonal architecture | Domain logic must remain independent of infrastructure | More ports/adapters to maintain |
| Event-driven architecture | Producers and consumers need loose temporal coupling | Delivery, ordering, and observability complexity |
| CQRS | Read and write models have distinct requirements | More moving parts and eventual consistency |
| Saga | A business process spans independent services | Compensation and partial failure complexity |
| API gateway | Shared routing, auth, or rate controls are needed | Central dependency and policy sprawl |
| Cache-aside | Repeated reads justify caching | Staleness and invalidation complexity |

## Universal review
- Define ownership and boundaries.
- Specify failure behavior and timeouts.
- Document consistency guarantees.
- Make security and data classification explicit.
- Include observability and operational ownership.
- Prefer reversible decisions where uncertainty is high.
