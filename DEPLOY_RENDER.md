# Ledger POS — Render deployment

This project is configured for Render with a Node/Express web service and PostgreSQL.

## Render Blueprint
- Build: `npm install && npx prisma generate`
- Start: `npm run start:setup`
- `DATABASE_URL` is connected automatically to the Render Postgres database.
- `JWT_SECRET` is generated automatically by Render.
- `start:setup` runs `prisma db push`, seeds the demo data, then starts the server.

## Demo login
- Admin PIN: `1234`
- Cashier PIN: `1111`

Change these before using the app for real business data.

## GitHub
Do not commit `.env` or real secrets. `.env.example` is safe to commit.
