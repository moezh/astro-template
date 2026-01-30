# Astro + Cloudflare Pages SSR Quickstart Template

A quickstart template for web applications built with **Astro** and **Cloudflare Pages SSR**, leveraging **TypeScript** for type safety, **Tailwind CSS** for utility-first styling and **Wrangler CLI** for deployment.

## Prerequisites

- **Node.js** and **npm** must be installed.

## Cloudflare Project Configuration

Before deploying, you must define the Cloudflare project name used by Wrangler. Edit `wrangler.toml` to update the `name` field.

## Database (Cloudflare D1)

This project supports an optional Cloudflare **D1** database.

When D1 is used, the database binding **must** be declared in `wrangler.toml` before running locally or deploying.

### Configuration

```toml
[[d1_databases]]
binding = "db"
database_name = "db"
database_id = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXX"
```

### Database scripts

The following npm scripts are provided for databases management:

- `npm run db:list` — list existing D1 databases
- `npm run db:create` — create a database
- `npm run db:delete` — delete a database

## Getting Started

1. Install dependencies: `npm install`

1. Log in to Cloudflare (if not already logged in): `npm run login`

1. Start the local **development** server (hot reload enabled): `npm run dev`

## Quick Workflow For Deployments

1. Log in to Cloudflare (if not already logged in): `npm run login`

2. Preview the project locally: `npm run preview`

3. Deploy to Cloudflare: `npm run deploy`
