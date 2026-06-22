# Frontend

Client-facing web app for the current business idea: UI, routing, and API consumption.

## Intended layout

```
frontend/
├── src/
│   ├── app/          # Routes / pages (framework-dependent)
│   ├── components/   # Reusable UI
│   ├── lib/          # Helpers, API client, utilities
│   └── styles/       # Global styles / design tokens
├── public/
└── README.md
```

## Stack

To be chosen per business. Common options:

- **Next.js** — React with SSR and app router
- **Vite + React** — Lightweight SPA
- **Tailwind CSS** — Utility-first styling

## Local development

Setup instructions will go here once the stack is picked.

```bash
# Example (Next.js)
cd frontend
npm install
npm run dev
```

## Environment

Create a `.env.local` file in this folder (not committed). Typical variables:

```
NEXT_PUBLIC_API_URL=http://localhost:3001
```
