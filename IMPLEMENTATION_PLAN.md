# Implementation Plan — Free AI Ebook Studio

Ship vertical slices; do not advance until acceptance checks pass or remaining risks are recorded.

## Phase 0 — Audit and architecture
Inspect repository and agent/hosting options; document stack decision, architecture, data flows, env vars, free-tier assumptions, and run/test commands. Confirm secrets strategy and deployment compatibility.

## Phase 1 — App shell
Mobile-first navigation, dashboard, project list/create form, design tokens, accessible components, empty/loading/error states. Verify narrow-screen layout, keyboard use, lint/typecheck/build.

## Phase 2 — Persistence
Schema/migrations, project and chapter CRUD, stable ordering, save status, reopen after refresh, authorization if accounts exist. Test data isolation and failure recovery.

## Phase 3 — Outline studio
Outline suggestion adapter, manual outline, add/edit/remove/reorder. Confirm generation failure does not erase content and order persists.

## Phase 4 — Writing studio
Chapter editor, context assembly, per-chapter generation, progress/retry, compare/confirm replacement. Test manual mode, retries, context consistency, and preservation of original text.

## Phase 5 — Preview and exports
Preview renderer plus PDF/DOCX/EPUB generation, metadata and table of contents. Validate EPUB structure; inspect PDF clipping/page breaks; open DOCX; test special characters and chapter order.

## Phase 6 — Cover and revision tools
Cover upload/basic customization first; optional generation only after cost/provider review. Selected-text revisions with diff/undo. Validate uploads and graceful provider failure.

## Phase 7 — Research and quality
Source-aware research, reference list, checkpoints/recovery, word count, optional import. Verify citations are inspectable and recovery works.

## Phase 8 — Hardening and release
Cross-device QA, security review, performance/accessibility pass, deployment and limitation docs. No unresolved critical/high issues; release smoke tests pass.

## Priority
Reliable project lifecycle, outline, editor, persistence, and exports before decorative polish or speculative features.
