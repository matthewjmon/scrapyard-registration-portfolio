# Scrapyard Registration App (Portfolio Project)

Portfolio-safe adaptation of a real, paid, and deployed business application built for a local scrapyard operation.

## Live Demo
- Frontend App: `https://scrapyard-frontend-portfolio.onrender.com`
- Backend API: `https://scrapyard-backend-portfolio.onrender.com/api`

## Source Repositories
- Frontend: `https://github.com/matthewjmon/scrapyard-frontend-portfolio`
- Backend: `https://github.com/matthewjmon/scrapyard-backend-portfolio`

## Problem Context
- Intake registration was manual and time-consuming during busy periods.
- Duplicate and inconsistent entries reduced data quality.
- Record lookup and operational reporting were harder than necessary.

## Solution Delivered
- Built a secure, authenticated CRUD workflow for acquisition records.
- Standardized data capture with structured forms and server-side validation.
- Added search/sort/detail/print flows for daily operational use.
- Implemented sequential record codes for consistent traceability.

## Business Impact
- Faster registration turnaround time.
- Fewer duplicate and incomplete records.
- Better day-to-day visibility and audit readiness.

## Architecture
- Frontend: React + Vite static site on Render.
- Backend: Express + MongoDB API on Render web service.
- Auth: JWT-based session flow with protected API routes.

The frontend and backend are intentionally split into separate repos to mirror real production deployment boundaries.

## Screenshots
### Login
Focused auth entry with demo-access helpers for quick reviewer onboarding.

![Login screen](docs/screenshots/login.png)

### Dashboard
Core operations screen for searching, sorting, and managing registrations.

![Dashboard screen](docs/screenshots/dashboard.png)

### New Record Form
Structured capture flow to reduce errors and improve consistency.

![New record form](docs/screenshots/new-record-form.png)

### Record Details
Detailed view for verification and historical traceability.

![Record details view](docs/screenshots/record-details.png)

### Print View
Print-friendly output for physical filing and compliance workflows.

![Print view](docs/screenshots/print-record.png)

## Tech Stack
- Frontend: React, React Router, Axios, Bootstrap, Vite
- Backend: Node.js, Express, MongoDB (Mongoose), JWT

## Portfolio Safety Notes
- This project is sanitized for portfolio demonstration.
- No production credentials or production data are included.
