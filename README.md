# Christophe Pirolley

Full-stack Python/Django developer. I design, build and operate transactional
platforms on my own: marketplaces with escrow payments, fintech platforms with
card issuing, AI agents in production.

Sofia, Bulgaria — 100% remote. French (native), English (fluent).

## What I build

### [StarShipDealers](https://www.starshipdealers.com)
Peer-to-peer marketplace with escrow-protected payments. Sole designer,
developer and operator. Live since November 2025, 600+ users, 170+ orders.

→ [Architecture case study](https://github.com/Meranhor/starshipdealers-architecture)

- 28 Django apps, ~375,000 lines of code, 92 Celery tasks, ~4,000 tests
- Multi-PSP payments (Stripe, PayPal, crypto), escrow, internal wallet and
  ledger, automated payouts with a security hold window
- MCP server exposing 29 tools over OAuth 2.1, so AI agents run day-to-day
  operations under human approval
- AI customer support: a Claude agent handles Discord tickets in FR/EN and
  drafts replies to in-app tickets
- Interconnected services: the Django app, a .NET catalog sync service and two
  Python Discord bots, over REST APIs and HMAC-signed webhooks. I specified the
  .NET service, managed the external team of 4 who delivered it, then took it
  over and refactored it
- OWASP audit across 13 attack surfaces, 2FA/WebAuthn on withdrawals, signup
  risk scoring
- Migrated production from Railway to DigitalOcean with zero downtime

`Django` `DRF` `Celery` `Redis` `PostgreSQL` `Docker` `Cloudflare` `HTMX`

### [GoldenHive](https://www.goldenhive.io)
Fintech platform: accounts, payment cards, investments and KYC. Freelance,
sole developer, 2024-2026.

→ [Architecture case study](https://github.com/Meranhor/goldenhive-architecture)

- Payment card issuing API integration, investment system (subscriptions,
  returns, withdrawals), KYC, fees and transactions
- 5 languages with an automated translation pipeline
- Infrastructure handed over to the client with zero downtime

### [NegotiNation](https://www.negotination.com)
B2B supplier price negotiation platform. Freelance, sole developer. Sold in
2026 and handed over to the buyer with zero downtime.

→ [Architecture case study](https://github.com/Meranhor/negotination-architecture)

- Card issuing integration with signed API requests
- Webhook dispatcher handling 33 event types: card lifecycle, authorizations,
  3-D Secure, Apple Pay, KYC

## Stack

| | |
|---|---|
| **Backend** | Python · Django · Django REST Framework · Celery · Redis · PostgreSQL |
| **Fintech** | Stripe · PayPal · crypto · escrow · wallet & ledger · card issuing · KYC/AML |
| **Security** | OWASP · OAuth 2.1 · JWT · 2FA/WebAuthn · CSP · rate limiting · fraud scoring |
| **Infra** | Docker · DigitalOcean · AWS · Railway · Cloudflare · GitHub Actions · Sentry · Linux |
| **AI** | Claude Code · MCP servers · LLM agents · Anthropic API |
| **Quality** | pytest · ruff · mypy · pre-commit |

## About the repositories

The code behind these platforms is private: they run in production and handle
real money. Read access on request.

## Contact

[LinkedIn](https://www.linkedin.com/in/christophe-pirolley)
