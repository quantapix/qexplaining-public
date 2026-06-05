# qexplaining-public — status

_Snapshot: 2026-06-05. Refreshed weekly (Fridays) during the
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

- **Caption track no longer leaks** — captions are baked into short
  transparent intermediate overlays and tiled onto a fresh top track instead
  of being hosted on a presenter take, which had leaked its source full-frame
  at render. One caption file now serves both as the upload sidecar and the
  bake source, so on-screen and uploaded captions can't drift.
- **PIP wipe-transition** — the presenter corner stays continuously filled
  between beats by overlapping adjacent takes on two tracks and wiping between
  them, hosted on picture-in-picture clips so it's leak-safe; this retires the
  earlier parked gap-holder approach.
- **Phrase-anchored re-timing** — per-beat takes carry a trailing-silence
  handle for clean overlaps, and cue timings re-anchor to narrated phrase
  boundaries rather than segment indices (re-renders re-segment). Wired across
  the first four episodes.
- **qreel shipped to main** — a one-command bake tool that collapses the
  multi-step finishing pass (assemble → caption → render → loudness) behind a
  single command driving a running editor session and handing back one
  normalized MP4; two input modes (a full episode directory, or a minimal
  standalone bundle), auto-detected; episode-side callers reconciled to the
  shipped API.
- **Production-phasing** — the earlier monolithic per-episode driver is
  retired channel-wide in favor of a per-phase pipeline + a multi-phase
  operator runsheet, each phase ending in an explicit playback gate.

## Next

- First end-to-end finishing run on the pilot with the new caption bake and
  wipe-transition in place.
- Carry the per-beat re-timing pipeline across the second cohort of scripts;
  ship the first sprint cohort to the channel.

## How to verify

- The master plan + every authored script lands in this repo as ordinary
  diffs; the commit log is the change record.
- Finished videos publish to the channel; the public surface refreshes
  weekly.
