# Demo Database Setup

This project now supports a demo-only backend path that is isolated from production.

## 1) Create a demo database
- In your MongoDB provider (Atlas/local), create a new database name for portfolio use only.
- Example name: `scrapyard_portfolio_demo`.

## 2) Configure backend demo environment
- In `scrapyard-backend-portfolio`, create a local `.env` using `scrapyard-backend-portfolio/.env.portfolio.example`.
- Set `MONGO_URI` to the new demo DB URI.
- Do not keep production DB credentials in this repository.
- If you use Atlas SRV, host should look like `cluster0.xxxxx.mongodb.net`.

## 3) Configure frontend demo environment
- In `scrapyard-frontend-portfolio`, set `VITE_API_URL=http://localhost:5001/api`.
- Reference: `scrapyard-frontend-portfolio/.env.portfolio.example`.

## 4) Bootstrap demo data
- From `scrapyard-backend-portfolio`:
  - `npm run portfolio:create-user`
  - `npm run portfolio:seed`
  - `npm run portfolio`

## Safety notes
- `server.js` now refuses to start unless `MONGO_URI` is set.
- Demo seeding and demo user creation use the same `MONGO_URI` demo database.
- Backend now blocks URIs that do not include `portfolio` or `demo` in the DB name.
- Password reset email flow is intentionally removed for this portfolio version.
