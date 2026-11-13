# claude-architecture-skill

A practical architecture decision skill for analyzing requirements, comparing system design options, selecting patterns, and recording decisions.

## Overview

This skill structures architecture work before implementation. It emphasizes understanding the problem, identifying constraints, evaluating trade-offs, selecting an appropriate design, and documenting the rationale.

## Core Workflow

1. Discover project context and clarify requirements.
2. Identify functional and non-functional constraints.
3. Classify system boundaries and dependencies.
4. Generate a small set of viable architecture options.
5. Compare complexity, cost, reliability, performance, security, and maintainability.
6. Select a pattern that fits the requirements.
7. Record the decision and its consequences in an Architecture Decision Record (ADR).
8. Revisit the decision when constraints materially change.

## What It Covers

- Context discovery and requirements analysis.
- Architecture trade-off evaluation.
- Pattern selection, including modular, service-oriented, and event-driven designs.
- Worked examples and pattern references.
- Architecture Decision Records.

## Installation

```bash
git clone https://github.com/Brajesh31/claude-architecture-skill.git ~/.claude/skills/architecture
```

## Usage

Invoke `/architecture` when planning a new system, reviewing a major design change, or documenting a technical decision. Provide project context, requirements, constraints, and the decision to be made.

## Decision Quality Checklist

- Requirements are explicit and testable.
- Constraints and assumptions are visible.
- Viable alternatives have been considered.
- Trade-offs use consistent criteria.
- Complexity is justified by a real requirement.
- Security, reliability, and operations are considered.
- The decision and its consequences are recorded.

## Repository Contents

- `SKILL.md`: Main decision-making workflow.
- `references/`: Supporting architecture guides.
- `README.md`: Installation, workflow, and overview.

## Creator and maintainer

Created and maintained by **Brajesh Kumar**.
