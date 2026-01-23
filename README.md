# Astro + Cloudflare Pages SSR Quickstart

Starter template for **Astro** projects with **Cloudflare Pages SSR**, **TailwindCSS**, and **TypeScript**.

## Prerequisites

- **Node.js** and **npm** must be installed.
- **Wrangler CLI** must be installed for Cloudflare deployment.

## Cloudflare Project Configuration

Before deploying, you must define the Cloudflare Pages project name used by Wrangler. Edit `package.json` and update the `cfProject` value under the `config` section.

## Getting Started

1. Install dependencies: `npm install`

2. Start the local Astro **development** server with hot reload: `npm run dev`

## Quick Workflow For Deployments

1. Log in to Cloudflare (if not already logged in): `npm run cf:login`

2. Create the project (first time only): `npm run cf:create`

3. Build the project locally: `npm run build`

4. Preview the project with SSR locally: `npm run preview`

5. Deploy to Cloudflare Pages: `npm run deploy`
