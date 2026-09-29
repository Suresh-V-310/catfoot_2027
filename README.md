# HackFlow

Open-source, self-hostable hackathon submission and judging platform MVP.

## Run locally

```bash
docker compose up
```

Open http://localhost:8080

No cloud account, hosted database, authentication provider, external API, or network connection is required for the demo. Data is stored in browser localStorage.

## Demo accounts

- Organizer: organizer@hackflow.local / demo123
- Participant: participant@hackflow.local / demo123
- Judge: judge@hackflow.local / demo123

## Core flow

Organizer creates/publishes an event -> participant forms a team and submits -> judge scores -> leaderboard updates -> gallery and audit log show the lifecycle.

## Scope

This is a rapid MVP intended for a 5-hour build. It demonstrates the core product experience and local deployment. For a production submission, replace browser-local state with a backend database and enforce every permission server-side.
