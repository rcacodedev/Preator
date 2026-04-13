# Architecture

PREATOR uses a separated architecture oriented to a real SaaS deployment model.

## Main layers

### 1. Backend API

The backend is responsible for:

- business logic
- authentication and authorization
- billing coordination
- data access and persistence
- asynchronous processing
- external integration points

Main technologies:
- Django
- Django REST Framework
- PostgreSQL
- Redis + RQ
- Stripe

### 2. Frontend application

The authenticated application is built as a dedicated frontend layer that consumes the backend API and organizes the user-facing workflows of the product.

Main technologies:
- React
- Vite
- Tailwind CSS

### 3. Public website

The public website is separated from the main app in order to support marketing, product positioning, pricing presentation and onboarding entry flows.

Main technology:
- Next.js

## Supporting services

The platform also relies on infrastructure and service layers such as:

- PostgreSQL for persistent product data
- Redis/RQ for background work
- Stripe for subscription billing
- hosting and deployment infrastructure
- email/provider services

## Design intent

The architecture is intentionally split so that:

- the public web can evolve independently from the app
- the app can focus on authenticated workflows
- the backend can remain the source of business logic
- operational and billing concerns stay centralized

This structure also supports a more professional product lifecycle than a single monolithic codebase used for every concern.
