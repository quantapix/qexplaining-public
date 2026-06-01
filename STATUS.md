# qexplaining-public — status

_Snapshot: 2026-06-01. Refreshed weekly (Fridays) during the
2026-06-01 → 2026-12-01 drive window._

Release-narrative status of the 50-video explainer arc (5 topics × 10
subjects). Companion to the [README](./README.md), whose rolling
`Status — <date>` log carries the per-week detail; this file is the
consolidated current snapshot.

## Overall

**In production.** The master plan (all 50 subjects, profile-area tagged,
in shootable order) is locked; the per-episode production pipeline is
operational; the first sprint cohort plus a second cohort of scripts are
authored. The output of the work is **scripts + the data behind every
graphic** — rendering, voice, and finishing run in separate pipelines.

## Pipeline

- **A-roll** — an AI presenter (a trained photo-avatar set, rotated per
  beat-archetype) over a locked voice; per-beat generation (one clip +
  caption track per script beat per aspect) for cheaper re-cuts and tighter
  lipsync.
- **B-roll** — programmatic, React-based components rendered to a
  high-quality intermediate, with brand tokens read from a generated
  module so no raw values leak into renders; plus a Geometry-Nodes
  background-plate lane for the recursive-tessellation motifs.
- **Composition + finishing** — a scripted non-linear-editor session via an
  in-house Python wrapper + a recipe library, now a per-phase pipeline under
  a multi-phase operator runsheet, each phase ending in an explicit playback
  gate.
- **Captions + loudness** — captions are typeset from the already-correct
  script caption track (so technical terms are exact by construction, not
  transcribed), and loudness is normalized deterministically to the
  voice-content target.

## What landed recently

- **qreel shipped to main** — a one-command bake tool (`/reel <bundle>`)
  that collapses the multi-step finishing pass (assemble → caption → render
  → loudness) behind a single command driving a running editor session and
  handing back one normalized MP4. Two input modes (a full episode
  directory, or a minimal standalone bundle), auto-detected. The
  episode-side callers are reconciled to the shipped API.
- **Production-phasing** — the earlier monolithic per-episode driver is
  retired channel-wide in favor of a per-phase pipeline + a 12-phase
  operator runsheet.
- **Cohort-2 scripts** — the next block of subjects authored (script +
  design), extending the layered-scaffolding pipeline beyond the first
  sprint cohort.

## Next

- First end-to-end `/reel` bake of a standalone bundle against a live editor
  session.
- Carry the per-episode pipeline across the cohort-2 scripts; ship the first
  sprint cohort to the channel.

## How to verify

- The master plan + every authored script lands in this repo as ordinary
  diffs; the commit log is the change record.
- Finished videos publish to the channel; the public surface refreshes
  weekly.
