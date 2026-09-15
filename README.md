# DPRGRMMD.COM

The production website for **DPRGRMMD**.

## Repository authority

**This repository is the sole source of truth for `dprgrmmd.com`.**

All website design, application code, Cloudflare Worker configuration, deployment changes, fixes, and future website development must be made in `dprgrmmd/dprgrmmdcom` only.

Do not place or deploy DPRGRMMD website code from the `cloudflare-mcp` repository. That repository is reserved exclusively for the Cloudflare MCP service and its supporting infrastructure.

Current production mapping:

- Repository: `dprgrmmd/dprgrmmdcom`
- Production Worker: `dprgrmmd-site`
- Production domain: `https://dprgrmmd.com`
- Current baseline: `v1.2.1`

## Direction

DPRGRMMD is designed as a digital object rather than a conventional corporate website: architectural, cinematic, restrained, and technically expressive. The V1 homepage uses generative WebGL, oversized editorial typography, subtle depth and motion, and a deliberately minimal content system.

## Runtime

- Cloudflare Workers
- Zero runtime dependencies
- WebGL hero with graceful CSS fallback
- Responsive and touch-aware
- `prefers-reduced-motion` support
- Production security headers
- `/health`, `/robots.txt`, and `/sitemap.xml`

## Development

```bash
npm install
npm run check
npm run dev
```

## Deployment

```bash
npm run deploy
```

`wrangler.jsonc` targets the `dprgrmmd-site` Worker and the `dprgrmmd.com` custom domain.

Production deployments must originate from this repository and should be validated before replacing the currently active production version.
