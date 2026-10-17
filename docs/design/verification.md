# Verification Strategy

## Critical behaviors

- An application opens only within the appropriate access context.
- Long-running work has visible progress and failure states.
- A user receives only their authorized files and deliverables.
- A child-application update preserves the suite’s integration boundaries.

## Test layers

| Layer | Focus |
|---|---|
| Unit | Domain rules, validation and state changes without live external dependencies. |
| Integration | Consistency across application services and their storage or external-service adapters. |
| User journey | A complete path from a user action to its visible outcome, including failure states. |

## Environment checks

A shared portal does not make application data interchangeable; identity, document ownership and application-specific processing remain separate concerns.
