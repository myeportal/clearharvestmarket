# Clear Harvest Market Admin + Marketing Package

This package adds a lightweight but real operator backend structure for Clear Harvest Market.

## Roles

### Superadmin
Reserved for Founding Father only.

Capabilities:
- manage env keys and secrets
- approve or deny automation channels
- override payment routing
- create or retire marketing agents
- change global strategy and offer structure
- view all flows and lead classes

### Admin
Reserved for the owner.

Capabilities:
- run approved campaigns
- manage content queue
- review and route leads
- update offer pages and landing copy
- use approved automation workflows
- no direct access to master secrets

## Pages
- `/admin/` — owner dashboard
- `/superadmin/` — top-level control console

## Config
- `config/marketing-package.json`

## API routes
- `api/admin-status.js` — reads current package config for dashboards
- `api/admin-session.js` — simple role check scaffold using env keys
- `api/marketing-command.js` — action router for marketing workflow calls
- `api/lead-intake.js` — lead classification and funnel recommendation scaffold

## Recommended env vars
- `SUPERADMIN_KEY`
- `ADMIN_KEY`
- `STRIPE_SECRET_KEY`
- `STRIPE_SUCCESS_URL`
- `STRIPE_CANCEL_URL`
- `RESEND_API_KEY`
- `ORDER_FROM_EMAIL`
- `ORDER_TEAM_EMAIL`
- `NEWSLETTER_FROM_EMAIL`
- `PARTNER_FROM_EMAIL`
- `PARTNER_TEAM_EMAIL`

## Included agent model
- SEO Agent
- Video Agent
- Autopost Agent
- Lead Gen Agent
- Funnel Agent
- Payments Agent

## Suggested workflow map
1. SEO / social / video content creates intent
2. Intent enters a lead form or offer page
3. `lead-intake` classifies the lead
4. Lead is routed to the correct funnel
5. Funnel routes to Hotplate or Stripe depending on offer type
6. Follow-up email, upsell, or repeat-offer logic continues the relationship

## Security recommendation
Keep this package approval-first. Drafts and planning can be automated aggressively. Publishing, paid media, and external sending should stay superadmin-approved unless intentionally loosened later.
