# Backend

Server-side code for the current business idea: API, data layer, auth, and integrations.

## Intended layout

```
backend/
├── src/
│   ├── routes/       # HTTP endpoints
│   ├── services/     # Business logic
│   ├── models/       # Data models / schemas
│   └── config/       # App configuration
├── tests/
└── README.md
```

## Stack

To be chosen per business. Common options:

- **Node.js** — Express, Fastify, or NestJS
- **Python** — FastAPI or Django REST
- **Database** — PostgreSQL, SQLite (dev), or managed service

## Local development

Setup instructions will go here once the stack is picked.

```bash
# Example (Node)
cd backend
npm install
npm run dev
```

## Environment

Create a `.env` file in this folder (not committed). Typical variables:

```
PORT=3001
DATABASE_URL=
API_SECRET=
```
