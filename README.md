# qexplaining-public

> 50 videos = 5 topics × 10 subjects each. 10–15 min per video,
> AI-narrated over animated cards/text + D3.js / Cytoscape.js
> graphics. Brand-synced with the two product sites and the two
> product app shells.

A weekly-refreshed window into the explainer arc that runs alongside
the private working repository. The output of the work is **scripts**
(plus the data behind every graphic); rendering happens in Claude
Design; voice + lipsync in a separate pipeline. This repo publishes
the master plan and the scripts as they land.

- Parent organisation: <https://github.com/quantapix>
- Engineering output: <https://quantapix.com>
- Motivational record: <https://femfas.net>
- **Watch: <https://www.youtube.com/@Quantapix>** — the channel where this
  arc publishes; six episodes are live (June–July 2026), with the full
  roster at <https://quantapix.com/videos>.

## Profile-area tags

Every subject below carries one or two of these tags. Order within a
topic is **shootable order** — earlier subjects motivate later ones.

- **P1** — rigorous proofs for LLM "reasoning"
- **P2** — legal applications (axiomatizing complaints for Qnarre)
- **P3** — financial applications (analyzing + accounting → Qresev)
- **P4** — grounding competing technical-analysis approaches
- **P5** — agentic software development (Claude Code + monorepo)

---

## Status — 2026-07-03

Two more episodes went public this week — both from Topic 4 (technical
analysis). Six episodes are now live on YouTube and the channel CDN, up from
four. The full 50-video roster, live and upcoming, renders at
<https://quantapix.com/videos>.

Landed since the last entry:

- **Episode 4.2 — "TA-Lib as Ground Truth: the MACD Alignment Quirk" — is
  public.** A "wrong" MACD that is actually right: the reference library
  realigns both moving averages to the slow period minus one bar, so a naive
  subtraction is off by a single bar; parity with the reference is
  non-negotiable. It is the first Topic-4 episode to reach the channel. Watch:
  <https://www.youtube.com/watch?v=suIFSrd3pHI> or the CDN cut at
  <https://videos.quantapix.com/T4/01-talib-macd-quirk.mp4>.
- **Episode 4.1 — "The TA Bestiary: 117 Indicators, Mostly Redundant" — is
  public.** Scrolling the indicator catalog to a counter that ends at 117 — the
  indicator-inflation problem, and the equivalence classes hidden in plain
  sight. Watch: <https://www.youtube.com/watch?v=wugQWlHa-Ag> or
  <https://videos.quantapix.com/T4/02-ta-bestiary.mp4>.
- **A third script cohort landed — ten more subjects.** Full narration scripts
  plus per-video design bundles are now written for ten more subjects across
  every topic: what semantic search can and can't do, the Lean4 kernel as a
  proof-correctness oracle, the predicate bridge between the model and the
  kernel, a narrative-as-structure formalization, live proof-event streaming,
  the six-strategy defined-risk allow-list, the five evaluation frameworks,
  columnar bar storage, the two-teammate practice, and the monorepo tour. These
  are scripts and graphic specs; rendering happens downstream.
- **Financial-evaluation disclosure baked onto the frame.** Any rasterized card
  that carries a financial evaluation or report now bakes the full "an
  evaluation, not investment advice or a recommendation — do your own due
  diligence" footer directly into the image, not only into the narration, so
  the disclosure travels with the frame wherever it is reused.
- **Channel-wide finishing polish.** Every episode now opens on its own 16:9
  thumbnail as a roughly half-second branded flash that hard-cuts into an
  already-established cold open — no fade-up, and no black frame at the head.
  The branded end screen carries the Quantapix mark and wordmark in the brand
  display typeface, and a shared font loader guarantees the real brand faces
  render on every card rather than a system fallback.

What's coming up:

- The next Topic-1, Topic-2, and Topic-3 episodes from the new script cohort,
  through the same production pipeline.
- Vertical shorts for the live episodes.

## Status — 2026-06-26

No new episode went public this week; the four live episodes (1.1, 1.5, 1.7,
2.1) hold on YouTube and the channel CDN. The full roster, live and upcoming,
renders at <https://quantapix.com/videos>.

Landed since the last entry:

- **The first Topic-4 episode reached a finished master.** Episode 4.2 — "The
  MACD Alignment Quirk" — completed its full finishing pass to a normalized
  master: per-beat takes generated, B-roll cohort rendered, markers re-anchored
  to the actual narration phrase boundaries, loudness normalized. It is the
  first episode outside the Topic-1/Topic-2 production block to bake end-to-end,
  and it is queued for the upload step (not yet public).
- **Silence-handle preflight gate.** Per-beat takes carry short muted speech
  handles so adjacent clips overlap cleanly through wipe transitions. A take
  that arrives without them is now rejected at pre-flight rather than caught as
  a silent-talking artifact downstream — a production-readiness check, not a
  post-render fix.
- **Shared rendering surface.** The B-roll and composition lanes now draw their
  brand tokens (palette, type, easing) from the constellation's shared rendering
  engine, so the explainer arc and the product sites can't drift on brand.
- **Launch-cohort shorts finished.** Each of the four live episodes now has its
  own dedicated vertical short — a self-contained hook-and-payoff cut, not a
  mechanical re-slice of the long form — finished through the off-editor
  decoration and outro lane and entering the upload step.

What's coming up:

- Publish 4.2 and the launch-cohort shorts through the channel's upload path.
- The next block of Topic-1, Topic-2, and Topic-4 episodes through the same
  pipeline.

## Status — 2026-06-19

Four episodes are now public on YouTube and the channel CDN — up from two at the
last entry. The full 50-video roster (live and upcoming) renders at
<https://quantapix.com/videos>.

Landed since the last entry:

- **Episode 1.7 — "Civil RICO, End to End" — is public.** A single complaint
  reduced to a Prop: person → predicate acts → enterprise → pattern → the
  statutory elements, each one a provable lemma. The episode carries the
  channel's first Geometry-Nodes background plate (a recursive tessellation as
  the visual metaphor for the "pattern" element). Watch:
  <https://www.youtube.com/watch?v=FSC5ajwOfUk> or the CDN cut at
  <https://videos.quantapix.com/T1/07-civil-rico-walkthrough.mp4>.
- **Episode 2.1 — "When a docket and its record disagree" — is public.** The
  first Topic-2 episode: a real narrative-analysis use case where a docket and
  its record disagree, and why the verifier's first job is procedural posture.
  Watch: <https://www.youtube.com/watch?v=boe2ZwizQWM> or
  <https://videos.quantapix.com/T2/01-docket-record-disagree.mp4>.
- **Purpose-built Shorts, not re-cuts.** The Shorts lane changed shape. A short
  is now its own ≤2-minute hook-and-payoff with a dedicated vertical take — not
  a mechanical re-cut of the long form. The earlier derivative model (re-slicing
  long-form beats into a vertical timeline) is retired. Fourteen subjects across
  the roster carry a locked short title; the first cohort (the four built long
  episodes) gets shorts first, and the rest follow as their long forms ship.
- **The first short is produced.** The 1.1 short — "The Hallucination Tax" — runs
  through the new off-editor decoration and outro lane end-to-end.
- **Roster titles locked.** Every long-form subject title (and the short titles
  where one exists) is now fixed. Titles are metadata: the on-disk position id
  never changes when a title is reworded, so a title edit never triggers a rename
  cascade and the public URL carries only the cleared phrasing.

What's coming up:

- Shorts for the remaining live episodes (1.5, 1.7, 2.1).
- The next block of Topic-1 and Topic-2 episodes through the same pipeline.

## Status — 2026-06-12

The channel is live. The first two episodes are public on YouTube and the
channel CDN, and the full 50-video roster — live and upcoming — now renders
at <https://quantapix.com/videos>.

Landed since the last entry:

- **Episode 1.1 — "The hallucination tax" — is public** (2026-06-09). The
  pilot's first end-to-end finishing run completed: caption bake, presenter
  wipe-transitions, branded outro plate, chapters recomputed against the
  7:05 final cut. Watch: <https://www.youtube.com/watch?v=DDdKgzDMPzY> or
  the CDN cut at <https://videos.quantapix.com/T1/01-hallucination-tax.mp4>.
- **Episode 1.5 — "Negative verification" — is public** (2026-06-11). The
  episode where the build *fails on purpose* — and the kernel's "no" is the
  right answer. Watch: <https://www.youtube.com/watch?v=3nzYNQhL57k> or
  <https://videos.quantapix.com/T1/05-negative-verification.mp4>.
- **Two-lane presenter decoration.** The compositor can't render a scripted
  node-tree comp hosted on a sourced clip headlessly — it leaks the source
  full-frame, the same class of bug that earlier killed take-hosted captions.
  The decoration pipeline now forks into two lanes: the default lane bakes
  the picture-in-picture element, wipe, and corner chrome **off the editor**
  into transparent intermediates and composites them as plain alpha media
  (leak-safe by construction, fully headless); a second staging lane keeps
  the rich node-tree comps for interactive delivery. All lane-common logic
  lives in shared modules, and both lanes read one layout sidecar, so they
  cannot diverge on where clips land.
- **Freeze-at-gap wipes.** Per-beat takes carry short muted speech handles
  so adjacent clips overlap cleanly — but those handles used to play as
  silent talking during wipe transitions. Wipe segments outside a clip's
  content span now render held frames instead.
- **Operator content marks.** Acoustically-derived content spans tend to
  freeze the presenter mid-blink or open-mouthed. Each episode driver can
  now carry per-take unfreeze/freeze source frames from an operator scrub,
  overriding the acoustic spans; the audio trim marks never move, so the
  timing clock is bit-identical to the acoustic baseline.
- **Branded outro plate.** A 20-second end screen with the next episode's
  tile, composited as a flat raster plate and appended as a plain clip —
  vector-text node-tree authoring was abandoned after missing-font blank
  renders. Bottom corners stay clear for YouTube's native end-screen
  elements.
- **Channel background bed.** A seamless programmatic loop, dimmed and baked
  to a low-alpha plate, lands on the bottom track automatically.
- **Reproducibility.** The first four episodes were reproduced from scratch
  through the full pipeline — the per-phase drivers plus the shared modules
  rebuild a shipped episode end-to-end, which is the point of scripting the
  finishing pass in the first place.

What's coming up:

- 1.7 (Civil RICO walkthrough) and 2.1 finish through the same pipeline —
  both already carry the wipe layout and the segmented caption bake.
- The Shorts pickup lane for the live episodes.

## Status — 2026-06-05

Production-finishing work on the channel's first end-to-end episode (the
hallucination-tax pilot). Two longstanding finishing bugs are now fixed, and
the per-beat narration pipeline is consistent across the first four episodes.

Landed since the last entry:

- **Caption track no longer leaks.** The earlier approach hosted the burned-in
  caption composite on a portrait presenter take, and that take-hosted comp
  leaked its own source full-frame at render — the "two presenters" artifact.
  The fix bakes the assembled caption track into a few short **transparent
  intermediate overlays** and tiles them onto a fresh top track: plain alpha
  media, no take-hosted comp, nothing to leak. The same caption file is now
  both the upload sidecar and the bake source, so on-screen text and the
  uploaded captions can't drift.
- **PIP wipe-transition replaces the parked gap-holder.** Keeping the
  presenter corner continuously filled between beats used to need a gap-holder
  clip, which tripped the same take-host leak and got parked. It's removed
  entirely. The replacement overlaps adjacent presenter takes on two video
  tracks and wipes between them; because it's hosted on picture-in-picture
  clips rather than a full-frame take, it's leak-safe by construction.
- **Phrase-anchored re-timing across the pole-position episodes.** Per-beat
  takes carry a short trailing-silence handle so neighboring clips overlap
  cleanly, and cue timings re-anchor to the actual narrated phrase boundaries
  (with a small tail-guard) rather than segment indices — re-renders
  re-segment, so anchoring by phrase text is the stable contract. This
  pipeline is now wired across the first four episodes, not just the pilot.

What's coming up:

- First end-to-end finishing run on the pilot with the new caption bake and
  wipe-transition in place.
- Carry the per-beat re-timing pipeline across the second cohort of scripts.

---

## Status — 2026-06-01

Launch day for the public donation drive; the channel's public surface
refreshes weekly (Fridays) from here on. A consolidated current snapshot
now lives in [`STATUS.md`](./STATUS.md); this rolling log keeps the
per-week detail.

Landed since the last entry:

- **qreel shipped to main.** The one-command bake tool described in the
  2026-05-28 entry is no longer a draft — the plugin (the `/reel <bundle>`
  command + its Python package) is built and on the mainline, and the
  episode-side callers have been reconciled to the shipped API. It bakes a
  finished-script bundle to a captioned, loudness-normalized MP4 through a
  running DaVinci Resolve session, composing the production-assistance,
  explainer, and background-plate outputs.
- **Cohort-2 scripts landed.** The next block of subjects (the priority
  slots that follow the pole-position production episodes) have their
  `script.md` + `design.md` authored, extending the layered-scaffolding
  pipeline beyond the first sprint cohort.

What's coming up:

- First end-to-end `/reel` bake of a standalone bundle against a live
  Resolve session.
- Continue the per-episode production pipeline across the cohort-2 scripts.

---

## Status — 2026-05-28

Design work this week on **qreel** — a one-command bake tool that turns a
finished-script bundle into a finished video. The idea: collapse the
multi-step Resolve finishing pass (assemble → caption → render → loudness)
behind a single `/reel <bundle>` command that drives a running DaVinci
Resolve session and hands back one normalized MP4.

What the design locks:

- **Two input modes, auto-detected.** A full explainer-episode directory, or
  a minimal standalone bundle (a script plus a folder of clips) — the tool
  sniffs which and dispatches accordingly. Standalone mode makes the same
  pipeline available for ad-hoc one-offs, not just the 50-episode arc.
- **Captions are typeset, not transcribed.** Burn-in captions are authored as
  a vector text overlay rendered directly from the already-correct script
  SRT, so technical terms (`Prop`, `§ 1983`, `Lean`, `RICO`) are exact by
  construction. Speech-to-text is kept only as a fallback for bundles that
  arrive without a caption track — it can't be spell-corrected after the
  fact, so it's the wrong default for jargon-dense narration. This follows
  the channel's "let the compositor draw the typography" principle.
- **Loudness is deterministic.** The finished master is normalized to the
  −14 LUFS / −1 dBTP voice-content target by a standard two-pass loudness
  filter applied after render, rather than a hand-tuned mixer pass — so the
  level is reproducible and verifiable on every bake.
- **One finished output per run.** A single aspect per invocation (16:9 or
  9:16); the command loops for both. The tool ends at the normalized MP4 —
  upload stays a separate, deliberate step.

The work also formalizes a dedicated **captioning phase** in the per-episode
pipeline (authoring the text overlay from the script SRT) and trims the
mastering phase to chapter markers, with loudness handled by the bake tool.
The design is captured in a `qreel` spec under review; implementation is
sequenced behind a small set of upstream Resolve-wrapper additions.

What's coming up:

- Promote the qreel spec out of draft and stand up the plugin scaffold.
- Lift the subtitle-overlay routine in the Resolve wrapper (today a stub) and
  add the new captioning-phase driver across the production episodes.
- First end-to-end `/reel` bake of a standalone bundle against a live Resolve.

---

## Status — 2026-05-24

Five-episode sprint week kickoff. The week's lock is **1.0 + 1.1 +
1.5 + 2.1 + 1.7** end-to-end — the first four are pole-position
production episodes ready to ship; 1.7 (Civil RICO walkthrough) is
the channel's first greenfield full-quad authoring under the
layered-scaffolding pipeline.

- **Production-phasing spec adopted** (2026-05-19). The earlier
  monolithic `assemble.py` driver is retired channel-wide.
  Replaced by a 7-script per-episode pipeline
  (`phase{0,1,3,5,6,8,9}_*.py`) running under a 12-phase operator
  runsheet — pre-flight, assembly, captioning, decoration, scoring,
  mastering, review render, cut review, final render, shorts pickup,
  rescue, upload. Each phase ends in an explicit playback gate;
  later phases never silently override earlier decisions. Spec at
  `data/specs/production-phasing-2026-05-19/SPEC.md`.
- **All three earlier production episodes migrated** (1.1 + 1.5 +
  2.1). Same 7-phase shape across the channel; per-episode
  `PRODUCTION.md` runsheets are the operator's source of truth.
- **Real-Janet 3-avatar production set** locked since 2026-05-11.
  Three HeyGen Photo Avatars trained from real-Janet source stills,
  rotated per beat-archetype: priority 1 hand-down (channel default;
  declarative narration spine), priority 2 hand-up (contemplative
  beats), priority 3 head + shoulders (PIP / lower-third / B-roll
  cutaway). Voice unchanged: Janet-2 Design-a-Voice (locked
  2026-05-07). Pose rotation is per-episode creative texture, not
  identity drift — any change to the three pinned avatar IDs is a
  channel-rebrand event.
- **1.0 channel-preview** upgrades to the full 7-phase shape this
  week. Today it carries a preview-light single-take A-roll path; the
  upgrade brings it under the same operator runsheet as 1.1+, so the
  channel has one production shape, not two.
- **1.7 Civil RICO walkthrough** enters full production. Episode
  ships with the channel's first **Blender Geometry-Nodes plate**
  (G3 — a `p4m` recursive tessellation as the visual metaphor for
  RICO's "pattern" element) rendered via the typed `blendr._cli`
  wrapper alongside the standard Remotion B-roll. Two-lane delivery:
  Remotion components for G1, G2, G4, G5, G6 and the cards;
  Blender-rendered PNG for G3.

What's coming up:

- Five-episode end-of-week ship target: 1.0 / 1.1 / 1.5 / 2.1 / 1.7
  all uploaded to `videos.quantapix.com` and the YouTube channel,
  24-h unlisted hold before public flip.
- Channel-page Claude Design additive bundle (5 playlist covers +
  channel-trailer end-frame composite, dual aspect).
- Reshoot of the 1.0 and 1.1 narration tracks against the
  rebalanced three-avatar pose rotation (no copy changes — the
  existing scripts hold; the visual variety lift is on the
  pose-rotation mix per beat).

---

## Status — 2026-05-17

The three production episodes (1.1 + 1.5 + 2.1) have crossed the
final pre-Resolve gate: every B-roll component is Remotion-ported,
every internal cue is anchored to the actual narration word
boundaries, and both per-episode operator runsheets are locked.
What landed this week:

- **B-roll Remotion port complete** for 1.1, 1.5, 2.1 — 16 G-slot
  compositions registered, rendering to ProRes 4444 RGBA at the
  channel-locked 1920×1080 / 30 fps. Each composition's internal
  cue frames (line type-in, recolor, glow ramp, layout crossfade,
  zoom transition, etc.) re-anchored to the production-locked
  marker CSVs — the SRT word boundaries from the actual Janet
  takes, not the script's narrative estimates.
- **9:16-only HeyGen rule** (locked 2026-05-10) confirmed across
  all three production episodes. HeyGen ships portrait; Resolve
  composites the 16:9 long-form via Pan/Tilt crop on the keyed
  9:16 source. Halves credit spend, halves render latency,
  eliminates the crown-crop class of bugs that plagued earlier
  square→16:9 attempts.
- **1.1 production-prep parity** with 1.5 + 2.1. Both per-episode
  authoring aids landed: a Fusion-keyframe notes file (S5 corner
  PIP + S6 Shorts inset band + S7 trust-boundary glow timing) and
  a 10-phase operator runsheet from pre-flight through upload. 1.1
  is the channel's first end-to-end pass; the per-episode keyframe
  choreography it locks in templates for 1.5+.
- **Channel-canonical proper-noun pronunciation pins** locked at
  the channel-wide voice config. **Qnarre = `Kuh-NAR-REE`** (three
  syllables; stressed middle; French *qnarré* ending — channel
  debut at 2.1 beat 06 with 8 narrated instances); **Qresev =
  `Kuh-RES-ev`** (three syllables; stressed middle `-RES-`;
  sibling-shape to Qnarre — channel debut at 2.1 close). Per-take
  drift inside an episode (or across two episodes) is a re-render
  trigger, not a tolerance accept: trivially-verifiable consistency
  is the channel's structural promise.
- **Per-episode `assemble.py`** drivers (DaVinci Resolve assembly
  via the in-house Python wrapper + recipe library) verified
  against the 9:16-only source path. Single take-pool import; two
  parallel timelines off the same source; per-cue Remotion MOVs
  placed at marker frames; back-to-back YouTube-master + Shorts
  render.

What's coming up:

- First end-to-end Resolve run on 1.1 — assemble.py executes; S5 +
  S6 Fusion template builds (channel-wide one-time authoring); S7
  per-episode kernel-layer breathing-glow keyframes; S8 subtitle
  generation from the A-roll; S9 loudness normalization to −14
  LUFS; S10 dual render (long + short).
- Channel music-bed selection (T1 register — minimalism / ambient
  electronic) — the loop chosen for 1.1 becomes the T1 default;
  every subsequent T1 episode must pick a different loop per the
  channel rebrand-event rule.
- Publish path validation: long-form master to the channel's
  binary CDN at `videos.quantapix.com`; YouTube upload with the
  AI-disclosure toggle and the stack disclosure in the description.
- 1.5 + 2.1 inherit the 1.1 path; 1.6+ inherit the lift-eligible
  pieces that fall out of running the chain three times.

## Working stack (locked)

- **A-roll (voice + face).** HeyGen Photo Avatar V against a single
  locked still. Voice generated via HeyGen's Design-a-Voice (channel
  voice locked retroactively to the production preview at
  <https://quantapix.com/videos/Janet-preview.mp4>). Per-beat
  generation — one MP4 + sidecar SRT per script beat per aspect —
  rather than monolithic takes; cheaper re-cuts, tighter lipsync.
- **B-roll (cards + graphics + animations).** Remotion: React-based
  programmatic video. Per-video components live alongside the
  script as JSX in a small workspace package; brand tokens
  (palette, type, easing) are read through a generated `tokens.ts`
  so no hex literals leak into renders.
- **Composition + finishing.** DaVinci Resolve Studio, scripted via
  an in-house Python wrapper plus a recipe library that turns
  per-episode Resolve drivers from ~260-line scripts into ~80-line
  ones (now a per-phase pipeline). The wrapper handles import, two-aspect timeline
  setup, A-roll comping with breath gaps, B-roll cue placement at
  marker frames, and back-to-back YouTube-master + Shorts render.
  Fusion node-tree authoring (Janet PIP corner ring + soft shadow,
  Shorts inset band, per-cue compositing) is manual at v1, guided
  by per-skill node-tree force-graph diagrams.
- **Captions + loudness.** Resolve native subtitle generation from
  the A-roll track (V4 burn-in plus sidecar SRT for upload
  metadata); Fairlight loudness normalization to −14 LUFS / −1 dBTP
  on the master bus.
- **Music + SFX.** YouTube Audio Library (free, no-attribution-
  required filter, monetization-safe); per-topic register pivot
  (T1 ambient electronic / T2 string-pad / etc.). SFX library
  selected per cue, kept sparing — no whooshes, no risers under
  Janet.

ElevenLabs is deferred — only revisited if HeyGen's voice quality
fails a real production take. So far it hasn't.

---

## Topic 1 — Why theorem provers… instead of semantic searches?

*Profile mix: **P1** dominant, P2 / P3 supporting.*

1. **The Hallucination Tax — Where LLMs Lose at High Stakes** [P1] A complaint that hinges on a § 1983 element the model "remembered wrong"; probabilistic recall vs. provable derivation; the cost curve as stakes rise. · Short: "The Hallucination Tax"
2. **What Semantic Search Actually Does — and What It Can't** [P1, P5] Cosine similarity demoed as a magic trick that's not magic; embeddings cluster, they do not derive.
3. **The Lean4 Kernel — a 10kloc Oracle for Proof Correctness** [P1] "Every proof is checked by a program small enough to read." Type checker as the trust boundary; one `.lean` file's type elaboration *is* the verdict. · Short: "The 10,000-Line Checker"
4. **Predicates — Where Judgment Lives Between LLM and Kernel** [P1] Not the kernel, not the LLM — the markdown predicate. Three-layer split: kernel + predicate sub-agents + thin driver; each predicate has provenance + cite + question.
5. **Negative Verification — When the Kernel Says "Not Proven"** [P1, P2] The demo where the build *fails*, and that's the right answer. `sorry` on the affected theorem; other theories still elaborate. · Short: "When the Kernel Won't Sign Off"
6. **Axioms vs. Evidence — What We Don't Trust the LLM With** [P1] Which knobs are policy, which are facts, which are model output. Axioms first-class with cite + scope; LLM output never enters the trust base.
7. **Civil RICO, End to End — Predicate, Sub-Axioms, § 1962 Elements** [P1, P2] A single complaint reduced to a Prop. Person → predicate acts → enterprise → pattern → § 1962 elements; each one a provable lemma. · Short: "What Makes a 'Pattern'"
8. **Title VI — Discriminatory Intent Has Structure** [P1, P2] "Intent" sounds soft. It isn't. Protected class, recipient of federal funds, intentional treatment, causation; predicates render each as a question with required cites.
9. **Same Kernel, Different Axioms — Scaling to Financial Contracts** [P1, P3] Same machinery, different axioms. TREND, MOMENTUM, OPTIONS-RISK, SECTOR, DRAWDOWN as kernel-checkable predicate vocabularies over an OHLCV trace.
10. **The Cost — Latency, Surface Area, and Auditability as a Feature** [P1, P5] 30s elaboration vs. 1s vector search; predicate library upkeep; but every result ships with a witness.

---

## Topic 2 — Why narrative analysis… or Qnarre?

*Profile mix: **P2** dominant, P1 supporting, P5 cameo.*

1. **When a Docket and Its Record Disagree — Why I Built Qnarre** [P2] A real docket, dispositions misread, a brief built on a wrong premise. Why Qnarre's first job is procedural posture. · Short: "When the Docket and the Record Disagree"
2. **What a "Narrative" Is, Formally — Predicates Over Named Entities** [P1, P2] A story is a graph plus a calendar. Actors, acts, edges, time; the narrative reduces to a Lean structure.
3. **Three-Zone Qnarre — Input, Kernel, Witness** [P2, P5] A tour of the live `/app` island: docx/text in (left), kernel elaboration (middle), witness + fail trace (right).
4. **Watching a Proof Elaborate Live — SSE Event Streaming** [P2, P5] 12 seconds of a real Lean elaboration as a stream of `{stage, msg, kind}` events; the events drive the React island's colors.
5. **From DOCX to Lean — How a Complaint Becomes a Claim Object** [P2] A paragraph of pleading mapped to four structured predicates. Extraction → predicate match → axiom selection → theorem assembly.
6. **When the Appendix Is the Source of Truth — RAv:p Record Citations** [P2] Every assertion carries `RAII:203`. 10-vol Combined Record Appendix; ground-truth pagination by footer stamp; never cite raw filings on appeal.
7. **Pro Se on Appeal — Encoding the Procedural Traps as Predicates** [P2] The asymmetry between counsel and pro se on procedural traps. Rule 4(a), tolling motions, the SO 2-99 page ceiling — encoded as predicates so a brief doesn't trip them. · Short: "The Procedural Traps, Made Explicit"
8. **Counterfactual Narratives — What a Defense Story Has to Deny** [P1, P2] Every theorem has a contrapositive. Opposing counsel's narrative as a competing predicate set; Qnarre shows which axioms they would need.
9. **Stacking Predicates — Civil RICO and § 1983 Over One Fact File** [P1, P2] One fact pattern, two statutory frames, one kernel. Shared facts file, framework-specific axioms, theorems compose.
10. **What Qnarre Never Does — Write Your Brief for You** [P2, P5] The verifier's modesty. Predicates check, witnesses cite, but legal-strategy and prose are the lawyer's; auditability over autonomy.

---

## Topic 3 — Why result evaluations… or Qresev?

*Profile mix: **P3** dominant, P1 + P4 supporting.*

1. **Backtests Lie — the Survivorship and Look-Ahead Problem** [P3] A hand-picked equity curve that explodes when delisted names are removed. Where standard backtests cheat; what a kernel-checked evaluator must refuse. · Short: "Why That Backtest Is Lying"
2. **Six Defined-Risk Strategies — and a Hard Refusal of the Rest** [P3] "We won't even compute it" for naked options. Long calls/puts, debit spreads, covered calls, protective puts — the allow-list. · Short: "The Six It Will Compute, and Nothing Else"
3. **Five Frameworks — TREND, MOMENTUM, OPTIONS-RISK, SECTOR, DRAWDOWN** [P3, P1] A portfolio is judged five ways at once. Each framework a Lean theorem set with its own predicate library.
4. **Why a Sector Cap Needs a Kernel, Not a Spreadsheet** [P3] "Max 25% Tech" — under whose definition? GICS sectors as the only acceptable referent; canonical 11 names; cap is a provable predicate.
5. **One Bar Schema, Ten Consumers — the OHLCV Parquet Hub** [P3, P4] One bar schema, ten consumers. `{ts, o, h, l, c, v, adj_c}`; vendor names die at the boundary.
6. **Portfolio In, Verdict and Witness Out — Qresev Live** [P3] 90 seconds of Qresev rendering verdicts on a 10-name portfolio. SSE events tagged by framework; the witness card carries the cite chain.
7. **Drawdown as a Theorem — the Conservative Mandate as a Prop** [P3] "No drawdown > 8%" is a Prop, not a wish. How the predicate phrases historical drawdown; how a conservative PM uses it as a precondition. · Short: "'No Drawdown Over 8%' as a Checkable Claim"
8. **Where the LLM Lives — Predicate Judgments Over Price Action** [P1, P3] A chart segment, a question, an answer with a cite. Structured-output prompts return JSON predicate values; never free text into the kernel.
9. **Three PMs Disagree, the Kernel Doesn't — Per-PM Axioms** [P3] Three PMs disagree. The kernel doesn't. Per-PM `risk_policy.md` becomes per-PM axiom set; same theorems, different verdicts.
10. **What Qresev Refuses — Naked Options, Leverage, Look-Ahead** [P3] Refusal as a feature. UI hard-refuse on disallowed legs; kernel rejection on look-ahead reads.

---

## Topic 4 — Why rigorous debates about… technical analysis?

*Profile mix: **P4** dominant, P3 + P5 supporting.*

1. **The TA Bestiary — 117 Indicators, Mostly Redundant** [P4] Scrolling the catalog with a counter that ends at 117. The indicator-inflation problem; equivalence classes hidden in plain sight. · Short: "117 Indicators, Mostly the Same"
2. **TA-Lib as Ground Truth — the MACD EMA-Realignment Quirk** [P4] A "wrong" MACD that's actually right. TA-Lib realigns both EMAs to slow-1; naive subtraction misses by one bar; parity is non-negotiable. · Short: "The MACD Alignment Quirk"
3. **DuckDB and Parquet — Why Columnar Beats Row-Store for Bars** [P4, P5] "10 years of bars in 30 ms." Column-oriented IO, predicate pushdown, single-file portability.
4. **Lightweight-Charts v5 — 10 Years of Bars at 60fps** [P4] The chart that doesn't blink at zoom-out. Pinned via npm at `5.2.0`; canvas-only rendering; v5 shape.
5. **Aggregators — Small-Multiples, Heatmaps, Three.js Surfaces** [P4] From one symbol to a sector. Tab-switching; aggregates = symbol sets; operators DuckDB-first.
6. **Three PMs on One Feed — Where the Disagreements Live** [P3, P4] Same bars, three verdicts. Separation of capital + differentiated strategies; per-PM watchlists; disagreement as a signal.
7. **Even the Chart Viewer Refuses Naked Legs — the Options Floor** [P3, P4] Even the chart viewer refuses naked legs. Cross-project rule; UI never offers a leg the runtime would refuse.
8. **The Bar You Saw vs. the Bar You Traded On — Data Sourcing** [P4] The bar you saw vs. the bar you traded on. Live IEX vs. consolidated tape; backfill sources; reconciliation at the canonical schema.
9. **"Tech" Is Not a Sector — GICS as the Only Referent** [P3, P4] "Tech" is not a sector — `Information Technology` is. 11 canonical names; shared parquet, thin readers per project.
10. **What an Indicator Is, Formally — TA as Testable Predicates** [P1, P4] "RSI > 70" as a Prop with a witness. Predicate libraries promote indicators from cosmetic to provable; the bridge from analyzing to accounting.

---

## Topic 5 — About Quantapix… the two-teammate practice

*Profile mix: **P5** dominant, all others as illustrations.*

1. **Two Teammates, One Repo — What the Practice Looks Like** [P5] Sole developer + expert AI assistant; narrow team, wide repo, explicit `CLAUDE.md` contracts at every boundary. · Short: "Two People, One Repo"
2. **The Monorepo Tour — Subprojects, One Venv, One Workspace** [P5] Sixty seconds, every subproject. Cytoscape repo map; edges are shared-data hubs. · Short: "The Monorepo in 60 Seconds"
3. **Claude Code as the Third Teammate — Agents You Can Fire** [P5] A sub-agent that did one job and vanished. Per-task agents; when to spawn vs. inline; `CLAUDE.md` as the contract.
4. **CLAUDE.md — Instructions for the Colleague Who Never Reads Twice** [P5] A short, harsh `CLAUDE.md` beats a long polite one. Rules over preferences; pointers over prose; the trim discipline.
5. **memsearch — Remembering What Was Said Last Tuesday** [P5] Cross-session recall. ONNX `bge-m3`, per-subproject collection scope, fork-isolated recall.
6. **The 5×10 Plan — Made by Claude, for Claude to Make** [P5] Outlining as a structured-output task; the design hand-off; the brand-sync constraint; the very plan you're watching being executed.
7. **Two Products From One Kernel — Qnarre and Qresev** [P1, P5] Two SSE servers, two Astro islands, one type-checked Lean. How product variation lives above a shared kernel without copy-paste.
8. **The Legal Arc — How a Complaint Becomes an Axiom Set** [P2, P5] How a legal complaint is read into predicates and axioms, and how the kernel composes a verdict from them. Worked on synthetic complaint fixtures — the method, not any party's live case.
9. **The Financial Arc — From Analyzing TA to Evaluating Portfolios** [P3, P5] An indicator becoming a predicate becoming a portfolio verdict. Data hub → analyzer → evaluator; each layer narrower.
10. **What Quantapix Is Betting On — Kernels Under Everything** [P1, P5] The thesis in one card. An LLM is fast and frequently right; a kernel is slow and rarely wrong; both, audited together, change which industries can adopt this. · Short: "Kernels Under Everything"

---

## Brand sync (must hold across all 50 videos)

- Single source of truth for color / type / spacing is the
  `tokens.css` shipped to <https://quantapix.com>; D3 / Cytoscape
  themes pull palette from it, never hex literals.
- Wordmark, accent shapes, and closing-card lockup match the live
  product sites and the two `/app` shells (Qnarre, Qresev).
- Voice and pacing match the calm, declarative cadence of the site
  copy. No marketing exclamations. No rhetorical questions. No
  activist framing.
- Every closing card carries the same Quantapix wordmark + a
  one-sentence pull-quote.

## Cadence

Refreshed weekly from the private working tree. Outline edits, new
profile-area tags, and finalised scripts are committed as ordinary
diffs — the commit log is the change record.

Per-video deliverables follow a seven-file shape under
`scripts/<topic-slug>/<n.m>-<slug>/`:

- `script.md` — Janet narration with timing, on-screen card cues,
  graphic-spec slugs, pacing notes for the voice generator.
- `design.md` — Claude Design prompts for the per-video B-roll
  bundle; tokens contract; cue-state spec for each Remotion
  component.
- `resolve.md` — DaVinci Resolve project preset, V1–V4 / A1–A4
  track layout, A↔B sync strategy via marker CSV, render preset.
- `SHOOTING.md` — production-readiness gate (voice, takes,
  per-cue motion exports, marker CSV, SFX, music) plus the
  cut → review → render → publish sequence.
- `FUSION-NOTES.md` — per-episode Fusion-comp keyframe schedule
  (S5 PIP corner / S6 Shorts inset band / S7 trust-boundary
  glow), color-page guard, SFX placement, music-bed register.
- `PRODUCTION.md` — 12-phase operator runsheet from pre-flight
  through upload (pre-flight → assembly → captioning →
  decoration → scoring → mastering → review render → cut review
  → final render → shorts pickup → rescue → upload). Each phase
  ends in an explicit playback gate.
- `heygen-aroll.md` — per-beat HeyGen call payloads (one
  `create_video_from_avatar` payload per script beat) plus
  per-take acceptance gate.

Plus seven per-phase Python drivers
(`phase{0,1,3,5,6,8,9}_*.py`) and a marker resolver
(`retime_markers.py` — cue-key → SRT-phrase resolver that emits
the per-episode marker CSVs from the actual take SRTs). The
earlier monolithic `assemble.py` driver is retired channel-wide
as of 2026-05-19.

Five episodes carry the full set this sprint week:
1.0, 1.1, 1.5, 2.1, 1.7. Channel pilot 1.0 upgrades from the
preview-light shape to the same 7-phase pipeline as 1.1+.

## Contact

[`quantapix@gmail.com`](mailto:quantapix@gmail.com)

## License

MIT (`LICENSE`). Content-class repo — explainer scripts, episode
plans, and production READMEs. Short embedded snippets ride the
same MIT grant.
