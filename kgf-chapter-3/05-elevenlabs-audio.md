# PART 5 — ELEVENLABS AUDIO PRODUCTION

## 5.0 Model and workflow

- **Model:** use **Eleven v3** for the Malayalam lines. It's the ElevenLabs model with the widest language coverage and it supports inline audio tags (`[whispers]`, `[pause]`, and so on). Older Multilingual v2 is fine for the English lines, but do the Malayalam lines with v3 or they may come out with a Hindi/Tamil accent or be refused. **Check that Malayalam appears in the language list of your account's model before recording.**
- **Voices:** create original voices with **Voice Design** (text-to-voice) from the descriptions below. Don't clone or imitate any film actor or dubbing artist.
- **Takes:** generate 3–4 takes per line and pick by ear. TTS timing is never exact, so time-stretch ±8% in the editor to hit the timestamps (Part 7). Never stretch more than 10%: that's where artefacts start.
- **Export:** WAV 48 kHz / 24-bit if your plan allows it, otherwise the highest-quality MP3. Name files `VO_<shot>_<character>_t<take>.wav`.
- **Honest fallback:** for the narrator and Rocky's single line, a real Malayalam voice actor recorded on a decent USB mic will very likely beat TTS on dramatic weight. Use the same script either way.

> **Settings note.** The ElevenLabs sliders are Stability, Similarity, Style exaggeration, Speaker boost and Speed. On v3, Stability is a three-way choice: *Creative / Natural / Robust*. The values below are starting points; adjust by ear.

---

## 5.1 Voice Design briefs (paste these into Voice Design)

### V1 — NARRATOR (Malayalam)
```
An elderly Malayali man in his seventies, a veteran writer telling a legend. Very deep, warm, slightly gravelly bass voice with a soft breathy texture. Slow, measured storytelling cadence, long dramatic pauses, quiet intensity, intimate close-microphone sound. Native Malayalam speaker, neutral central-Kerala accent.
```
Preview text: `ഒരു കപ്പൽ മുങ്ങി… ഒരു സാമ്രാജ്യം അവസാനിച്ചു… അങ്ങനെയാണ് ലോകം വിശ്വസിച്ചത്.`

### V2 — NEWSREADER (Malayalam, 1980s radio)
```
A middle-aged Malayali male radio news announcer from the 1980s. Clear, formal, crisp mid-range voice, brisk official broadcast cadence, serious and urgent tone, precise enunciation. Native Malayalam speaker.
```

### V3 — RAMIKA SEN (English)
```
A powerful Indian woman politician in her mid-fifties. Low, cool, controlled alto voice, educated Indian-English accent, very precise diction, unhurried, every word final. Cold authority with no warmth, never raises her voice.
```

### V4 — INTELLIGENCE OFFICER (English)
```
A nervous Indian male government intelligence officer in his forties. Mid-baritone voice with a North Indian English accent, respectful, slightly breathless, speaks carefully as if afraid of the reply, capable of a tense whisper.
```

### V5 — ROCKY (Malayalam)
```
A confident South Indian man in his mid-thirties. Very low, calm, resonant bass-baritone voice, relaxed and dangerously quiet, slight rasp, minimal effort, speaks as if he already owns the world. Native Malayalam speaker.
```

---

## 5.2 Line-by-line recording script

| # | Time (in–out) | Shot | Character | Voice | Exact line (paste into ElevenLabs) | Emotion / intensity | Pace / pauses / breath | Settings (starting point) |
|---|---|---|---|---|---|---|---|---|
| L1 | 0:05.5–0:09.8 | 2B→3 | Newsreader | V2 | `ഇന്ത്യൻ മഹാസമുദ്രത്തിൽ റോക്കിയുടെ കപ്പൽ മുങ്ങി. [short pause] റോക്കി കൊല്ലപ്പെട്ടതായാണ് റിപ്പോർട്ടുകൾ!` | Urgent, official, 7/10 | Brisk news pace (Speed 1.05). 0.3 s pause at the full stop. No audible breath. | Stability: Robust · Similarity 0.80 · Style 0.15 · Speaker boost on |
| L2 | 0:10.8–0:14.2 | 4 | Narrator | V1 | `ഒരു കപ്പൽ മുങ്ങി… [pause] ഒരു സാമ്രാജ്യം… അവസാനിച്ചു…` | Sorrowful gravity, 4/10 | Slow (Speed 0.88). 0.6 s pause after "മുങ്ങി". Soft exhale at the end. | Stability: Natural · Similarity 0.85 · Style 0.35 · Speaker boost on |
| L3 | 0:14.8–0:17.0 | 5 | Narrator | V1 | `അങ്ങനെയാണ്… [pause] ലോകം വിശ്വസിച്ചത്.` | Knowing, a hint of irony, 5/10 | Slow (0.88). A 0.5 s pause carrying the irony. Stress "വിശ്വസിച്ചത്". | Same as L2 |
| L4 | 0:19.0–0:20.7 | 6 | Officer | V4 | `Madam, the operation is complete.` | Formal, quietly relieved, 4/10 | Normal (1.0). Small inhale before "Madam". | Stability: Natural · Similarity 0.80 · Style 0.20 |
| L5 | 0:21.7–0:22.9 | 7 | Ramika | V3 | `Close the KGF file.` | Cold command, 6/10 | Deliberate (0.92). Say "K-G-F" as three letters. | Stability: Robust · Similarity 0.85 · Style 0.30 |
| L6 | 0:23.5–0:24.1 | 7 | Ramika | V3 | `Forever.` | Absolute finality, quiet, 7/10 | Slow. Generate it as a **separate file** for clean timing. | Same as L5 |
| L7 | 0:27.3–0:28.9 | 9 | Narrator | V1 | `ഖനികൾ… നിശ്ശബ്ദമായി…` | Mournful, 4/10 | Slow (0.9). Let it trail off. | Same as L2 |
| L8 | 0:31.5–0:33.2 | 11 | Narrator | V1 | `ശത്രുക്കൾ… ആഘോഷിച്ചു…` | Bitter, quiet contempt, 5/10 | Slow (0.9). A slight edge on "ആഘോഷിച്ചു". | Same as L2, Style 0.45 |
| L9 | 0:35.6–0:38.8 | 12→13 | Narrator | V1 | `പക്ഷേ… [pause] അവന്റെ സാമ്രാജ്യം… ഉറങ്ങിയിരുന്നില്ല.` | Turning point: dark rising tension, 7/10 | 0.7 s pause after "പക്ഷേ". Lower and slower on the last word. | Same as L2, Style 0.50 |
| L10 | 0:41.8–0:44.3 | 15 | Officer | V4 | `Madam… [nervous breath] the accounts in sixteen countries…` | Fearful, hesitant, 6/10 | Halting. Audible nervous breath after "Madam". Trails off. | Stability: Creative · Similarity 0.80 · Style 0.40 |
| L11 | 0:44.8–0:45.7 | 16 | Ramika | V3 | `What about them?` | Suspicion, ice-cold, 6/10 | Clipped. No breath before it. | Stability: Robust · Similarity 0.85 · Style 0.30 |
| L12 | 0:47.0–0:48.0 | 17 | Officer | V4 | `[whispers] They're active again.` | Dread, a terrified whisper, 8/10 internally | Slow whisper, breathy. | Stability: Creative · Style 0.50 |
| L13 | 0:49.6–0:52.0 | 18 | Narrator | V1 | `അവർ അവനെ തിരഞ്ഞത്… [pause] കടലിലായിരുന്നു.` | Building awe, 7/10 | Measured (0.92). Pause after "തിരഞ്ഞത്". | Same as L2, Style 0.50 |
| L14 | 0:52.4–0:54.5 | 19 | Narrator | V1 | `അവൻ കടന്നത്… [pause] അതിരുകളായിരുന്നു!` | Triumphant climax, 9/10 | A shade faster (0.95). The last word rises with power, chest voice. | Stability: Creative · Similarity 0.85 · Style 0.65 |
| L15 | 0:55.4–0:55.8 | 20 | Rocky | V5 | `ഇനി…` | Calm, almost amused, 5/10 outwardly | Very slow, low. A soft breath before. Separate file. | Stability: Natural · Similarity 0.90 · Style 0.40 |
| L16 | 0:56.2–0:56.7 | 20 | Rocky | V5 | `ലോകം.` | Quiet total certainty, 10/10 inner menace | Low, short, closed ending: no rise. Separate file. | Same as L15 |

**Total speech:** 16 clips. Generating L5/L6 and L15/L16 as separate files lets you place the dramatic pauses exactly in the edit.

## 5.3 Post-processing chain (in your editor or DAW)

| Voice | Chain |
|---|---|
| Newsreader (L1) | High-pass at 300 Hz, low-pass at 3.5 kHz, light distortion/saturation, radio hiss bed underneath. **This is the "old radio" filter.** For the 2B part (0:05.5–0:06.5), add a 20% underwater low-pass, opening up at the cut to 3. |
| Narrator | High-pass 70 Hz, +2 dB at 120 Hz (warmth), de-ess, compressor 3:1, plate reverb at 8% wet. Keep it dry and intimate. |
| Ramika | High-pass 90 Hz, light compression, small-room reverb at 6% (office). For L11, a phone-line EQ on 30% of the signal only: she's on the phone, but we stay "inside" her room. |
| Officer | L4: room reverb 10%. L10: **full phone EQ** (300 Hz–3.4 kHz). L12: dry and close, no phone EQ: an intimate whisper. |
| Rocky | High-pass 50 Hz, +3 dB at 90 Hz, gentle compression, a long cold hall reverb at 12% wet (harbour space), and a 1/8-note delay at −24 dB on "ലോകം." The tail should die *inside* the 0.3 s silence before the BOOM. |

---

## 5.4 Generated assets (ElevenLabs workspace)

Flow: **"KGF Ch3 Fan Teaser — Voices"** (all takes are on this canvas). Model: `eleven_v4`, 2 takes per line.

| Voice | Saved name | voice_id |
|---|---|---|
| Narrator (heavy bass) | KGF3 Teaser – Narrator (ML, heavy bass) | `XXw1MI8wlYHKjchE8bKo` |
| Newsreader | KGF3 Teaser – Newsreader (ML) | `0mOnChcqQD3xjv5v3pWn` |
| Ramika Sen | KGF3 Teaser – Ramika Sen (EN) | `lcSIEtx9IIFGV4clrdCC` |
| Officer | KGF3 Teaser – Intelligence Officer (EN) | `P7BqWYvOwvc9PvBHsTw5` |
| Rocky | *not yet chosen* | — |

### Take durations vs. timeline slots (first pass)

| Line | Slot | Take 1 | Take 2 | Fit |
|---|---|---|---|---|
| L1 Newsreader | 4.3 s | 5.84 | 5.76 | Too long: start at 0:04.2 instead |
| L2 Narrator | 3.4 s | 5.60 | 5.76 | **Too long** |
| L3 Narrator | 2.2 s | 3.28 | 3.28 | **Too long** |
| L4 Officer | 1.7 s | 2.48 | 2.56 | Start at 0:18.5, OK |
| L5 Ramika | 1.2 s | 2.56 | 2.64 | Start at 0:21.3, OK |
| L6 Ramika | 0.6 s | 1.44 | 1.36 | Lands on the stamp, OK |
| L7 Narrator | 1.6 s | 2.72 | 2.72 | **Too long** |
| L8 Narrator | 1.7 s | 2.72 | 2.88 | **Too long** |
| L9 Narrator | 3.2 s | 4.80 | 4.48 | **Too long** |
| L10 Officer | 2.5 s | 3.68 | 3.92 | Tight: trim the padding |
| L11 Ramika | 0.9 s | 1.60 | 1.52 | OK after trimming |
| L12 Officer | 1.0 s | 2.00 | 2.00 | OK (uses the silence window) |
| L13 Narrator | 2.4 s | 4.16 | 4.00 | **Too long** |
| L14 Narrator | 2.1 s | 3.36 | 3.44 | **Too long** |
| L15–L16 Rocky | — | — | — | Waiting for the voice choice |

Durations include TTS lead-in and lead-out padding (usually 0.2–0.4 s).
