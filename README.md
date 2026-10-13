# JITENDAR KEWAT — PHANTOM X ULTRA

A bilingual (Hindi + English) cyber-security learning and authorized-testing platform starter.

## Important security notes
- This repository is a frontend starter, not a production-ready authenticated security service.
- Do **not** put real passwords, API keys, or secrets in frontend JavaScript.
- The demo login is intentionally disabled until a backend authentication service is configured.
- GitHub Pages can host the static frontend, but secure registration/login, admin authorization, scan history, AI, and active scanners need a backend or trusted service.
- Only test systems you own or have explicit permission to assess.

## Project structure
- `frontend/`: responsive dashboard, login/register UI, tools and learning pages.
- `backend/README.md`: requirements for the production backend.
- `tests/`: basic manual security checklist.

## Run locally
Open `frontend/index.html` in a browser, or serve the `frontend` directory using a local static web server.

## Planned production setup
1. Add a server-side authentication provider (secure password hashing, email verification, password reset, rate limiting, session cookies).
2. Enforce roles server-side: `user` and `admin`. Never trust a role supplied by browser JavaScript.
3. Add a database for users, authorized targets, scan history, audit events and learning progress.
4. Run active scans only in an isolated worker with strict target allowlists, rate limits, timeouts and audit logs.
5. Add AI or threat-intelligence APIs server-side; never expose API keys to the browser.
6. Add automated tests, dependency updates, backups and privacy/retention policies.
