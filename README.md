# Astro + Cloudflare Pages SSR Quickstart Template

A quickstart template for web applications built with **Astro** and **Cloudflare Pages SSR**, leveraging **TypeScript** for type safety, **Tailwind CSS** for utility-first styling and **Wrangler CLI** for deployment.

## Prerequisites

- **Node.js** and **npm** must be installed.

## Getting Started

1. Install dependencies: `npm install`

2. Start the local Astro **development** server with hot reload: `npm run dev`

## Cloudflare Project Configuration

Before deploying, you must define the Cloudflare project name used by Wrangler. Edit `wrangler.toml` to update the `name` field.

## Quick Workflow For Deployments

1. Log in to Cloudflare (if not already logged in): `npm run login`

2. Preview the project locally: `npm run preview`

3. Deploy to Cloudflare: `npm run deploy`
