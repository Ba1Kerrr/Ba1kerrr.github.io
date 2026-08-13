# SoulMates Landing Page

Marketing site for SoulMates, an ML-matched dating platform with a couples ecosystem. This repo is one of three; the other two (backend/web app, mobile app) are private, so their scope is summarized below instead of linked.

**Author:** Ba1Kerrr

## The three repos

**Backend/web** (private) — Python/FastAPI backend and React web client, in production. ML-ranked feed (LightGBM), real-time chat over WebSocket, WebRTC video calls, a couples ecosystem (shared timeline, budget, challenges), subscriptions and micropayments, admin panel with moderation and CRM tooling. 330+ backend tests, Docker Compose deployment.

**Mobile** (private) — Flutter client covering auth, profile, swipe feed, chat, and subscription screens, building successfully in CI for Android. Its API client still targets an earlier backend endpoint layout and does not yet talk to the live API — UI is ahead of integration.

**This repo** — the public-facing static site described below.

## What this is

Plain HTML/CSS, no build step, no framework. Five pages:

| Page | Content |
|------|---------|
| `index.html` | Landing page — hero, core pitch, feature highlights |
| `features.html` | Full feature breakdown |
| `couples.html` | Couples ecosystem pitch |
| `screenshots.html` | Product screenshots |
| `faq.html` | FAQ |

Shared styling in `style.css`, shared nav/footer markup repeated per page (no templating).

## Running locally

```bash
python -m http.server 5599
```

Then open `http://localhost:5599`.

## Deployment

`.github/workflows/deploy.yml` publishes the repo root to GitHub Pages on every push to `main`.

## License

Proprietary. Not licensed for redistribution.
