# Astro + Cloudflare Pages SSR Quickstart Template

A quickstart template for web applications built with **Astro** and **Cloudflare Pages SSR**, leveraging **TypeScript** for type safety, **Tailwind CSS** for utility-first styling and **Wrangler CLI** for deployment.

## Prerequisites

- **Node.js** and **npm** must be installed.

## Cloudflare Project Configuration

Before deployment, the project name used by Wrangler must be defined in the `config.name` field of `package.json`.

## Database (Cloudflare D1)

This project supports an optional Cloudflare **D1** database.

When D1 is used, the database binding **must** be declared in `wrangler.toml` before running locally or deploying.

### Configuration

```toml
[[d1_databases]]
binding = "db"
database_name = ""
database_id = ""
remote = true
```

## Getting Started

1. Install dependencies: `npm install`

1. Log in to Cloudflare (if not already logged in): `npm run login`

1. Start the local **development** server (hot reload enabled): `npm run dev`

### Database scripts

The following npm scripts are provided for the D1 database management:

- `npm run db:info` — show D1 database info
- `npm run db:create` — create D1 database
- `npm run db:init` — initialize D1 schema

## Quick Workflow For Deployments

1. Log in to Cloudflare (if not already logged in): `npm run login`

2. Preview the project locally: `npm run preview`

3. Deploy to Cloudflare: `npm run deploy`
