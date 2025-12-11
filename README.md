# WhatsApp CRM (monorepo)

## Structure
- `apps/web` — Next.js frontend
- `apps/worker` — background worker & WA driver
- `packages/shared` — shared utilities & types

## Quick start (local)
1. Start dev services:
```bash
docker compose up -d
```

2. Install dependencies (root uses npm workspaces):
```bash
npm run install:all
```

3. Start web app:
```bash
npm run dev:web
# open http://localhost:3000
```

4. Start worker (in another terminal):
```bash
npm run dev:worker
```

## Notes
- Add `.env` files in each app before starting if required.
- We'll wire the WhatsApp driver and DB next.
