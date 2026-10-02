# Daulat Ram College Voicebox

Anonymous complaint & suggestion box for the Daulat Ram College Students'
Union. Static frontend in `public/`, three serverless API routes in `api/`,
shared auth helper in `lib/`, and data stored in Upstash Redis.

- **Tracking code format:** `DRC-XXXXXX` (6 chars from `A–Z`, `2–9`, minus ambiguous letters)
- **Redis namespace:** `du:drc:voicebox` (all keys live under this prefix)
- **Admin auth:** password protected, session tokens in Redis (12h TTL), never stored in the browser

## Deploy in 5 steps

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "drc-voicebox"
git branch -M main
git remote add origin https://github.com/anubhavbajpaibusiness/daulat-ram-opress.git
git push -u origin main