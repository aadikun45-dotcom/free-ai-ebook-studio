# Release Workflow — Free AI Ebook Studio

## Readiness
- Confirm commit and release scope.
- Verify P0 journeys and acceptance criteria.
- Review diff/dependencies.
- Complete QA/security checklist.
- Verify migrations and recovery/rollback plan.
- Check environment variables and secret handling.
- Document hosting, storage, AI, and image-provider quotas.
- Confirm no payment/credit wall or unexpected mandatory paid dependency.

## Build and test
Inspect actual project scripts first. Run available install (respect lockfile), lint, typecheck, unit/integration tests, production build, export validation, and mobile smoke tests. Do not invent commands. Record results and checks not run.

## Data and security
Apply documented migrations; verify ownership/authorization; validate upload type and size; keep secrets out of source; prevent sensitive manuscript data in logs; document deletion and retention expectations.

## Deployment
Use preview/staging where available. Smoke-test project create/save/reopen, outline edits, chapter save, and every export. Verify mobile layout and manual editing when AI is unavailable. Promote only after checks pass. Record URL, commit SHA, timestamp, and operator when available.

## Rollback
Stop promotion for data loss, security issues, or core workflow failures. Roll back application code only when safe. Do not blindly reverse destructive migrations; prefer a forward fix or documented recovery. Communicate impact and workaround.

## Release notes
Include user impact, features/fixes, known issues, migrations/config changes, actual test results, unrun checks, deployment reference, and commit SHA.

## Free-service integrity
Verify current terms and quotas before release. Do not advertise unlimited AI or zero operator cost without evidence. If a provider quota is reached, explain it clearly and retain manual writing/editing/export.
