# QA and Security Checklist — Free AI Ebook Studio

Mark each item Pass, Fail, N/A, or Not Run; do not mark Pass without evidence.

## Core functionality
- [ ] Create, rename, duplicate, and delete projects.
- [ ] Save, refresh, and reopen content without loss.
- [ ] Add/edit/remove/reorder chapters; order remains stable.
- [ ] Manual writing/editing works without AI.
- [ ] AI generation shows progress and handles errors/retry.
- [ ] Regeneration never silently overwrites user edits.
- [ ] Preview reflects current content.
- [ ] PDF is readable and ordinary text is not clipped.
- [ ] DOCX opens and preserves headings/order.
- [ ] EPUB passes structural validation and opens in a compatible reader.
- [ ] Cover/provider failure does not block writing/export.
- [ ] Empty/loading/saving/offline/error states are understandable.

## Mobile and accessibility
- [ ] Test narrow Android and desktop viewports.
- [ ] No unintended horizontal overflow or clipped controls.
- [ ] Touch targets, labels, focus, contrast, and text scaling are usable.
- [ ] Keyboard navigation and dialogs/menus work.

## Security and privacy
- [ ] No secrets/tokens/service-role keys in repository or client bundle.
- [ ] Server/database authorization protects projects and assets.
- [ ] Cross-user ID tampering does not expose or change data.
- [ ] Validate inputs and render authored/generated text safely.
- [ ] Uploads validate size/type and access permissions.
- [ ] Rate-limit public/expensive endpoints as appropriate.
- [ ] Logs/analytics exclude secrets and unnecessary manuscript content.
- [ ] Data deletion/retention expectations are documented.
- [ ] Dependencies/lockfile reviewed; critical/high vulnerabilities resolved or mitigated.

## AI reliability
- [ ] Provider secrets are server-side only.
- [ ] Adapter handles timeout, quota, malformed output, and unavailable service.
- [ ] Generated content is validated before saving.
- [ ] Research references are traceable; no fabricated citations.
- [ ] Retries/long outputs do not duplicate or corrupt content.
- [ ] Users can reject AI revisions and recover originals.

## Free-to-user
- [ ] No subscriptions, payments, credit wallets, or paywalls.
- [ ] Third-party quotas and limits are documented.
- [ ] No mandatory paid AI dependency for basic editing/export.
- [ ] Clear behavior when free provider quotas are exhausted.

## Evidence
- Commit SHA:
- Build:
- Lint/typecheck/tests:
- Export validation:
- Mobile/browser coverage:
- Open defects/mitigations:
- Reviewer/date:
