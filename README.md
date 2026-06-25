# Next Business Idea

A monorepo for building and launching new business ideas. Each project lives in the same structure so we can move fast from concept to product.

## Motivation

Starting a new business idea often means reinventing the same scaffolding: repo layout, backend and frontend folders, environment conventions, and a repeatable workflow from idea to MVP. This repository provides a consistent starting point so you can focus on the product instead of project setup.

The monorepo keeps server and client code side by side, makes it easy for reviewers to clone and explore, and documents how each new idea should be structured as it grows.

## Structure

```
Next-Business-Idea/
├── backend/     # API, services, database, business logic
├── frontend/    # Web app, UI, client-facing experience
└── README.md
```

## Quick Start

1. **Clone the repository**

   ```bash
   git clone https://github.com/Gdawg399/Next-Business-Idea.git
   cd Next-Business-Idea
   ```

2. **Pick your stack** — Choose backend and frontend technologies for the current business idea (see [backend/README.md](./backend/README.md) and [frontend/README.md](./frontend/README.md)).

3. **Scaffold the app** — Add source code under `backend/` and `frontend/` following the layouts described in each subfolder README.

4. **Run locally** — Once dependencies are in place:

   ```bash
   # Backend (example: Node.js)
   cd backend
   npm install
   npm run dev

   # Frontend (example: Next.js) — in a second terminal
   cd frontend
   npm install
   npm run dev
   ```

   Exact commands depend on the stack you choose; update the subfolder READMEs when you commit to a framework.

## Usage

Use this repo as a template for each new business idea:

1. **Define the idea** — What problem does this business solve? Who is the customer?
2. **Backend** — Models, API routes, auth, integrations, and core logic in `backend/`
3. **Frontend** — Pages, components, and user flows in `frontend/`
4. **Ship** — Deploy, iterate, and decide whether to keep or pivot

### Conventions

- Keep business-specific code inside `backend/` and `frontend/` — avoid scattering logic at the repo root
- Document decisions and API contracts as you build
- Use environment variables for secrets (never commit `.env` files)

### Environment

| Location   | File         | Typical variables                          |
| ---------- | ------------ | ------------------------------------------ |
| `backend/` | `.env`       | `PORT`, `DATABASE_URL`, `API_SECRET`       |
| `frontend/`| `.env.local` | `NEXT_PUBLIC_API_URL=http://localhost:3001`|

See [backend/README.md](./backend/README.md) and [frontend/README.md](./frontend/README.md) for details.

## Contributing

### Clone the repo

```bash
git clone https://github.com/Gdawg399/Next-Business-Idea.git
cd Next-Business-Idea
```

### Set up for local development

The repo is currently a scaffold. After choosing a stack, install dependencies in each app folder:

```bash
# Backend
cd backend
npm install
npm run dev

# Frontend (separate terminal)
cd frontend
npm install
npm run dev
```

When you add a backend or frontend framework, document the exact install, build, and test commands in that folder's README.

### Run the test suite

Once tests are added for your chosen stack:

```bash
# Backend
cd backend
npm test

# Frontend
cd frontend
npm test
```

Replace `npm test` with the appropriate command for your stack (for example, `go test ./...` or `pytest`).

### Submit a pull request

If you'd like to contribute, please fork the repository and open a pull request to the `main` branch.

## Status

Scaffold in place — ready for the first business idea.
