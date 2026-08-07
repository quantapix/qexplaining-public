# qexplaining-public — status

_Snapshot: 2026-08-07. Refreshed weekly (Fridays) during the
2026-06-01 → 2026-12-01 drive window._

Release status of the 50-video explainer arc (5 topics × 10 subjects).
Companion to the [README](./README.md), whose rolling `Status — <date>` log
carries the per-week detail; this file is the consolidated current snapshot.

**Every episode is AI-narrated.** The presenter is a synthesized avatar over a
synthesized voice — not a recording of a person — and each upload carries the
platform's altered-content disclosure.

## Overall

**Live: 8 of 50.** Eight episodes are public on YouTube
(<https://www.youtube.com/@Quantapix>) and the channel CDN, spanning four of the
five topics:

| # | Subject | Topic | Public |
|---|---|---|---|
| 1.1 | The Hallucination Tax | 1 | 2026-06-09 |
| 1.5 | Negative Verification | 1 | 2026-06-11 |
| 1.7 | Civil RICO, End to End | 1 | 2026-06-13 |
| 2.1 | When a Docket and Its Record Disagree | 2 | 2026-06-14 |
| 3.1 | Backtests Lie | 3 | 2026-06-30 |
| 4.2 | TA-Lib as Ground Truth — the MACD Alignment Quirk | 4 | 2026-07-01 |
| 4.1 | The TA Bestiary — 117 Indicators | 4 | 2026-07-02 |
| 1.2 | What Semantic Search Actually Does — and What It Can't | 1 | 2026-07-12 |

The full roster, live and upcoming, renders at
<https://quantapix.com/videos>. The master plan — all 50 subjects,
profile-area tagged, in shootable order — is locked; the per-episode production
pipeline is operational and has reproduced every live episode end-to-end from
scratch.

The live table above is the authoritative count. The progress counters on the
public status page derive "rendered" from finished cuts on disk rather than from
the tracked release records, so that one figure varies with which workstation
took the snapshot; it is being re-derived from the release records.

No vertical shorts are public yet. The four launch-cohort shorts were cut,
finished, and uploaded in late June; they have been held unlisted since, pending
a decision on the shorts' ending. What holds them is the public flip, not the
upload.

## Pipeline

- **A-roll** — a generated AI presenter (a set of synthesized photo-avatars,
  rotated per beat-archetype) over a locked synthesized voice; per-beat
  generation (one clip + caption track per script beat per aspect) for cheaper
  re-cuts and tighter lipsync. The presenter is generated, not derived from a
  recording of a person.
- **B-roll** — programmatic, React-based components rendered to a high-quality
  intermediate, with brand tokens read from a generated module so no raw values
  leak into renders; plus a Geometry-Nodes background-plate lane for the
  recursive-tessellation motifs.
- **Composition + finishing** — a scripted non-linear-editor session via an
  in-house Python wrapper + a recipe library, run as a per-phase pipeline under a
  multi-phase operator runsheet. Presenter-corner decoration runs two lanes: a
  default headless lane that bakes the picture-in-picture element, wipes, and
  chrome off the editor as transparent alpha intermediates (leak-safe by
  construction), and a staging lane that keeps the rich node-tree comps for
  interactive delivery; both read one layout sidecar so they can't diverge.
- **Captions + loudness** — captions are typeset from the already-correct script
  caption track (so technical terms are exact by construction, not transcribed),
  and loudness is normalized deterministically to the voice-content target.

## What landed recently

- **No new episode this week.** The live set holds at eight. The week's work was
  a correctness pass over this repo's own claims — the shorts' hold point, the
  presenter description, and what this repo actually publishes — all three
  corrected above and detailed in the README's rolling log.
- **Episode 1.2 is public** (2026-07-12) — "What Semantic Search Actually Does —
  and What It Can't", the eighth live episode and the first to be built under the
  B-roll-first gate below.
- **B-roll-first production gate.** Once a script clears, the next step is the
  supporting graphics, not narration: the full component set is authored and
  assembled into a silent preview, and no narration take fires until that preview
  is reviewed. Narration is the expensive, re-shoot-hostile leg; the graphics are
  the cheap one to iterate.
- **The silent preview is presenter-blind.** It composites no
  picture-in-picture and no captions, so a graphic whose payoff sits underneath
  the presenter corner — or behind the caption band — passes review and only
  fails after the takes are shot. The keep-out box is now drawn onto the preview
  before the gate is lifted.
- **Caption-contrast floor, channel-wide.** Caption ink is derived per episode
  from that episode's own background base rather than inherited from a previous
  cohort's constants; never near-white text over a light bed. Review checks
  legibility over the lightest frame the captions cross.
- **Timeline colour management pinned.** Setting the colour-science mode alone
  left the editor in a scene-linear space that gamma-decoded every input and
  wrote it back without re-encoding, crushing near-blacks — it reads as "moody
  dark" rather than broken, so it survives eyeballing. The timeline and output
  colour spaces are now pinned explicitly, and a black-frame check is the gate.
- **App-UI episodes held.** Any episode whose graphics depict the product app
  shells holds final production until the refreshed shell ships, then re-skins
  those graphics against the real interface rather than a mock. Non-UI material
  for those episodes proceeds under the B-roll-first gate.
- **Release records reconciled.** Every published episode now carries its release
  date and immutable CDN key in the episode record, so the plan, the roster page,
  and the channel agree without a manual cross-check.
- **Arc progress is a dashboard.** The 50-row arc matrix on the public status
  page is now a dashboard: a four-card progress strip (scripted / designed /
  recorded / rendered) plus per-topic filter chips over the same rows. A
  presentation re-shape — no new numbers.

## Next

- Publish the launch-cohort shorts through the channel's upload path.
- Resume the held app-UI episodes once the refreshed shell ships.
- The next block of Topic-1, Topic-2, and Topic-3 episodes from the current
  script cohort, through the same pipeline.

## How to verify

- Watch the live episodes: the channel at
  <https://www.youtube.com/@Quantapix>, or the CDN cuts linked from
  <https://quantapix.com/videos>.
- The master plan above and the weekly release status are what this repo
  publishes, refreshed as ordinary diffs — the commit log is the change record.
  The narration scripts and per-episode production files stay in the private
  working tree.
