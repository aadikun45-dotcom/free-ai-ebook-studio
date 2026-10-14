# Free AI Ebook Studio

An advanced, mobile-first ebook creation platform inspired by modern AI ebook workflows, with original branding and implementation.

## Locked decisions
- Product direction: advanced studio (A2).
- Pricing: free to users; no subscriptions, credits, payment walls, or billing in the initial product (B3).
- Coding agent: choose the most capable compatible agent with practical free access; remain agent-agnostic.
- Source of truth: GitHub.
- UX: mobile-first responsive web app, including desktop support.
- Proposed stack: React + TypeScript, accessible UI, PostgreSQL persistence, and a replaceable AI-provider adapter. Confirm stack against the selected host before implementation.

## Core journey
Create project → generate/edit outline → draft chapters with book context → revise content → design/upload cover → preview → export PDF/DOCX/EPUB → save and reopen.

## Documentation
- PROJECT_CHARTER.md — vision, scope, constraints, success.
- PROJECT_RULES.md — engineering and agent rules.
- PRD_TEMPLATE.md — project-specific product requirements.
- IMPLEMENTATION_PLAN.md — staged delivery.
- BUG_REPORT.md — issue template.
- FEATURE_WORKFLOW.md — idea-to-tested-feature.
- RELEASE_WORKFLOW.md — release and deployment.
- QA_SECURITY_CHECKLIST.md — release gates.

## Free means free to users
Prefer open-source components and free tiers, and document quotas, hosting/storage limits, and potential operator costs. Never claim unlimited AI generation or zero operating cost without verification. Manual editing and export must remain useful if AI is unavailable.

## Status
Planning/documentation stage. Do not claim features are implemented until verified in code.

## Required loop
Define requirements → plan → implement a small slice → review diff → test → security/QA check → checkpoint → report actual results.
