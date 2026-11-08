# claude-architecture-skill

A practical architecture decision skill for analyzing requirements, comparing system design options, selecting patterns, and recording decisions.

## Overview

This skill helps structure architecture work before implementation begins. It emphasizes understanding the problem, identifying constraints, evaluating trade-offs, selecting an appropriate design, and documenting why that decision was made.

Architecture should follow the needs of the system. The goal is not to choose the most elaborate pattern, but to choose a design that fits the product, team, scale, and operational constraints.

## Core Workflow

1. Discover the project context and clarify the requirements.
2. Identify functional and non-functional constraints.
3. Classify the system and its major boundaries.
4. Generate a small set of viable architecture options.
5. Compare trade-offs such as complexity, cost, reliability, performance, security, and maintainability.
6. Select a pattern that fits the actual requirements.
7. Record the decision and its consequences in an Architecture Decision Record (ADR).
8. Revisit the decision when constraints materially change.

## What It Covers

### Context Discovery

Clarify users, system boundaries, dependencies, data flows, deployment environment, expected load, reliability needs, and delivery constraints.

### Trade-off Analysis

Compare options using explicit criteria. Consider both immediate implementation cost and long-term operational burden.

### Pattern Selection

Evaluate architectural patterns and avoid applying them without a concrete reason. Consider modular monoliths, service-oriented boundaries, event-driven systems, and other patterns in the context of the problem.

### Examples and Reference Patterns

Use the included examples and pattern reference to understand how design choices apply to different project sizes and requirements.

### Decision Records

Capture the context, decision, alternatives, consequences, and follow-up actions so future contributors can understand the rationale.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-architecture-skill.git ~/.claude/skills/architecture
```

## Usage

Invoke the skill when planning a new system, reviewing a major design change, or documenting a technical decision:

```text
/architecture
```

Provide the project context, requirements, constraints, and the decision that needs to be made. If information is missing, identify the unknowns rather than silently assuming answers.

## Reference Guide

| File | Purpose |
|---|---|
| `context-discovery.md` | Questions and project classification |
| `trade-off-analysis.md` | Evaluation criteria and ADR guidance |
| `pattern-selection.md` | Pattern selection and anti-patterns |
| `examples.md` | Worked architecture examples |
| `patterns-reference.md` | Quick reference for architecture patterns |

## Decision Quality Checklist

- Requirements are explicit and testable.
- Constraints and assumptions are visible.
- More than one viable option has been considered where appropriate.
- Trade-offs are evaluated against the same criteria.
- Complexity is justified by a real requirement.
- Security, reliability, and operations are considered.
- The decision and its consequences are recorded.
- The design can evolve without unnecessary coupling.

## Repository Contents

- `SKILL.md`: Main decision-making workflow.
- `references/`: Supporting architecture guides.
- `README.md`: Installation, workflow, and reference index.
