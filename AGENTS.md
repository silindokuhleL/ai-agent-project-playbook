# AGENTS.md

These instructions apply to all repos that use this playbook.

## Core Rule

Every project is an AI-assisted, production-minded portfolio system. Agents must build reusable, documented, testable systems that demonstrate real engineering skill.

## Agent Priorities

1. Keep frontend and backend responsibilities separate.
2. Use REST APIs as the integration boundary.
3. Add AI features deliberately, with clear user value.
4. Keep business logic out of controllers and frontend pages.
5. Use services, resources, traits, policies, jobs, and reusable UI components.
6. Update docs whenever architecture, APIs, data models, or flows change.
7. Test core functionality before calling work done.

## Required Reading Before Work

Before starting implementation, agents must read:

- `docs/agent-rules/agent-rules.md`
- `docs/agent-rules/branching-and-commits.md`
- `docs/agent-rules/api-contract-rules.md`
- `docs/ai/ai-system-rules.md`

Backend agents must also read:

- `docs/agent-rules/laravel-backend-rules.md`

Frontend agents must also read:

- `docs/agent-rules/nextjs-frontend-rules.md`

Testing or release work must also read:

- `docs/agent-rules/testing-rules.md`
- `docs/agent-rules/tooling-and-quality-rules.md`

## Branching Rule

Always start from `master`, pull latest changes, create a focused branch, make small commits, test, then merge only after the task is complete.

## Build Order Rule

For SaaS-style projects, build the authentication and protected app shell before core modules. Users must be able to log in as seeded roles, switch accounts or tenants where relevant, and navigate empty protected pages before billing, CRM, reporting, AI, or admin functionality is implemented.

## AI Feature Rule

Every product should include useful AI assistance, but AI must not replace core business logic, security checks, payment truth, permissions, or auditability.
