# Directory Structure

```text
chatbot-public-version/
├── backend/
│   ├── src/
│   │   └── assistant/
│   │       ├── access/
│   │       ├── conversations/
│   │       ├── core/
│   │       │   └── migrations/
│   │       │       └── versions/
│   │       ├── documents/
│   │       │   └── extraction/
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
│   │   ├── architecture/
│   │   ├── db/
│   │   ├── fixtures/
│   │   │   ├── branding/
│   │   │   ├── documents/
│   │   │   ├── module-004/
│   │   │   └── module-005/
│   │   │       ├── module-001/
│   │   │       │   ├── module-001/
│   │   │       │   │   ├── module-001/
│   │   │       │   │   └── module-003/
│   │   │       │   │       └── module-001/
│   │   │       │   └── module-003/
│   │   │       ├── module-002/
│   │   │       │   └── module-001/
│   │   │       │       └── module-001/
│   │   │       │           └── module-001/
│   │   │       └── module-004/
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
│   │   │   └── ui/
│   │   ├── lib/
│   │   │   └── conversation/
│   │   ├── module-008/
│   │   ├── module-012/
│   │   ├── pages/
│   │   │   ├── accueil/
│   │   │   ├── connexion/
│   │   │   ├── modeles/
│   │   │   ├── module-003/
│   │   │   ├── module-004/
│   │   │   ├── module-005/
│   │   │   │   ├── documents/
│   │   │   │   └── module-002/
│   │   │   ├── module-013/
│   │   │   ├── preferences/
│   │   │   ├── recherche/
│   │   │   ├── reglages/
│   │   │   │   └── module-007/
│   │   │   ├── supervision/
│   │   │   ├── usages/
│   │   │   └── utilisateurs/
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
