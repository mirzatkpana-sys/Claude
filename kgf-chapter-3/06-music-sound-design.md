# PART 6 — MUSIC AND SOUND DESIGN

## 6.0 Principles

- **Score:** fully original. No KGF themes, melodies, chants or sound-alikes. Don't put "KGF", "Ravi Basrur" or any film or composer name into a music-generation prompt: it risks copying and many tools refuse those prompts.
- **Silence is the main weapon.** There are three engineered silences:
  1. **0:17.0–0:18.0** after "വിശ്വസിച്ചത്": a gentle silence.
  2. **0:39.0–0:39.6, and from 0:48.0 to 0:49.0**: dead silence, no room tone.
  3. **0:56.7–0:57.0**: the suck-out before the BOOM.
- **Mix targets:** −14 LUFS integrated (YouTube/Instagram), true peak ≤ −1 dBTP. Dialogue always sits on top. Duck the music −8 to −12 dB under every line.

## 6.1 Music-generation prompts (Suno / Udio / ElevenLabs Music / Stable Audio)

Generating one 60-second cue rarely lands the cues exactly. **Generate three stems and cut them to the timeline:**

### Cue A — "Requiem for an Empire" (0:00–0:27) · 45 s generation
```
Original dark cinematic orchestral underscore, instrumental only, 60 bpm, D minor. Opens with a deep sub-bass drone and distant low brass cluster, a lonely solo cello melody of sorrow, slow tremolo strings, sparse low piano notes, occasional timpani rolls like distant thunder. Mysterious, mournful, epic Indian action-thriller atmosphere with subtle South Indian tonal colour from a low nadaswaram-like reed drone. Gradually builds cold tension with high sustained violins at the end. No vocals, no drums kit, no melody resembling any existing film theme.
```

### Cue B — "The World Moves On" (0:27–0:39) · 30 s generation
```
Original tense cinematic montage cue, instrumental only, 100 bpm, D minor. A driving low string ostinato in 16th notes, ticking clock-like percussion, low staccato brass stabs, a pulsing synth bass under the orchestra, mridangam and frame-drum rhythmic layer, rising pitch and intensity every four bars, ending on a sharp unresolved crescendo that cuts off abruptly. Espionage, conspiracy, momentum. No vocals.
```

### Cue C — "Return" (0:49–1:00) · 30 s generation
```
Original epic cinematic hero-reveal cue, instrumental with wordless choir, starts at 70 bpm in D minor. Opens with a very deep sub-bass rumble and a low male wordless choir hum, slow building taiko and large thunder-drum hits, rising string swells and brass crescendo growing for 7 seconds, then a complete sudden silence for half a second, then one enormous full-orchestra plus choir plus sub-drop impact hit in D, then a long ringing orchestral tail with low brass and choir sustaining, fading out. Triumphant, menacing, legendary. No lyrics.
```

**Extra one-shots to generate or source (royalty-free):** a big orchestral "BOOM" hit with sub-drop · a riser that reverses into the BOOM · a single deep taiko hit.

## 6.2 Music map

| Time | Section | Level | Action |
|---|---|---|---|
| 0:00.0–0:02.5 | Cue A intro drone | −30 → −22 dB | Fade in under the typewriter |
| 0:02.5–0:06.5 | Cue A brass cluster | −18 dB | **Rises** with the storm |
| 0:06.5–0:10.0 | Cue A drone | −24 dB (ducked) | Under the radio. **Cut dead at 0:10.0**, together with the static |
| 0:10.5–0:17.5 | Cue A solo cello | −20 dB | Re-enters soft at 0:10.6, **fades out** by 0:17.5 |
| 0:17.5–0:18.0 | — | silence | Clock tick only |
| 0:18.0–0:26.0 | Cue A cold strings | −22 → −16 dB | Builds through Scene 3, a semitone rise at 0:23.5 ("Forever") |
| 0:26.0 | Transition | — | Cue A ends **on the CLANG** |
| 0:26.0–0:39.0 | Cue B ostinato | −18 → −10 dB | **Rises** through the montage, ducked under VO |
| **0:39.0** | **HARD STOP** | **silence** | Cut on the exact frame of the cut to Shot 14. No reverb tail. |
| 0:39.0–0:49.0 | — | none | Scene 5 has **no music**. Phone, room tone and breathing only. |
| 0:49.0–0:56.7 | Cue C build | −24 → −8 dB | **Returns** under the ship horn and crescendos to the reveal |
| **0:56.7–0:57.0** | **SUCK-OUT** | **−∞** | All tracks muted, including the reverb tails |
| **0:57.0** | **BOOM** | −3 dBFS peak | Orchestral tutti + sub-drop + taiko, synced to the cut to black |
| 0:57.0–0:59.7 | Cue C tail | −10 dB → fade | Choir and brass ring-out under the title |
| 0:59.7–1:00.0 | — | fade to silence | |

## 6.3 Sound-effects cue sheet

| # | Time | Shot | SFX | Notes |
|---|---|---|---|---|
| S1 | 0:00.2–0:02.3 | 1 | Typewriter key strikes ×11 + carriage bell | Sync each strike to a letter appearing; the bell on the "." |
| S2 | 0:02.5 | 2A | Thunder crack (close, sharp) | Sync to the lightning flash |
| S3 | 0:02.5–0:05.0 | 2A | Storm wind + rain + crashing waves | A bed with a big low-end roar |
| S4 | 0:03.5 | 2A | Steel hull groan / metal stress | Pitch down by 3 semitones |
| S5 | 0:05.0–0:06.5 | 2B | Underwater pressure + bubbles + muffled thunder | Low-pass everything above at 400 Hz |
| S6 | 0:06.5–0:09.8 | 3 | Radio hiss/crackle bed | Under the newsreader |
| S7 | 0:09.8–0:10.0 | 3 | Static swell → hard cut | Builds 200 ms, then silence |
| S8 | 0:10.5–0:18.0 | 4–5 | Wall clock tick (1 Hz) | Quiet. Most audible in the 0:17–0:18 silence |
| S9 | 0:13.2 | 4 | Manuscript page riffle + cover thump | |
| S10 | 0:14.6 | 5 | Spectacles fold click | Tiny, close |
| S11 | 0:18.3 / 0:18.8–0:19.0 | 6 | Door latch click + 3 footsteps on marble | |
| S12 | 0:18.0–0:24.5 | 6–7 | Distant 1980s Delhi traffic, Ambassador car horn | −30 dB, outside the window |
| S13 | **0:25.2** | 8 | **Stamp THUD** + sub-bass hit (40 Hz) | Layer a wooden desk thump with a kick drum |
| S14 | **0:26.05** | 8B | **Iron gate CLANG** + long metallic reverb tail | The tail runs into Shot 9 |
| S15 | 0:27.0–0:29.0 | 9 | Desert wind, creaking hinge, a lone crow | |
| S16 | 0:29.0–0:31.0 | 10 | Distant temple bell, breeze, prayer-bead clicks | |
| S17 | 0:31.6 | 11 | Gold ring drop and bounce on wood | Exaggerate the metallic ring |
| S18 | 0:32.4 | 11 | Low male laughter + glasses clink | |
| S19 | 0:33.5–0:36.0 | 12 | Folder flap, distant typewriter, telex chatter | |
| S20 | 0:36.0–0:39.0 | 13 | Crane motor, chains, steam hiss, a **distant ship horn** at 0:37.5 | Foreshadows S26 |
| S21 | 0:39.0–0:39.6 | 14 | **Dead silence** | Mute everything |
| S22 | 0:39.6 / 0:40.4 | 14 | **Rotary phone bell TRRRING ×2** | Loud, dry, mechanical: the loudest moment since the THUD |
| S23 | 0:41.1 | 14 | Receiver lift, clunk | Cuts off the bell |
| S24 | 0:41.5–0:46.0 | 15–16 | Phone line hiss, telex hum, fluorescent buzz | Low |
| S25 | 0:46.2–0:47.5 | 17 | Paper rustle, fingertip tap | Then **total silence from 0:48.0 to 0:49.0** |
| S26 | **0:49.0–0:51.0** | 18 | **Ship's horn**: huge, low, long | The main low-end event before the BOOM. Hard cut in, no fade |
| S27 | 0:49.0–0:54.5 | 18–19 | Snow wind, distant gulls, lapping water | |
| S28 | 0:51.7 / 0:52.3 / 0:52.9 | 19 | Boot crunches on snow ×3 | Close-miked, heavy |
| S29 | 0:53.6 | 19 | Coat fabric swish + a tiny metallic "ting" for the ring glint | |
| S30 | 0:54.5–0:56.7 | 20 | Wind dropping away, a soft smoke whoosh | Clear space for Rocky |
| S31 | 0:56.4–0:56.7 | 20 | **Reverse riser** into the cut | Ends 1 frame before the silence |
| S32 | **0:57.0** | 21 | **BOOM**: orchestral hit + sub-drop + taiko | Peak moment |
| S33 | 0:57.4 / 0:57.8 | 21 | Two smaller metallic "shing" hits for CHAPTER 3 and THE GLOBAL EMPIRE | |
| S34 | 0:57.0–0:59.7 | 21 | Ember crackle, low wind tail | |

**Sources:** generate SFX with ElevenLabs Sound Effects (text-to-SFX, e.g. *"1970s rotary telephone bell ringing twice, dry close mic"*) or use royalty-free libraries. Check each library's licence for social-media use.
