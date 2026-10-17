# Verification Strategy

## Critical behaviors

- A citation opens the correct source page and passage.
- Search and document viewing respect workspace access.
- Ingestion failures remain visible and do not appear as ready documents.
- Conversation streaming and interruption states remain understandable.

## Test layers

| Layer | Focus |
|---|---|
| Unit | Domain rules, validation and state changes without live external dependencies. |
| Integration | Consistency across application services and their storage or external-service adapters. |
| User journey | A complete path from a user action to its visible outcome, including failure states. |

## Environment checks

An answer is an interpretation of the available sources; citations and direct document inspection remain part of the user’s workflow.
