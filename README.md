# EarningsPulse — Cloudflare Workers experiment

Isolated copy of the Next.js frontend, adapted with [OpenNext](https://opennext.js.org/cloudflare) so it can run on Cloudflare Workers.

The FastAPI backend is unchanged and still lives in the main EarningsPulse repo. Point the frontend at it with `NEXT_PUBLIC_BACKEND_URL`.

Wrangler is a local `devDependency`. Use that copy via `npx`, not a global install:

```bash
bun install
npx wrangler --version
npx wrangler login
npx wrangler whoami

bun run preview   # local Workers runtime
bun run deploy
```
