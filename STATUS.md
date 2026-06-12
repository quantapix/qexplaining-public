# qexplaining-public — status

_Snapshot: 2026-06-12. Refreshed weekly (Fridays) during the
2026-06-01 → 2026-12-01 drive window._

Release-narrative status of the 50-video explainer arc (5 topics × 10
subjects). Companion to the [README](./README.md), whose rolling
`Status — <date>` log carries the per-week detail; this file is the
consolidated current snapshot.

## Overall

**Live.** The channel's first two episodes are public — 1.1 "The
hallucination tax" (2026-06-09) and 1.5 "Negative verification"
(2026-06-11) — on YouTube (<https://www.youtube.com/@Quantapix>) and the
channel CDN. The full roster, live and upcoming, renders at
<https://quantapix.com/videos>. The master plan (all 50 subjects,
profile-area tagged, in shootable order) is locked; the per-episode
production pipeline is operational and has now reproduced the first four
episodes end-to-end from scratch.

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
  in-house Python wrapper + a recipe library, a per-phase pipeline under a
  multi-phase operator runsheet. Presenter-corner decoration runs two
  lanes: a default headless lane that bakes the picture-in-picture
  element, wipes, and chrome off the editor as transparent alpha
  intermediates (leak-safe by construction), and a staging lane that keeps
  the rich node-tree comps for interactive delivery; both read one layout
  sidecar so they can't diverge.
- **Captions + loudness** — captions are typeset from the already-correct
  script caption track (so technical terms are exact by construction, not
  transcribed), and loudness is normalized deterministically to the
  voice-content target.

## What landed recently

- **Two episodes shipped public** — 1.1 (2026-06-09) and 1.5 (2026-06-11),
  each with a YouTube leg and an immutable CDN cut, recomputed chapters,
  a branded outro plate, and a normalized master.
- **The /videos roster page** — the full 5×10 plan with live/upcoming
  states, watch links, and thumbnails, published as a JSON roster consumed
  by the site at build time.
- **Freeze-at-gap wipes** — muted speech handles no longer play as silent
  talking during wipe transitions; segments outside a clip's content span
  render held frames.
- **Operator content marks** — per-take unfreeze/freeze source frames from
  an operator scrub override the acoustic content spans (which freeze the
  presenter mid-blink), with the audio timing clock bit-identical.
- **Branded outro + channel bed** — a 20-second raster end-screen plate
  with the next episode's tile, and a seamless low-alpha background loop
  composited automatically.

## Next

- Finish 1.7 (Civil RICO walkthrough) and 2.1 through the same pipeline;
  both already carry the wipe layout and segmented caption bake.
- Shorts pickup lane for the live episodes.

## How to verify

- Watch the live episodes: the channel at
  <https://www.youtube.com/@Quantapix>, or the CDN cuts linked from
  <https://quantapix.com/videos>.
- The master plan + every authored script lands in this repo as ordinary
  diffs; the commit log is the change record.
