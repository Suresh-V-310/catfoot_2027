# ARCHITECTURE

HackFlow MVP uses a static web client served by Nginx in Docker.

Browser
  -> HackFlow UI
  -> localStorage data layer
  -> dashboard / events / teams / submissions / judging / leaderboard / gallery / audit

The deployment is intentionally self-contained. `docker compose up` starts the portal locally.

Production extension:
- React/Vite frontend
- Node/Express API
- SQLite/PostgreSQL
- server-side sessions/JWT
- REST API and OpenAPI
- persistent audit log
