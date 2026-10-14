# Project Rules — Free AI Ebook Studio

1. Read this folder's README, charter, PRD, plan, and relevant workflows before coding.
2. Inspect the actual repository, scripts, schema, and dependencies; never assume.
3. Before edits, state goal, files likely to change, approach, and acceptance checks.
4. Make focused, reviewable changes; preserve unrelated working behavior.
5. Never claim tests, deployments, or features succeeded unless verified. Mark unrun checks as “not run.”
6. Never delete tests or weaken validation just to get a pass.
7. Keep API keys, tokens, and service-role secrets out of source control and browser bundles.
8. Enforce authorization on the server/database, not only in UI.
9. Validate inputs at trust boundaries and render user/AI text safely.
10. Never silently overwrite user-authored text with regenerated AI content; provide compare/confirm/undo.
11. Put provider-specific logic behind an adapter; keep manual editing/export usable without AI.
12. No payments, subscriptions, credit balances, or paywalls in the initial release.
13. Do not promise unlimited generation until real quotas and costs are verified.
14. Minimize personal data; do not send manuscript content to analytics.
15. Use accessible semantic controls, visible focus, readable contrast, and mobile-friendly touch targets.
16. Use documented migrations for database changes; preserve recovery options.
17. Add/update tests for changed behavior; run relevant tests, lint, typecheck, and build.
18. Review the final diff for accidental deletions, secret leaks, unsafe rendering, and dependency bloat.
19. Keep setup and environment configuration documented; never invent commands or env vars.
20. End each task with changed files, behavior, actual checks/results, limitations, risks, and next step.

## AI writing/research
Treat generated text as draft material. Do not fabricate sources, quotations, or statistics. Preserve language, audience, tone, outline, and terminology. Make long-running generation status, failure, and retry understandable. Preserve existing text until a user accepts a revision.
