# Architecture

PREATOR is structured as a real SaaS product with clearly separated surfaces for backend, authenticated application and public website.

## Main layers

### 1. Backend API

The backend acts as the source of business logic and system coordination.

Responsibilities include:

- domain logic
- authentication and authorization
- billing coordination
- persistence and data access
- asynchronous work
- integration entry points

Main technologies:

- Django
- Django REST Framework
- PostgreSQL
- Redis + RQ
- Stripe

### 2. Frontend application

The authenticated app is a separate frontend layer dedicated to product workflows and day-to-day user interaction.

Responsibilities include:

- operational navigation
- module UX
- settings and billing UI
- product-level workflow execution

Main technologies:

- React
- Vite
- Tailwind CSS

### 3. Public website

The public website is intentionally separated from the product app so that communication, positioning, pricing and onboarding can evolve independently.

Responsibilities include:

- public product presentation
- pricing communication
- trial/onboarding entry
- brand and positioning layer

Main technology:

- Next.js

## Supporting services

At a high level, PREATOR also relies on supporting infrastructure such as:

- PostgreSQL
- Redis / background workers
- Stripe
- hosting and deployment services
- email/provider infrastructure

## Architectural intent

This split is deliberate.

It allows:

- the backend to remain the center of logic
- the product app to focus on authenticated operational UX
- the public website to focus on communication and onboarding
- billing and integrations to stay centralized in the application core

The result is a more serious SaaS structure than a single undifferentiated codebase handling every concern in the same layer.
