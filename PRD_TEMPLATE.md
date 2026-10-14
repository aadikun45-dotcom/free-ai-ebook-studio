# Product Requirements — Free AI Ebook Studio

**Status:** Initial baseline | **Direction:** Advanced ebook studio | **Pricing:** Free to users | **UX:** Mobile-first responsive web

## Problem and solution
Users need one workspace to structure a book, maintain chapter consistency, revise drafts, design a cover, and export a properly formatted ebook. Provide these tools without a subscription or credit paywall; AI assists but never removes user control.

## P0 requirements
### Project lifecycle
Users can create, rename, duplicate, delete, save, and reopen projects. Metadata includes title/working title, audience, purpose, language, and style. Show clear empty/loading/saving/error states.

### Outline
Generate a suggested outline; allow add/edit/remove/reorder; require user approval before bulk drafting. Manual outline remains available if AI fails. Changes persist with stable chapter order.

### Writing
Manual editing works without an AI provider. AI drafts chapters using the book brief, outline, and relevant prior context. Show progress and handle timeout, malformed output, quota, and retry. Never silently overwrite edits; compare and explicitly accept replacements.

### Preview and export
Preview book structure before export. PDF, DOCX, and EPUB must preserve title, chapter order, heading hierarchy, and supported metadata. Validate EPUB structure; inspect PDF for clipping/page breaks; confirm DOCX opens. Export failure must not lose project data.

## P1 requirements
Cover upload and basic customization; optional image generation only if a suitable free provider is verified. Selected-text rewrite/expand/simplify/proofread with diff and undo. Research references with source URL/title/access date and no fabricated citations.

## P2 requirements
Version checkpoints/recovery, word count, keyboard shortcuts, Markdown/text import if justified.

## Non-functional
Responsive from narrow Android screens to desktop; accessible keyboard flow; server-side authorization; safe rendering; input/file validation; protected secrets; understandable provider errors; minimal data collection; maintainable dependencies.

## Free-to-user constraint
No payment wall, paid tier, subscription, or credits. Document third-party quotas and potential operator costs. If free AI cannot be guaranteed, explain limits honestly and keep manual editing/export available.

## Suggested entities
BookProject, Chapter, Asset, SourceReference, RevisionCheckpoint, and optional User/account. Choose a normalized schema with migrations and ownership rules; avoid redundant state.

## Out of scope
Payments, credit wallets, automatic marketplace publishing, native apps, and claims of unlimited AI generation.

## Release acceptance
P0 flows pass on mobile; persistence and access isolation verified; exports tested in appropriate readers/validators; critical/high security issues resolved; setup and limits documented.
