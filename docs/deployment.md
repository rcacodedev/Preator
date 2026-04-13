# Deployment

PREATOR is deployed as a multi-surface SaaS product with separate concerns for backend, authenticated frontend and public web.

## High-level deployment model

### Backend
The backend API is deployed separately and is responsible for application logic, persistence, billing coordination and integrations.

### Frontend application
The authenticated app is deployed independently from the backend and consumes its API.

### Public website
The public website is deployed as its own surface, focused on product communication, pricing and onboarding.

## Infrastructure

At a high level, the platform uses:

- backend hosting
- public web/app hosting
- PostgreSQL
- Redis/RQ
- Stripe
- email/provider infrastructure

## Operational approach

The project is handled as a product deployment rather than as a static portfolio app.

This means deployment work includes concerns such as:

- environment configuration
- subscription flow validation
- operational smoke checks
- post-update verification
- service health review

Specific production scripts, infrastructure details and private operational configuration are intentionally not included in this public repository.
