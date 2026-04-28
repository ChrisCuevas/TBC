# TBC — The Breathing Cove Reference Asset Repository

Public hosting layer for AI-generation reference assets used in the production of *The Breathing Cove* (MFA short film, dir. Christian Cuevas, USC SCA, 2026).

This repo serves as the permanent URL host for character reference images, look references, and other assets cited via `--oref` and `--sref` parameters in Midjourney and similar generative pipelines. URLs from this repo (`https://raw.githubusercontent.com/ChrisCuevas/TBC/main/<path>`) are stable for the lifetime of the repo and branch — no expiry.

## Canonical project location

The full project (script, specs, pipeline, deliverables) lives in a separate Drive folder. This repo is the *publishing layer* for assets that need internet-accessible URLs. The canonical AI specs (`_AI/characters/*`, `_AI/looks/*`) and the central catalog (`_AI/_oref_catalog.md`) reference URLs that resolve here.

## Repo structure

- `CHARACTERS/<NAME>/master/` — locked character master references (canonical face/body for `--oref`)
- `CHARACTERS/<NAME>/variations/` — variant references (alternative angles, expressions, wardrobe variants)
- `LOOKS/` — look references for `--sref` if any are promoted to hosted form
- `PROPS/` — prop references when locked

## Filename convention

`<ENTITY>_<kind>_<NNN>.<ext>` (mirrors the project's REFERENCES library convention).

Examples:
- `CHARACTERS/SELENE/master/SELENE_master_001.png`
- `CHARACTERS/DIANA/variations/DIANA_variation_003.png`

## How to add a new reference

1. Lock the image in the project's REFERENCES library (upstream of this repo).
2. The Cowork agent or operator pushes the file to the corresponding path in this repo.
3. The raw URL is `https://raw.githubusercontent.com/ChrisCuevas/TBC/main/<path>`.
4. The catalog at `_AI/_oref_catalog.md` and the corresponding character spec are updated with the new URL in the same operation.

## Privacy

Public repo. Reference images are visual development outputs. Script and other proprietary materials are not in this repo.
