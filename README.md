# Chatbot — Document Knowledge Assistant

A document assistant that answers questions about an organization’s knowledge base and connects each answer to the relevant source passages.

Employees can ask a question in natural language instead of searching through folders and reading entire documents. Answers arrive progressively, with citations that open the source document at the relevant page. Knowledge is organized into workspaces with controlled access.

## Users

| Role | Use |
|---|---|
| Employees | Ask questions, inspect sources, browse documents and manage their conversations. |
| Administrators | Manage workspace access, document sources, model providers and operational monitoring. |

## Main features

- **Document-grounded conversations.** Ask follow-up questions and read answers alongside the material used to produce them.
- **Source inspection.** Open cited pages and passages in a document viewer rather than relying on an unsupported answer.
- **Workspace-based knowledge.** Keep document collections and user access aligned with distinct working contexts.
- **Document ingestion.** Index material from a read-only shared source or an administrator’s manual import.
- **Conversation tools.** Use attachments, conversation search, exports and personal preferences.
- **Administration.** Configure models and review processing failures, usage, latency and activity.

## Typical workflow

1. Choose an accessible workspace and ask a question.
2. Retrieve relevant passages from the indexed documents.
3. Read the streamed answer and open its citations.
4. Continue the conversation or inspect the source documents directly.

## Project structure

```text
chatbot-public-version/
├── backend/
│   ├── src/
│   │   └── assistant/
│   │       ├── access/
│   │       ├── conversations/
│   │       ├── core/
│   │       ├── documents/
│   │       ├── identity/
│   │       ├── knowledge/
│   │       ├── models/
│   │       ├── module-003/
│   │       ├── module-012/
│   │       ├── module-018/
│   │       ├── settings/
│   │       ├── spaces/
│   │       ├── supervision/
│   │       ├── usage/
│   │       └── app.py
│   ├── tests/
│   │   └── unit/
│   └── pyproject.toml
├── deploy/
│   ├── db/
│   │   └── initdb/
│   ├── migration/
│   ├── module-007/
│   │   ├── identity-portal/
│   │   │   └── README.md
│   │   └── provider/
│   │       └── README.md
│   ├── scripts/
│   └── README.md
├── docs/
│   ├── decisions/
│   │   └── README.md
│   ├── design/
│   │   ├── decisions.md
│   │   ├── requirements.md
│   │   └── verification.md
│   ├── integration/
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   ├── module-004/
│   │   └── README.md
│   ├── module-017/
│   ├── operations/
│   │   └── README.md
│   ├── rag/
│   │   └── README.md
│   ├── security/
│   └── specifications/
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── auth/
│   │   ├── buildplugins/
│   │   ├── components/
│   │   ├── lib/
│   │   ├── module-008/
│   │   ├── module-012/
│   │   ├── pages/
│   │   ├── shell/
│   │   ├── styles/
│   │   ├── test/
│   │   └── theme/
│   ├── tests/
│   │   └── e2e/
│   └── package.json
├── ARCHITECTURE.md
└── README.md
```

[Complete directory structure](docs/design/structure.md)

| Area | Responsibility |
|---|---|
| Web interface | React and TypeScript conversation, document-viewing and administration screens. |
| Application API | Python/FastAPI services for conversations, permissions and document access. |
| Background worker | Document ingestion, indexing and scheduled processing. |
| Knowledge storage | PostgreSQL with vector search, document metadata and private document files. |
| Model adapters | Server-side interfaces to language, embedding and document-processing models. |

## Technology

React, TypeScript, Vite, Python, FastAPI, PostgreSQL, pgvector and Docker.

## Engineering

- [Architecture](ARCHITECTURE.md)
- [Product requirements](docs/design/requirements.md)
- [Design decisions](docs/design/decisions.md)
- [Verification strategy](docs/design/verification.md)

An answer is an interpretation of the available sources; citations and direct document inspection remain part of the user’s workflow.

---

Source code, operational configuration and project-specific data are withheld for confidentiality.
