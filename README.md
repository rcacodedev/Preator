# PREATOR

**PREATOR** is a production-oriented business management SaaS built to centralize day-to-day operations in a single online system.

It brings together inventory, purchasing, sales, agenda, analytics, integrations and billing into one coherent product experience.

**Website:** [preator.es](https://preator.es)

---

## What this repository is

This repository is a **public showcase** for PREATOR.

Its purpose is to explain:

- what the product is
- what business areas it covers
- what technical stack supports it
- how the platform is structured at a high level
- what kind of product and architecture work has been built

This repository **does not include the private source code** of PREATOR.

---

## Product overview

PREATOR is designed as a serious online management tool rather than a collection of disconnected admin screens.

The product is built around operational coherence across multiple business areas:

- stock and product structure
- purchasing workflows
- sales and financial document flows
- agenda and reminders
- KPI visibility
- integrations and webhook groundwork
- subscription billing and organization settings

The goal is to provide a practical system that helps teams manage operations with more structure, visibility and continuity.

---

## Main product areas

### Home / Cockpit
A central operational summary layer focused on visibility, priorities and quick actions.

### Inventory
Stock visibility, product structure, movement context, warehouses and related organization.

### Purchases
Purchase orders, receipts, supplier-side flows and operational purchasing control.

### Sales & Finance
Quotes, delivery notes, invoices and financially relevant document workflows.

### Agenda
Calendar-oriented operational planning, reminders and time-based business visibility.

### KPIs / Analytics
Structured business metrics and operational insight.

### Integrations
Webhook-based connectivity groundwork and external integration patterns.

### Billing & Settings
Plan visibility, subscription management, organization settings and team-related configuration.

---

## Technical stack

### Backend
- Python
- Django
- Django REST Framework
- PostgreSQL
- Redis + RQ
- Stripe

### Frontend application
- React
- Vite
- Tailwind CSS

### Public website
- Next.js

### Deployment
- Hetzner
- Vercel

---

## High-level architecture

PREATOR is structured as three main surfaces:

1. **Backend API**
   - business logic
   - authentication
   - billing coordination
   - operational modules
   - background jobs and integrations

2. **Frontend application**
   - authenticated product UI
   - module workflows
   - settings and billing UX
   - operational navigation

3. **Public website**
   - positioning
   - pricing
   - onboarding entry flow
   - product communication

Supporting services include PostgreSQL, Redis/RQ, Stripe and external provider infrastructure.

More detail is available in [`docs/architecture.md`](docs/architecture.md).

---

## Screenshots

Screenshots will be added progressively to this repository.

Planned set:

- public home
- pricing
- dashboard / cockpit
- inventory
- purchases
- sales / finance
- billing / settings

Assets live in:

- [`assets/screenshots/`](assets/screenshots/)

---

## Documentation

Additional project overview:

- [Overview](docs/overview.md)
- [Modules](docs/modules.md)
- [Architecture](docs/architecture.md)
- [Deployment](docs/deployment.md)
- [Roadmap](docs/roadmap.md)

---

## Current status

PREATOR is an active product project with:

- a public-facing website
- a production-oriented backend and frontend architecture
- subscription billing
- operational product modules
- ongoing product hardening and evolution

This public repository is maintained as a **product and architecture showcase**, not as an open-source release.

---

## Rights and ownership

All product rights, branding and implementation rights related to PREATOR are reserved by the author.

This repository is provided for informational and showcase purposes only.  
No private product source code is published here.

---

## Author

Built by **Rafael Cuevas**.

For public product context, visit [preator.es](https://preator.es).
