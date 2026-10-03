# CLAUDE.md

Guidance for Claude Code in this workspace. The full local agent rules live in `AGENTS.md` (local only, not published) and are imported below; they take precedence over anything summarized here.

@AGENTS.md

## Two layers: local workspace vs. public repository

- The local folder is a working studio of ~35 data-visualization projects (code, contracts, raw data, Blender scenes, frames, videos), organised by topic under `projects/<topic>/<project>/`.
- The GitHub repository is a **portfolio only**. `.gitignore` is an allow-list: `/*` is ignored and only `.gitignore`, `README.md`, `README.zh-CN.md`, `CLAUDE.md`, `PUBLIC_WORKS_MANIFEST.md` and `public-works/**` are tracked.
- Never un-ignore or force-add project folders, raw third-party data, scenes, frames or videos unless the user explicitly asks and the licenses permit redistribution.

## Adding a work to the public portfolio

1. Use only a delivered final named in the project's `README.md` / `STUDIO.md`; never drafts or unvalidated candidates.
2. Export a WebP web copy (quality ~88, original `1080×1920`) into `public-works/<collection>/`; do not edit the local original.
3. Add it to both `README.md` and `README.zh-CN.md` (keep the two in sync) and to `PUBLIC_WORKS_MANIFEST.md`.
4. Carry required disclosures (proxy semantics, nine-dash display-only status, third-party attribution).
5. Run `git diff --check` and confirm `git status` shows no unintended paths before committing.

## Local project map

See `LOCAL_PROJECT_INDEX.md` (local only) for the full catalogue, the topic definitions and the rules for adding a project. Production projects live under `projects/<topic>/<project>/`; the topics are `cities/`, `population/`, `terrain-maps/`, `climate-night-sky/`, `culture-language/`, `ai-tech/`, `shorts/` and `concepts/`. Root-level folders are infrastructure only: `public-works/` (public gallery), `tools/` (symlinks to the shared renderers whose real files live in `projects/cities/building-age/tools/`), `maintenance/` (cleanup and reorganisation logs, e.g. `reorg-2026-09-26/REPORT.md` with the move map and rollback script), `certification-evidence/`, and `_TO_DELETE_<date>/` staging. Other local-only root files: `VISUAL_REFERENCE_LIBRARY.md` (design references, not data endorsements) and `.claude/launch.json` (local preview servers). Some projects are nested git repositories with their own remotes (`projects/population/the-age-series/`, `projects/cities/city-data-visual/`, `projects/climate-night-sky/east-asia-nightlights/`); this repository's allow-list ignores them.

## Working conventions

- Each project keeps its own `README.md` or `STUDIO.md` as the resume point, plus a `PIPELINE.md` (core code, inputs and re-download paths, ordered render steps, checks, environment, constraints). Update both after substantial work.
- Cleanup follows `maintenance/cleanup-*/PROPOSAL.md`: approved items are moved (same relative path) into a root `_TO_DELETE_<date>/` staging folder, because CLI trash cannot handle iCloud-evicted files; the user empties it via Finder. Move files only with same-volume `mv` (a rename); never `cp`/`rsync` evicted files, which forces an iCloud download.
- New projects go in `projects/<topic>/<kebab-case-name>/` with a README/STUDIO and PIPELINE, plus a row in `LOCAL_PROJECT_INDEX.md`; never place a project directly at the root or in `projects/`.
- Canvas is `1080×1920` (9:16) unless the project states otherwise; bilingual (中文 / English) typography; signature @一尺之棰 / Zeno.yczc.
- Keep temporary work in `/tmp` or the session scratchpad; never render two jobs into the same frame directory.
- Do not delete, move or rename existing project files, backups or old versions without an explicit, path-specific approval.
