# DPRGRMMD.COM

The production website for **DPRGRMMD**.

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

Production Worker: `dprgrmmd-site`

Production domain: `https://dprgrmmd.com`
