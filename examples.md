# Architecture Examples

These are illustrative starting points. Adapt them to actual constraints rather than copying them blindly.

## MVP
- Single deployable application
- Clear module boundaries
- Managed relational database
- Stateless application instances
- Basic structured logs, health checks, backups, and CI
- Add queues or caches only when justified

## SaaS product
- Tenant-aware authorization and data isolation
- API boundary with validation and rate limiting
- Background job processing for slow workflows
- Audit events for sensitive actions
- Metrics for latency, errors, and tenant-level usage
- Tested backup and restore process

## Enterprise integration platform
- Explicit contracts for external systems
- Queue-based handling for unreliable dependencies
- Idempotency keys and retry limits
- Dead-letter handling and operational replay controls
- Centralized identity and secrets management
- End-to-end tracing and ownership documentation

## Review questions
For each example, verify security boundaries, data ownership, failure handling, deployment complexity, cost, and team capability before adoption.
