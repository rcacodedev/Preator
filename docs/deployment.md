# Deployment

PREATOR is deployed as a multi-surface SaaS product rather than as a single static application.

## Deployment model

### Backend API
The backend is deployed independently and is responsible for business logic, persistence, billing coordination, background jobs and integrations.

### Frontend application
The authenticated product UI is deployed separately from the backend and consumes its API.

### Public website
The public website is deployed as an independent surface focused on communication, positioning, pricing and onboarding.

## Supporting infrastructure

At a high level, the platform uses services such as:

- backend hosting
- frontend/public web hosting
- PostgreSQL
- Redis / worker infrastructure
- Stripe
- email/provider services

## Operational approach

PREATOR is handled as a real product deployment, which means operational work includes:

- environment configuration
- deployment validation
- billing flow verification
- smoke checks
- post-update review
- service health checks

Specific production scripts, infrastructure paths, private operational setup and sensitive configuration are intentionally excluded from this public repository.
