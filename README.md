# SoulMates Landing Page

SoulMates is a dating platform built on ML-ranked matching instead of an endless swipe feed, with a couples ecosystem (shared timeline, budget, challenges) for people who match. This repo is the public marketing site for it: five static pages pitching the product, not the product itself.

**Author:** Ba1Kerrr

## The product

Backend and web client (private repo): Python/FastAPI, React. ML-ranked feed (LightGBM), real-time chat over WebSocket, WebRTC video calls, the couples ecosystem, subscriptions and micropayments, admin panel with moderation and CRM tooling. In production, 330+ backend tests.

Mobile app (private repo): Flutter client covering auth, profile, swipe feed, chat, and subscription screens. Builds in CI for Android; still being wired up to the live API.

## This repo

Plain HTML/CSS, no build step, no framework.

| Page | Content |
|------|---------|
| `index.html` | Hero, core pitch, feature highlights |
| `features.html` | Full feature breakdown |
| `couples.html` | Couples ecosystem pitch |
| `screenshots.html` | Product screenshots |
| `faq.html` | FAQ |

Shared styling in `style.css`; nav and footer markup are repeated per page (no templating). Deploys to GitHub Pages on every push to `main` via `.github/workflows/deploy.yml`.

## License

Proprietary. Not licensed for redistribution.
