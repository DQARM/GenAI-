# CLAUDE.md

> Sanitized external-sharing copy. Company identifiers, internal deck names,
> exact version fingerprints, review status, and private conversation-link
> locations have been generalized or removed.

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Kept deliberately lean (Claude 5 context-engineering rules): only current state and non-obvious gotchas live here. Folder roles and workflow are defined by the ref2pptx SKILL and are not repeated here. Long-form details are split out; read them on demand:

- **HISTORY.md** — record of changes, rationale, review verdicts, and archived decisions. Check it before changing a past decision involving sources, wording, or page structure.
- **40_Scripts/README.md** — build chain, template layouts, geometry/autofit/footer specifications, and script-editing gotchas. **Read it before editing anything in `40_Scripts/` or touching layout.**
- **51_Revised/vXX_YYYYMMDD/LOG.md** — external-review classification and user decisions for each revision round.

## What This Is

A **ref2pptx** project. Say `用 ref2pptx 處理這個專案` to trigger the skill.

## Current State

- **Deck**: `30_Output/training_deck_current.pptx` — current Chinese-language training deck. Exact title, page counts, chapter counts, delivery format, and revision history are intentionally omitted from this share-safe copy.
- **Fingerprints**: internal outline, audience, skill, and build hashes are intentionally omitted. Template: `00_Masters/corporate_template_16x9.pptx`.
- **Build**: use the current generation and QA scripts documented in `40_Scripts/README.md`.
- **Pending**: consult the private `HISTORY.md` and reviewer logs. Internal review labels, unreleased assets, company templates, and user-specific decisions are intentionally omitted here.

## Gotchas (non-obvious; read before editing content)

- **OUTLINE tail**: bare `##` headings after the「其他」idea-dump section are idea notes, not chapters.
- **Re-hash OUTLINE.md immediately before copying to OUTLINE.used.md** — the copy overwrites the old snapshot; if the hash changes mid-run, the diff baseline is lost.
- **Punctuation is per-page style and may be mixed**: legacy cover/section/reference strings can use fullwidth punctuation, while newer body bullets can use halfwidth punctuation with limited established exceptions. Match the exact page style; do not normalize the entire deck from OUTLINE punctuation, and keep English quotation marks halfwidth.
- **Panel edits**: `spec["panel"]` flows into speaker notes through an idempotent post-pass. When re-editing an existing panel, strip the stale notes copy first with `_drop_stale_panel_notes()`; see `40_Scripts/README.md`.
- **Established translations**: assertion = **斷言**, oracle = **判準**（裁判比喻）, fail → **不放行／驗不到** in body text. Reuse these terms rather than creating alternatives.
- **「你」rule**: avoid direct「你」in body text. Any intentional quoted exception must be preserved exactly as recorded in the private project history.
- **Unverified numbers**: never state figures that cannot be sourced.
- **Source citations**: source URL files in adopted reference folders render as a small source line above the progress bar; OUTLINE「來源:」lines are also page sources rather than body text. Preserve any explicitly approved source substitutions. **Do not publish private AI-conversation share links; replace them with public sources or remove them before external sharing.**
- **Same-name practices**: where two practices share the same abbreviation, keep their meanings distinct. Preserve established commercial and research mappings recorded in the private project history.
- **Image-page precedent**: an image page immediately after its topic content page is an annex, with the panel remaining on the content page. For in-chapter industry examples, place the image page first and the continuation content page with its panel afterward.
- **Mindmap precedent**: new topics do not always need a mindmap node. When a branch stack is full, re-space the layout before adding another node; the QA script must remain the source of truth for overflow checks.
- **Intentional cross-chapter placement**: some related material may deliberately remain in different chapters for historical or structural reasons. Do not unify or move it without checking the private project history and updating all cross-references.

## Repo notes not derivable from the SKILL

- `20_References/` contains adopted source folders. Some private reference folders may contain AI-conversation share links; those links and their exact folder locations are intentionally omitted from this external-sharing copy.
- Root `OUTLINE_example.md` is a user demonstration file and is not part of the main deck pipeline. Do not regenerate removed demonstration output unless explicitly requested.
- `90_Excluded/` also serves as the archive for old versions, scripts, and reports. Never delete archived material; move it into the archive.
- Legacy generation scripts that are still imported by the current chain must not be archived; see `40_Scripts/README.md`.
