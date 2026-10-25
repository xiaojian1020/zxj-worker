# zxj-worker

Cloudflare Worker optimized for **Free plan** (ordinary proxy use).

## Version
`2026.10.26.1_free_opt`

## Optimizations
- `freeCpu` enabled by default
- Free budget tightened: **256 KB** data / **48** connections
- Secondary fallback connection is skipped when Free protection is active (reduces long-tail CPU)
- Optimized for ordinary proxy traffic

## Connect to Cloudflare

1. Cloudflare Dashboard → **Workers & Pages**
2. Create application → **Connect to Git**
3. Select repository: `xiaojian1020/zxj-worker`
4. Configure the build / entry according to your setup (Worker or Pages)
5. Deploy

After connecting, future pushes to this repo will trigger automatic deployments.

## File
- `_worker.js` — the optimized worker script (root of the repo)
