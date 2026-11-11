# 70-SECOND RECUT (current master)

**This file replaces the timecodes in Part 1.2, Part 2, Part 6.2/6.3 and Part 7.1.** The shots, prompts and story are unchanged. Only the timing moves, to fit the generated ElevenLabs takes. In particular, the heavy-bass narrator reads about 1.5× slower than the 60-second plan assumed.

Placement times below are for the **speech inside each file, after trimming the 0.2–0.4 s of lead-in silence** that TTS adds. Line names L1–L16 are the ones in Part 5.

## R.1 Shot table (70.0 s)

| Shot | In | Out | Length | Dialogue / VO placed | Key sync points |
|---|---|---|---|---|---|
| 1 Typewriter | 0:00.0 | 0:02.5 | 2.5 | — | Key strikes; bell 0:02.3 |
| 2A Storm | 0:02.5 | 0:05.5 | 3.0 | L1 newsreader starts 0:05.0 (J-cut) | Thunder 0:02.5 |
| 2B Gold | 0:05.5 | 0:07.5 | 2.0 | L1 continues (underwater filter) | — |
| 3 Radio | 0:07.5 | 0:12.0 | 4.5 | L1 ends ≈0:10.5 | Static 10.5–11.5; **cut to black 0:11.5** |
| 4 The End | 0:12.0 | 0:17.5 | 5.5 | L2 narrator 0:12.2–17.5 | Manuscript thump ≈0:15.5 |
| 5 Narrator | 0:17.5 | 0:21.5 | 4.0 | L3 0:18.0–21.0 | Glasses click 0:17.8; 0.5 s clock-only silence |
| 6 PM office | 0:21.5 | 0:25.0 | 3.5 | L4 officer 0:22.4–24.6 | Door 0:21.8 |
| 7 Ramika CU | 0:25.0 | 0:29.5 | 4.5 | L5 0:25.4–27.7 · L6 "Forever." 0:28.2–29.3 | — |
| 8 Stamp | 0:29.5 | 0:31.0 | 1.5 | — | **THUD 0:30.2** |
| 8B Gate | 0:31.0 | 0:32.0 | 1.0 | — | **CLANG 0:31.05**; Cue B starts |
| 9 Mines | 0:32.0 | 0:34.5 | 2.5 | L7 0:32.1–34.5 | — |
| 10 Settlement | 0:34.5 | 0:36.0 | 1.5 | — | Temple bell |
| 11 Warehouse | 0:36.0 | 0:39.0 | 3.0 | L8 0:36.3–38.8 | Ring drop 0:36.2 |
| 12 World map | 0:39.0 | 0:41.5 | 2.5 | L9 pre-lap starts 0:40.6 | — |
| 13 Cargo port | 0:41.5 | 0:45.0 | 3.5 | L9 ends ≈0:44.9 | **MUSIC HARD STOP 0:45.0** |
| 14 Red phone | 0:45.0 | 0:47.5 | 2.5 | — | Silence 45.0–45.6; ring 0:45.6 and 0:46.4; pickup 0:47.1 |
| 15 Officer | 0:47.5 | 0:51.5 | 4.0 | L10 0:47.8–51.3 | — |
| 16 Ramika tight | 0:51.5 | 0:53.0 | 1.5 | L11 0:51.6–52.9 | — |
| 17 Telex | 0:53.0 | 0:56.5 | 3.5 | L12 whisper 0:53.8–55.5 | **Total silence 55.5–56.5** |
| 18 Harbour | 0:56.5 | 1:00.0 | 3.5 | L13 0:57.0–1:00.8 | **Ship horn 0:56.5**; Cue C starts |
| 19 Boots → ring | 1:00.0 | 1:03.5 | 3.5 | L14 1:00.9–1:04.0 (tail runs 0.5 s into Shot 20) | Boot crunches 60.2 / 60.8 / 61.4 |
| 20 Rocky reveal | 1:03.5 | 1:07.0 | 3.5 | L15 "ഇനി…" 1:04.5–05.3 · L16 "ലോകം." 1:05.7–06.7 | **Suck-out silence 1:06.7–07.0** |
| 21 Title | 1:07.0 | 1:10.0 | 3.0 | — | **BOOM 1:07.0**; CHAPTER 3 at 1:07.4; THE GLOBAL EMPIRE at 1:07.8; fan tag 1:08.5; fade 1:09.7–1:10.0 |

**Checksum:** 2.5+3+2+4.5+5.5+4+3.5+4.5+1.5+1+2.5+1.5+3+2.5+3.5+2.5+4+1.5+3.5+3.5+3.5+3.5+3 = **70.0 s** (1680 frames at 24 fps; the BOOM is on frame 1608).

**What changed from the 60-second plan:** Shot 10 got shorter (2.0 → 1.5 s, it has no dialogue). Every other shot is the same length or longer: the extra space goes to the narration, the phone scene and Rocky's reveal (now 3.5 s, so "ഇനി… ലോകം." keeps its pause).

## R.2 Video-generation changes (Part 4)

| Shot | New use length | Generate |
|---|---|---|
| 4 | 5.5 s | **10 s clip** (a 5 s clip can't cover it) |
| 7 | 4.5 s | **10 s clip** (it needs the lip-sync headroom) |
| 3, 15 | 4.0–4.5 s | 5 s clip, using nearly the whole clip; slow it to 90–95% with optical flow if needed |
| 18, 19, 20 | 3.5 s | 5 s clip; trim the weak first and last 0.5 s |
| All others | ≤ 3.0 s | As in Part 4 |

## R.3 Music map (replaces 6.2)

| Time | Section | Action |
|---|---|---|
| 0:00.0–0:11.5 | Cue A drone + brass | Fade in, rise with the storm, **cut dead at 0:11.5** with the static |
| 0:12.0–0:21.0 | Cue A solo cello | Soft, under the narrator; fade out by 0:21.0 |
| 0:21.0–0:21.5 | — | Clock tick only |
| 0:21.5–0:31.05 | Cue A cold strings | Build; semitone rise at 0:28.2 ("Forever.") |
| 0:31.05–0:45.0 | Cue B ostinato | Rising montage, ducked under L7–L9, **HARD STOP 0:45.0** |
| 0:45.0–0:56.5 | — | **No music** (the phone scene) |
| 0:56.5–1:06.7 | Cue C build | Starts with the ship horn: march → chant → brass. Duck the chant −6 dB under L13/L14. Drums only, at −12 dB, under Rocky's lines |
| **1:06.7–1:07.0** | **Suck-out** | Every track muted, reverb tails included |
| **1:07.0** | **BOOM / Cue C impact** | Peak |
| 1:07.0–1:10.0 | Cue C tail | Ring-out under the title, fade to silence by 1:10.0 |

**Cue C alignment:** with the cue starting at 0:56.5, its built-in silence must fall 10.2–10.5 s into the cue. The Cue C prompt in Part 6 has been updated to this timing.

## R.4 Second-by-second timeline (replaces 7.1)

| Sec | Shot | VO / dialogue | SFX | Music (0–10) |
|---|---|---|---|---|
| 0–1 | 1 | — | Typewriter | 1 |
| 2 | 1 → 2A | — | Bell, thunder at 2.5 | 2 |
| 3–4 | 2A | — | Storm, hull groan | 3 |
| 5 | 2A → 2B at 5.5 | L1 starts 5.0 (filtered) | Underwater | 3 |
| 6 | 2B | L1 | Bubbles | 2 |
| 7 | 2B → 3 at 7.5 | L1 | Radio hiss | 2 |
| 8–10 | 3 | L1 ends ≈10.5 | Hiss | 2 |
| 11 | 3 → black at 11.5 | — | Static swell → cut | 0 |
| 12–16 | 4 | L2 12.2–17.5 | Clock, page thump | 2 (cello) |
| 17 | 4 → 5 at 17.5 | L2 ends | Glasses click | 2 |
| 18–20 | 5 | L3 18.0–21.0 | Clock | 2 → 1 |
| 21 | 5 → 6 at 21.5 | — | Clock, door | 0 → 2 |
| 22–24 | 6 | L4 22.4–24.6 | Footsteps, traffic | 2 |
| 25–27 | 7 | L5 25.4–27.7 | Room tone | 3 |
| 28–29 | 7 → 8 at 29.5 | L6 28.2–29.3 | — | 4 |
| 30 | 8 | — | **THUD 30.2** | 4 |
| 31 | 8B | — | **CLANG 31.05** | 0 → 5 (Cue B) |
| 32–34 | 9 | L7 32.1–34.5 | Wind, crow | 5 |
| 35 | 10 | — | Temple bell | 6 |
| 36–38 | 11 | L8 36.3–38.8 | Ring drop, laughter | 6 |
| 39–40 | 12 | L9 starts 40.6 | Telex | 7 |
| 41–44 | 13 | L9 ends ≈44.9 | Crane, distant horn 43.0 | 8 → 9 |
| 45 | 14 | — | **Silence → TRRRING 45.6** | **0** |
| 46–47 | 14 → 15 at 47.5 | — | TRRRING 46.4, pickup 47.1 | 0 |
| 48–51 | 15 → 16 at 51.5 | L10 47.8–51.3 | Line hiss | 0 |
| 52 | 16 → 17 at 53.0 | L11 51.6–52.9 | — | 0 |
| 53–55 | 17 | L12 whisper 53.8–55.5 | Paper rustle | 0 |
| 56 | 17 → 18 at 56.5 | — | **Silence → SHIP HORN 56.5** | 0 → 2 |
| 57–59 | 18 | L13 57.0–60.8 | Gulls, snow wind | 3 |
| 60–62 | 19 | L14 60.9–64.0 | Boot crunches, ring "ting" | 4 → 6 |
| 63 | 19 → 20 at 63.5 | L14 | Wind drops | 7 |
| 64–65 | 20 | L15 64.5–65.3 · L16 65.7– | Smoke whoosh | 8 (drums only under VO) |
| 66 | 20 | L16 –66.7 → **silence** | Reverse riser → mute | 9 → **0** |
| 67 | 21 | — | **BOOM 67.0** | **10** |
| 68 | 21 | — | Shing hits, embers | 6 |
| 69 | 21 | — | Fade 69.7–70.0 | 3 → 0 |

## R.5 Take selection

Every line has two takes in the ElevenLabs flow "KGF Ch3 Fan Teaser — Voices". Pick by ear:

- **Narrator:** prefer the take with the heaviest chest resonance on the final word of each line.
- **Ramika:** the coldest, least "acted" take.
- **Officer L12:** the breathier whisper.
- **Rocky L16 "ലോകം.":** if a take is longer than 1.0 s of actual speech, trim its tail so the 0.3 s suck-out before the BOOM stays intact. The suck-out matters more than the reverb tail.
