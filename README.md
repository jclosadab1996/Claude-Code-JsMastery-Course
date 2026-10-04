# Claude-Code-JsMastery-Course

Next.js eCommerce app — initial setup.

## Stack

- Next.js (App Router, TypeScript, `src/` dir)
- Tailwind CSS v4
- Better Auth (`src/lib/auth.ts`, client in `src/lib/auth-client.ts`, handler at `/api/auth/[...all]`)
- Drizzle ORM + Neon serverless Postgres (`src/db`, `drizzle.config.ts`)

## Getting started

```bash
npm install
cp .env.example .env   # fill in DATABASE_URL and BETTER_AUTH_SECRET
npm run dev
```

## Scripts

| Script | Purpose |
| --- | --- |
| `npm run dev` / `build` / `start` | Next.js |
| `npm run lint` / `typecheck` | ESLint / TypeScript |
| `npm run auth:generate` | Generate Better Auth tables into `src/db/auth-schema.ts` |
| `npm run db:generate` / `db:migrate` | Create / apply Drizzle migrations |
| `npm run db:push` | Push schema directly (dev) |
| `npm run db:studio` | Open Drizzle Studio |
