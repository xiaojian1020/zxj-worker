# zxj-worker

Cloudflare Worker optimized for Free plan (ordinary proxy).

## Version
`2026.10.26.1_free_opt`

## Changes
- freeCpu enabled by default
- Budget tightened to 256KB / 48 connections
- Secondary fallback disabled when free protection is active
- Reduced long-tail CPU for ordinary proxy use

## How to use with Cloudflare

1. In Cloudflare Dashboard → Workers & Pages → Create → Connect to Git
2. Select this repository `xiaojian1020/zxj-worker`
3. For **Workers**, set the entry point to `_worker.js` (or upload the file manually if needed)
4. For **Pages**, put `_worker.js` in the root or functions directory as needed

## Manual upload
Download the latest `_worker.js` from the releases or contact for the optimized file.

After connecting Git, future updates can be pushed here and Cloudflare will auto-deploy.
