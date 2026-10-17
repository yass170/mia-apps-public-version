# Directory Structure

```text
mia-apps-public-version/
├── ai-workspace/
│   ├── assets/
│   │   └── module-001/
│   │       └── README.md
│   ├── backend/
│   │   ├── api/
│   │   │   ├── routers/
│   │   │   └── app.py
│   │   ├── cahier_des_charges_ia/
│   │   ├── extraction_texte/
│   │   ├── shared/
│   │   ├── test/
│   │   ├── transcription/
│   │   ├── worker/
│   │   │   └── main.py
│   │   └── requirements.txt
│   ├── database/
│   │   └── migrations/
│   │       └── versions/
│   ├── deploy/
│   │   ├── docker/
│   │   ├── scripts/
│   │   └── README.md
│   ├── docs/
│   │   ├── decisions/
│   │   │   └── README.md
│   │   ├── deployment/
│   │   │   └── README.md
│   │   ├── issue/
│   │   │   └── README.md
│   │   └── README.md
│   ├── frontend_react/
│   │   ├── docs/
│   │   │   └── apps/
│   │   │       ├── module-001/
│   │   │       │   └── README.md
│   │   │       ├── module-002/
│   │   │       │   └── README.md
│   │   │       ├── transcription/
│   │   │       │   └── README.md
│   │   │       └── README.md
│   │   ├── src/
│   │   │   ├── app/
│   │   │   ├── modules/
│   │   │   │   ├── delivery-note-archive/
│   │   │   │   ├── extraction/
│   │   │   │   ├── module-002/
│   │   │   │   ├── module-003/
│   │   │   │   ├── module-005/
│   │   │   │   ├── module-006/
│   │   │   │   ├── portal/
│   │   │   │   └── transcription/
│   │   │   ├── shared/
│   │   │   │   ├── api/
│   │   │   │   ├── auth/
│   │   │   │   ├── components/
│   │   │   │   ├── hooks/
│   │   │   │   ├── jobs/
│   │   │   │   ├── layouts/
│   │   │   │   └── storage/
│   │   │   └── styles/
│   │   ├── tests/
│   │   │   └── e2e/
│   │   │       └── support/
│   │   ├── package.json
│   │   └── README.md
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   └── README.md
├── docs/
│   └── design/
│       ├── decisions.md
│       ├── requirements.md
│       └── verification.md
├── identity-portal/
│   ├── backend/
│   │   ├── src/
│   │   │   ├── auth_broker/
│   │   │   │   ├── routers/
│   │   │   │   └── main.py
│   │   │   ├── identity_api/
│   │   │   │   ├── routers/
│   │   │   │   └── main.py
│   │   │   └── identity_core/
│   │   ├── tests/
│   │   │   └── integration/
│   │   ├── pyproject.toml
│   │   └── README.md
│   ├── database/
│   │   ├── migrations/
│   │   │   └── versions/
│   │   ├── tests/
│   │   └── README.md
│   ├── deploy/
│   │   ├── docker/
│   │   ├── scripts/
│   │   └── README.md
│   ├── docs/
│   │   ├── api/
│   │   ├── architecture/
│   │   ├── database/
│   │   ├── decisions/
│   │   │   └── README.md
│   │   ├── issue/
│   │   ├── module-009/
│   │   ├── operations/
│   │   ├── security/
│   │   └── specifications/
│   ├── examples/
│   │   └── sso_client_reference/
│   │       └── README.md
│   ├── frontend/
│   │   ├── src/
│   │   │   ├── api/
│   │   │   ├── assets/
│   │   │   │   └── README.md
│   │   │   ├── components/
│   │   │   └── routes/
│   │   │       └── admin/
│   │   ├── tests/
│   │   └── package.json
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   └── README.md
├── support-portal/
│   ├── backend/
│   │   ├── app/
│   │   │   ├── docs/
│   │   │   ├── support_content/
│   │   │   └── main.py
│   │   ├── tests/
│   │   ├── pyproject.toml
│   │   ├── README.md
│   │   └── requirements.txt
│   ├── deploy/
│   │   ├── docker/
│   │   ├── scripts/
│   │   ├── systemd/
│   │   └── README.md
│   ├── docs/
│   │   ├── decisions/
│   │   │   └── README.md
│   │   ├── issue/
│   │   └── support-content/
│   │       ├── module-001/
│   │       ├── prompts/
│   │       └── tutoriels/
│   ├── frontend/
│   │   ├── scripts/
│   │   ├── src/
│   │   │   ├── api/
│   │   │   ├── app/
│   │   │   ├── components/
│   │   │   │   └── docs/
│   │   │   ├── content/
│   │   │   │   ├── faq/
│   │   │   │   ├── module-001/
│   │   │   │   └── module-003/
│   │   │   ├── hooks/
│   │   │   ├── pages/
│   │   │   ├── styles/
│   │   │   ├── test/
│   │   │   └── utils/
│   │   ├── tests/
│   │   ├── package.json
│   │   └── README.md
│   ├── issues/
│   │   ├── epics/
│   │   ├── features/
│   │   ├── tasks/
│   │   └── README.md
│   └── README.md
├── ARCHITECTURE.md
└── README.md
```
