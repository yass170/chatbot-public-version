# Product Requirements

A document assistant that answers questions about an organization’s knowledge base and connects each answer to the relevant source passages.

## Users

| Role | Expected outcome |
|---|---|
| Employees | Ask questions, inspect sources, browse documents and manage their conversations. |
| Administrators | Manage workspace access, document sources, model providers and operational monitoring. |

## Functional scope

| Capability | User outcome |
|---|---|
| Document-grounded conversations | Ask follow-up questions and read answers alongside the material used to produce them. |
| Source inspection | Open cited pages and passages in a document viewer rather than relying on an unsupported answer. |
| Workspace-based knowledge | Keep document collections and user access aligned with distinct working contexts. |
| Document ingestion | Index material from a read-only shared source or an administrator’s manual import. |
| Conversation tools | Use attachments, conversation search, exports and personal preferences. |
| Administration | Configure models and review processing failures, usage, latency and activity. |

## Main user journey

1. Choose an accessible workspace and ask a question.
2. Retrieve relevant passages from the indexed documents.
3. Read the streamed answer and open its citations.
4. Continue the conversation or inspect the source documents directly.

## Acceptance priorities

- A citation opens the correct source page and passage.
- Search and document viewing respect workspace access.
- Ingestion failures remain visible and do not appear as ready documents.
- Conversation streaming and interruption states remain understandable.

## Product constraint

An answer is an interpretation of the available sources; citations and direct document inspection remain part of the user’s workflow.
