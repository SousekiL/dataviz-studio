# CLAUDE.md

Guidance for Claude Code in this workspace. The full local agent rules live in `AGENTS.md` (local only, not published) and are imported below; they take precedence over anything summarized here.

@AGENTS.md

## Two layers: local workspace vs. public repository

- The local folder is a working studio of ~30 data-visualization projects (code, contracts, raw data, Blender scenes, frames, videos).
- The GitHub repository is a **portfolio only**. `.gitignore` is an allow-list: `/*` is ignored and only `.gitignore`, `README.md`, `README.zh-CN.md`, `CLAUDE.md`, `PUBLIC_WORKS_MANIFEST.md`, `LICENSE` and `public-works/**` are tracked.
- Never un-ignore or force-add project folders, raw third-party data, scenes, frames or videos unless the user explicitly asks and the licenses permit redistribution.

## Adding a work to the public portfolio

1. Use only a delivered final named in the project's `README.md` / `STUDIO.md`; never drafts or unvalidated candidates.
2. Export a WebP web copy (quality ~88, original `1080×1920`) into `public-works/<collection>/`; do not edit the local original.
3. Add it to both `README.md` and `README.zh-CN.md` (keep the two in sync) and to `PUBLIC_WORKS_MANIFEST.md`.
4. Carry required disclosures (proxy semantics, nine-dash display-only status, third-party attribution).
5. Run `git diff --check` and confirm `git status` shows no unintended paths before committing.

## Local project map

See `LOCAL_PROJECT_INDEX.md` (local only) for the categorized index. Groupings: `building-age/` (city timelines + shared `tools/`), `population-3d/`, `lighthouses/`, terrain/hydrology projects, climate/night-light projects, demography/explainers, and article research packs.

## Working conventions

- Each project keeps its own `README.md` or `STUDIO.md` as the resume point, plus a `PIPELINE.md` (core code, inputs and re-download paths, ordered render steps, checks, environment, constraints). Update both after substantial work.
- Cleanup follows `maintenance/cleanup-*/PROPOSAL.md`: approved items are moved (same relative path) into a root `_TO_DELETE_<date>/` staging folder, because CLI trash cannot handle iCloud-evicted files; the user empties it via Finder.
- Canvas is `1080×1920` (9:16) unless the project states otherwise; bilingual (中文 / English) typography; signature @一尺之棰 / Zeno.yczc.
- Keep temporary work in `/tmp` or the session scratchpad; never render two jobs into the same frame directory.
- Do not delete, move or rename existing project files, backups or old versions without an explicit, path-specific approval.
