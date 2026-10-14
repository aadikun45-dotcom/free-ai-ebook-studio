# Feature Workflow — Free AI Ebook Studio

## 1. Clarify
State user problem, target user, expected outcome, scope, and observable success. Check charter and PRD. Resolve ambiguities that affect data safety, cost, architecture, or user-visible behavior.

## 2. Inspect
Read project rules and relevant docs. Inspect real files, scripts, dependencies, schema, and tests. Identify reuse and regression risks.

## 3. Specify
Write acceptance criteria covering success, loading, empty, failure, retry, cancellation, and mobile states as applicable. Define persistence, authorization, and data migration behavior. For AI features define context, output validation, provider failures, and user approval before replacement. Preserve free-to-user constraints.

## 4. Plan
List files/components/schema changes, smallest coherent steps, dependencies, environment variables, tests, and rollback/recovery concerns.

## 5. Implement
Make focused changes. Keep provider-specific logic behind adapters. Never expose secrets client-side. Use migrations for persistent schema changes. Preserve user content on failures and regeneration. Provide accessible status/error messages.

## 6. Verify
Run relevant available unit/integration tests, lint, typecheck, production build, mobile viewport checks, access-isolation checks, and export validation. Report actual results and explicitly mark unrun checks.

## 7. Review
Inspect full diff for regressions, accidental deletions, unsafe rendering, missing validation, secret leaks, redundant logic, and dependency bloat. Fix failed acceptance criteria before proceeding.

## 8. Checkpoint and report
Commit a coherent state where repository access allows. Report changed files, behavior, tests/results, limitations, risks, and next step.

## Definition of done
Acceptance criteria verified; relevant checks run; failures handled; user data protected; known limitations documented. A successful build alone does not prove a feature works.
