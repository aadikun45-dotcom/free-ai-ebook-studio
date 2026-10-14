# Project Charter — Free AI Ebook Studio

## Purpose and vision
Build a polished web studio that helps users plan, draft, revise, format, and export ebooks without subscriptions or credit purchases.

## Target users
First-time authors, students/educators, creators making guides and workbooks, and independent writers.

## Goals
- One coherent workflow from idea to downloadable book.
- Persistent projects and editable chapter structure.
- Context-aware chapter drafting with explicit user control.
- Readable, structurally valid PDF, DOCX, and EPUB exports.
- Excellent small-screen Android usability.
- Replaceable AI and hosting integrations; minimal vendor lock-in.

## Scope
Project dashboard; book metadata; outline generation/editing/reordering; chapter editor and AI drafting/revision; cover upload/customization; preview; persistence; PDF/DOCX/EPUB export; accessible responsive UI; error/retry states.

## Non-goals for initial release
Payments, subscriptions, credit wallets, guaranteed unlimited AI, professional desktop-publishing parity, automatic marketplace publishing, native mobile apps, or copying another product's branding/assets/source code.

## Constraints
Free to users. Use open-source tools and verified free tiers where practical. Do not expose secrets client-side. Manual editing/export must work without AI. Generated content is a draft; research claims require traceable sources. Do not add external services until costs, limits, terms, and data flows are understood.

## Success criteria
- Create, edit, save, close, and reopen a project without losing content.
- Outline edits and chapter order persist.
- Generation failure/retry does not corrupt content or silently overwrite user edits.
- Exported files open in compatible readers and preserve chapter order/headings.
- Mobile and keyboard workflows remain usable.
- No unresolved critical/high security findings at release.
- No paywall or hidden paid feature in the initial product.

## Delivery
Build in small vertical slices. Each phase needs acceptance criteria, relevant tests, a checkpoint, and a status report.
