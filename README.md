# PREATOR

PREATOR is a web-based business management SaaS focused on day-to-day operational control for small and medium teams.

It brings together inventory, purchasing, sales, agenda, analytics, integrations and billing in a single product designed to be practical, structured and production-oriented.

**Public website:** [preator.es](https://preator.es)

---

## What PREATOR is

PREATOR is not a template project or a UI prototype. It is a real SaaS product built around operational workflows that businesses need to manage consistently:

- stock and product structure
- purchasing flows
- sales and financial documents
- agenda and operational reminders
- analytics and KPI visibility
- integrations and webhook-based connectivity
- subscription billing and plan control

The goal is to provide a serious online tool that feels coherent across modules, not a disconnected set of screens.

---

## Product scope

PREATOR is currently structured around the following areas:

- **Home / Cockpit**: operational overview, priorities, quick access and business signals
- **Inventory**: stock visibility, movements, products, warehouses and categories
- **Purchases**: purchase orders, receipts, supplier invoices and payment-linked flows
- **Sales & Finance**: quotes, delivery notes, invoices, financial visibility and document workflows
- **Agenda**: calendar-oriented operational planning and reminders
- **KPIs / Analytics**: business metrics and operational insight
- **Integrations**: webhook endpoints, deliveries and external connectivity groundwork
- **Billing & Settings**: plans, subscription management, team and organization settings

---

## Stack

PREATOR is built with a modern SaaS-oriented stack:

### Backend
- Python
- Django
- Django REST Framework
- PostgreSQL
- Redis + RQ
- Stripe

### Frontend app
- React
- Vite
- Tailwind CSS

### Public web
- Next.js

### Deployment
- Hetzner
- Vercel

---

## Architecture at a high level

PREATOR is split into three main surfaces:

1. **Backend API**
   - domain logic
   - authentication
   - billing logic
   - operational modules
   - async jobs and integrations

2. **Frontend application**
   - authenticated product UI
   - module navigation
   - operational workflows
   - settings and billing UX

3. **Public website**
   - product positioning
   - pricing and trial flow
   - public onboarding entry points

Supporting services include PostgreSQL, Redis/RQ, Stripe and email/provider infrastructure.

More detail is available in [`docs/architecture.md`](docs/architecture.md).

---

## Why this repository exists

This repository is a **public showcase** for PREATOR.

It is intended to show:

- what the product is
- what kind of SaaS architecture and product thinking is behind it
- what modules and workflows have been built
- how the project is positioned technically and functionally

This repository **does not include the private source code** of the product.

---

## Screenshots

Screenshots and product visuals will be added in:

- [`assets/screenshots/`](assets/screenshots/)

Recommended set:
- public home
- pricing
- dashboard / cockpit
- inventory
- purchases
- sales / finance
- billing / settings

---

## Documentation

Additional documentation:

- [Overview](docs/overview.md)
- [Modules](docs/modules.md)
- [Architecture](docs/architecture.md)
- [Deployment](docs/deployment.md)
- [Roadmap](docs/roadmap.md)

---

## Current status

PREATOR is an active product project with a real public-facing website and a production-oriented application stack.

This public repository is maintained as a product and architecture showcase rather than as an open-source codebase.

---

## Author

Built by **Rafael Cuevas**.

For product context and public positioning, visit [preator.es](https://preator.es).
