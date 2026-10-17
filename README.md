# MIA Apps — Enterprise AI Application Suite

A suite of internal web applications that combines a shared sign-in portal, AI-assisted document tools and IT support resources.

Employees access several document-oriented applications through a common entry point. The suite brings together identity and application access, audio transcription, PDF text extraction, assisted document preparation and support documentation, while keeping the individual applications organized as separate components.

## Users

| Role | Use |
|---|---|
| Employee | Open authorized applications, submit source documents and retrieve generated deliverables. |
| Application administrator | Manage access and application availability. |
| IT administrator | Maintain the suite and consult operating and support documentation. |

## Main features

- **Shared application portal.** Provide one entry point for sign-in and access to available applications.
- **Central identity.** Coordinate user identity and access across the integrated applications.
- **Document-processing workspace.** Prepare sources, launch a processing job and review the result.
- **AI-assisted tools.** Support transcription, PDF text extraction and document preparation.
- **Personal deliverables.** Collect generated outputs and distinguish temporary results from files saved by the user.
- **Support portal.** Provide technical documentation, guidance and reusable support content.

## Typical workflow

1. Sign in and choose an authorized application.
2. Upload or select the sources needed for a document task.
3. Follow the processing status and review the generated output.
4. Download the deliverable or save it to the user’s file space.

## Project structure

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
│   │   ├── src/
│   │   │   ├── app/
│   │   │   ├── modules/
│   │   │   ├── shared/
│   │   │   └── styles/
│   │   ├── tests/
│   │   │   └── e2e/
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
│   │   │   ├── identity_api/
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
│   │   │   ├── components/
│   │   │   └── routes/
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
│   │   │   └── components/
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

[Complete directory structure](docs/design/structure.md)

| Area | Responsibility |
|---|---|
| Identity portal | Authentication, user session and controlled routing to applications. |
| AI workspace | React interface and Python services for document-processing tools. |
| Background workers | Long-running processing separated from interactive requests. |
| Application data and private files | Persistent job records, metadata and user-owned deliverables. |
| Support portal | Documentation, tutorials and IT guidance. |
| Parent repository | Integrates independently maintained application projects through Git subtrees. |

## Technology

React, JavaScript/TypeScript, Python, FastAPI, PostgreSQL, background workers, Docker and Git subtrees.

## Engineering

- [Architecture](ARCHITECTURE.md)
- [Product requirements](docs/design/requirements.md)
- [Design decisions](docs/design/decisions.md)
- [Verification strategy](docs/design/verification.md)

A shared portal does not make application data interchangeable; identity, document ownership and application-specific processing remain separate concerns.

---

Source code, operational configuration and project-specific data are withheld for confidentiality.
