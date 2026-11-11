# PART 4 — IMAGE-TO-VIDEO GENERATION PROMPTS (Kling / Seedance)

## 4.0 Rules that apply to every clip

- **Always use image-to-video** with the Part 3 start frame. Text-to-video will drift off-model.
- **Generate 5 s for every clip**, even the 1–2.5 s shots. Most tools have a 5 s minimum and the first and last ~0.5 s are often the weakest. Trim to the best window in the edit. The "Use" column in 4.2 tells you which window to keep.
- **Use start + end frames** on the shots marked ★ in Part 3. That's the most reliable way to control the camera.
- **Settings:** professional/high-quality mode, creativity/"relevance" set toward the prompt (Kling CFG ≈ 0.6–0.7), 24 fps output if offered, 1080p, no auto-extend.
- **One camera move per clip.** If a prompt asks for two moves, the model usually does neither well.
- **Lip-sync:** generate those shots with the **mouth closed or neutral**, then apply lip-sync in a second pass using the final ElevenLabs line (Kling Lip Sync, Sync.so lipsync-2, Hedra, or a similar tool). Never let the video model invent speech.
- **Re-roll budget:** expect 3–6 generations per hero shot (2A, 6, 18, 19, 20) and 1–3 for inserts.

### Universal video negative prompt
```
morphing, face distortion, identity change, flickering, jitter, warping hands, extra fingers, melting objects, sudden camera cuts, zoom pulsing, fast unnatural motion, rubbery skin, talking or mouth moving (unless specified), text changing, modern objects, cartoon, low quality, frame blending
```

---

## 4.1 Per-shot prompts

### SHOT 1 — Typewriter · use 2.5 s · lip-sync: no
```
Macro shot. The typewriter type-bar strikes the paper rhythmically, each strike leaving one new inked letter, the paper advancing slightly left with each letter. Camera: locked off with an imperceptible slow push-in. Environment: dust motes drifting in the single top light. Mood: ominous, deliberate. Keep the background pure black and the existing letters unchanged.
```
*If the typed text morphs, generate the type-bar motion only on blank paper and add the letters as an animated text layer.*

### SHOT 2A — Storm aerial · use 2.5 s (from 1.0 s) · lip-sync: no
```
Aerial view. The cargo ship lists further and its bow sinks deeper into the black waves, the stern slowly rising, containers sliding off the deck into the sea. Massive waves roll and crash across the frame, heavy rain sweeps diagonally. One bright lightning strike flashes, lighting the clouds for a split second. Camera: slow steady lateral drift to the left, no rotation. Mood: catastrophic, epic, cold. The ship keeps its exact design and colours.
```

### SHOT 2B — Gold sinking · use 1.5 s · lip-sync: no
```
Underwater. The gold bars tumble slowly and heavily downward with realistic weight, turning end over end, small bubbles and silt rising past them, the shaft of surface light flickering faintly as lightning flashes far above. Camera: sinks slowly downward with the bars. Mood: silent loss, finality. Gold stays solid with no shape morphing.
```

### SHOT 3 — Radio · use 4.0 s · lip-sync: no
```
The camera dollies slowly and smoothly forward from a medium shot toward the glowing amber radio dial, ending close on the dial. The dial needle trembles slightly, the dial glow pulses faintly as if with the signal, and the kerosene lamp flame in the background flickers gently. No people. Mood: ominous, nostalgic, tense.
```

### SHOT 4 — The End · use 3.5 s · lip-sync: no
```
Top-down view, locked off. The elderly man's wrinkled hand slowly and gently closes the thick manuscript, the pages settle, and the hand rests flat on the closed cover. The lamp light stays steady, with a faint dust drift. Camera: static with an imperceptible slow push down. Mood: melancholic finality. The photo, files and newspapers stay perfectly still and unchanged.
```

### SHOT 5 — Narrator profile · use 4.0 s · lip-sync: no (mouth closed)
```
Side profile close-up. The elderly man slowly lowers his round gold spectacles from his face with his right hand, blinks once slowly, then lifts his eyes slightly into the distance with a sad, knowing expression. Mouth stays closed, no speaking. Subtle natural breathing. Camera: locked off. Background bookshelves softly out of focus. Mood: grave, intimate. Keep facial identity consistent.
```

### SHOT 6 — PM's office wide · use 3.0 s · lip-sync: optional (officer is small)
```
Wide shot. The intelligence officer walks in from the right through the tall door, takes three measured steps on the marble floor and stops, standing straight with his hands at his sides, speaking briefly with minimal mouth movement. The woman at the window stays completely still with her back to camera, looking out at the dusk skyline. Distant city haze moves slightly. Camera: locked off, very slow subtle push-in. Mood: cold, quiet, tense. Both characters keep their costumes exactly.
```

### SHOT 7 — Ramika close-up · use 3.5 s · lip-sync: YES (second pass)
```
Close-up. The woman looks down at the photograph with cold satisfaction, holds still, then slowly lifts her eyes toward the left of camera with a hard, final look. Mouth neutral and closed for lip-sync replacement. Subtle breathing, no head bobbing. Camera: locked off. The lamp light is steady and the shadow on half her face stays constant. Mood: chilling authority. Facial identity must match the reference exactly.
```

### SHOT 8 — CLOSED stamp · use 1.5 s · lip-sync: no
```
Top-down macro. The rubber stamp comes down quickly and firmly onto the file cover, presses for a beat with a tiny bounce of the folder, and lifts away revealing the bold red "CLOSED" mark. Camera: locked off, with a very subtle impact shake on contact. Mood: decisive, final.
```
*If the text warps, generate the motion without text and composite "CLOSED", revealing it as the stamp lifts.*

### SHOT 8B — Iron gate · use 1.0 s · lip-sync: no
```
The heavy rusted iron gate halves swing and slam shut together at the centre with great weight, dust and rust flakes bursting outward, the chain swinging violently. Camera: locked off with a single short impact shake. Mood: brutal finality.
```

### SHOT 9 — Silent mines · use 2.0 s · lip-sync: no
```
Wide shot of the abandoned gold mine. Wind blows dust across the ground, a broken gate creaks slightly on its hinge, loose sheet metal flutters. No people. Camera: slow smooth tracking to the right. Mood: desolate silence.
```

### SHOT 10 — Settlement elders · use 2.0 s · lip-sync: no
```
The three elderly men sit silently on the bench, one slowly turning prayer beads in his fingers, another lowering his eyes. In the foreground the boy stands still, gazing at the distant mine, his hair moving in the breeze. Dust floats in golden light. Camera: gentle handheld sway, no reframing. Mood: quiet sorrow, remembrance. No mouths moving.
```

### SHOT 11 — Warehouse, ring · use 2.5 s · lip-sync: no
```
Across the table, one man's hand drops the gold ring onto the wood where it bounces once and settles beside its tag. Behind it the men laugh silently and raise their whisky glasses in a toast. The bulb sways slightly, smoke drifts through the light. Camera: slow push-in toward the ring. The ring and the engraved R stay sharp and unchanged. Mood: sinister celebration.
```

### SHOT 12 — World map · use 2.5 s · lip-sync: no
```
The camera pans slowly down from the world map with red strings and pins to the officer's hands in the foreground as they open the buff classified folder. Cigarette smoke curls upward from the ashtray, the fluorescent light flickers once faintly. Mood: investigative tension. Map strings and pins remain fixed.
```

### SHOT 13 — Cargo port · use 3.0 s · lip-sync: no
```
Night port. The crane lifts and swings the wooden crate slowly through the floodlit steam. Focus racks smoothly from the crane in the background to the clipboard manifest held in the gloved hand in the foreground, revealing the text. Steam drifts, wet ground reflects the orange lights. Mood: secretive, rising tension. Use start and end frames.
```

### SHOT 14 — Red phone · use 2.5 s · lip-sync: no
```
Midnight, desk height. The red rotary phone sits still, then its bell rings, the handset rattling slightly in its cradle. A woman's hand with a gold bangle reaches in from the left, pauses briefly, then lifts the receiver firmly out of frame. Camera: locked off. Lamp light steady. Mood: dread.
```

### SHOT 15 — Officer sweating · use 3.0 s · lip-sync: YES (second pass)
```
Medium close-up. The officer presses the phone receiver to his ear, swallows nervously, his eyes darting down to papers and back up, a bead of sweat sliding down his temple. Mouth neutral for lip-sync replacement. Camera: slight handheld tremble. The telex in the background prints slowly. Mood: fear, urgency. Keep facial identity.
```

### SHOT 16 — Ramika tight · use 1.5 s · lip-sync: YES (second pass)
```
Tight close-up. The woman holds the receiver to her ear, her eyes narrowing slowly with suspicion, jaw tightening. Mouth neutral for lip-sync replacement. Minimal motion. Camera: locked off. Half her face in hard light, half in shadow. Mood: dangerous stillness.
```

### SHOT 17 — Telex · use 3.0 s · lip-sync: no
```
Extreme macro. A trembling index finger slides slowly down the telex printout and stops on the bold line "LAST TRANSACTION: YESTERDAY", tapping it once. The paper rustles slightly. Camera: slow slide following the finger, then holds still. Mood: shocking revelation. Printed text must remain stable.
```
*If the text warps: track a text overlay onto the blank printout.*

### SHOT 18 — Harbour silhouette · use 2.5 s · lip-sync: no
```
Dawn harbour. Thick fog rolls slowly across the pier, snow falls steadily, the colossal ship bow looms forward almost imperceptibly through the mist. The lone man in the long black coat stands completely still with his back to camera, the coat hem and his hair moving gently in the wind. Camera: slow steady push-in. Mood: mythic, ominous. Use start and end frames.
```

### SHOT 19 — Boots to ring · use 3.0 s · lip-sync: no
**Option A (one clip with start + end frames):**
```
Ground-level extreme low angle. Black leather boots step heavily through the snow toward camera, snow crunching and spraying. The camera then tilts up smoothly along the long black overcoat to the man's right hand at his side, ending on the gold R ring which catches a warm glint of light. Snow falls. Mood: powerful arrival. Use start and end frames.
```
**Option B (more reliable: two clips, cut on the motion):**
- 19-1 (1.5 s): *"Black leather boots step heavily through snow toward the ground-level camera, snow spraying, the coat hem swinging. Camera locked off."*
- 19-2 (1.5 s): *"Close-up of the man's right hand at his side; the fingers flex slightly and the gold R ring catches a warm glint. Camera tilts up slightly. Snow falls."*

### SHOT 20 — Rocky reveal · use 2.5 s · lip-sync: YES (second pass)
```
Centre close-up. Fog and smoke drift slowly across his face from right to left and clear away. His eyes, already looking down, lift slowly to look directly into the lens. A faint confident half-smile forms at one corner of his mouth. Mouth otherwise closed for lip-sync replacement. Snowflakes settle in his hair and beard. Camera: locked off. Lighting steady: gold top key, blue fill, strong rim. Mood: legendary, controlled menace. Facial identity must match the reference exactly; no morphing.
```
*For this shot, generate 6+ takes and choose the one with zero face drift. This shot decides whether the whole teaser works.*

### SHOT 21 — Title background · use 3.0 s · lip-sync: no
```
Pure black background. Small golden embers drift slowly upward with faint smoke wisps curling. Camera: very slow push-in. Mood: luxurious, epic aftermath.
```
*The title is built in the editor.*

---

## 4.2 Generation tracker

| Shot | Gen length | Use | Start/end frames | Lip-sync pass | Takes budget |
|---|---|---|---|---|---|
| 1 | 5 s | 2.5 s | start | — | 2 |
| 2A | 5 s | 2.5 s (from 1.0 s) | ★ start + end | — | 5 |
| 2B | 5 s | 1.5 s | start | — | 2 |
| 3 | 5 s | 4.0 s | start | — | 2 |
| 4 | 5 s | 3.5 s | start | — | 2 |
| 5 | 5 s | 4.0 s | start | — | 3 |
| 6 | 5 s | 3.0 s | ★ start + end | optional | 4 |
| 7 | 5 s | 3.5 s | start | **yes** | 4 |
| 8 | 5 s | 1.5 s | start | — | 2 |
| 8B | 5 s | 1.0 s | start | — | 2 |
| 9 | 5 s | 2.0 s | start | — | 2 |
| 10 | 5 s | 2.0 s | start | — | 2 |
| 11 | 5 s | 2.5 s | start | — | 3 |
| 12 | 5 s | 2.5 s | start | — | 2 |
| 13 | 5 s | 3.0 s | ★ start + end | — | 3 |
| 14 | 5 s | 2.5 s | start | — | 2 |
| 15 | 5 s | 3.0 s | start | **yes** | 3 |
| 16 | 5 s | 1.5 s | start | **yes** | 3 |
| 17 | 5 s | 3.0 s | start | — | 2 |
| 18 | 5 s | 2.5 s | ★ start + end | — | 4 |
| 19 | 5 s (or 2 × 5 s) | 3.0 s | ★ start + end | — | 4 |
| 20 | 5 s | 2.5 s | start | **yes** | 6 |
| 21 | 5 s | 3.0 s | start | — | 1 |
| **Total** | | **60.0 s** | | 4–5 shots | **≈ 65 gens** |
