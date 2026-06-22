# Next Business Idea

A monorepo for building and launching new business ideas. Each project lives in the same structure so we can move fast from concept to product.

## Structure

```
Next-Business-Idea/
├── backend/     # API, services, database, business logic
├── frontend/    # Web app, UI, client-facing experience
└── README.md
```

## Workflow

1. **Define the idea** — What problem does this business solve? Who is the customer?
2. **Backend** — Models, API routes, auth, integrations, and core logic
3. **Frontend** — Pages, components, and user flows
4. **Ship** — Deploy, iterate, and decide whether to keep or pivot

## Getting started

### Backend

See [backend/README.md](./backend/README.md).

### Frontend

See [frontend/README.md](./frontend/README.md).

## Conventions

- Keep business-specific code inside `backend/` and `frontend/` — avoid scattering logic at the repo root
- Document decisions and API contracts as you build
- Use environment variables for secrets (never commit `.env` files)

## Status

Scaffold in place — ready for the first business idea.
