# PART 3 — AI IMAGE GENERATION PROMPTS

## 3.0 Workflow (do this order or consistency will fail)

1. **Generate the four character reference sheets first (3.1).** Use one fixed seed per character and regenerate until you have a face you like. Then save:
   - a front portrait
   - a 3/4 portrait
   - a side profile
   - a full-body costume shot
2. **Lock the sheets as references.** Feed them to every shot image as a *character/omni reference*. Use whatever your tool calls it: Midjourney `--oref`, Flux Kontext / Seedream / Nano Banana with the reference image attached, Kling "Elements", or the ElevenLabs image models with a reference image. Reference weight: 70–85 for faces.
3. **Generate each shot's start frame (3.2).** Generate at **16:9, 1920×1080 or higher**, and keep the action inside the central 2.39 band. Where the video tool supports it, also make an end frame for the shots marked ★.
4. **Text inside images** (CLASSIFIED, CLOSED, OWNER: UNKNOWN, and so on) still breaks often. Generate the prop *blank* if the text comes out wrong, and add the text in the editor as a tracked overlay (Part 7).
5. Append the **global style suffix** and the **negative prompt** to every prompt.

### Global style suffix (append to every prompt)
```
shot on 35mm anamorphic film, early-1980s period production design, photorealistic, cinematic colour grade of crushed blacks, antique gold highlights and cold steel-blue shadows, fine film grain, natural skin texture, high dynamic range, dramatic motivated lighting, subject composed inside the central 2.39:1 band of a 16:9 frame, ultra-detailed, 8k
```

### Universal negative prompt
```
cartoon, anime, 3d render, CGI look, plastic skin, airbrushed, waxy face, doll eyes, deformed face, asymmetrical eyes, cross-eyed, extra fingers, missing fingers, fused fingers, six fingers, malformed hands, extra limbs, duplicated person, warped body, long neck, distorted anatomy, garbled text, misspelled text, random letters, watermark, logo, signature, subtitles, frame border, modern smartphone, LED lights, flat-screen monitor, modern car, contemporary clothing, sneakers, oversaturated, neon colours, HDR halo, blown highlights, low resolution, blurry, jpeg artifacts, motion smear, tilted horizon, resemblance to any real actor, celebrity likeness, real politician likeness
```

---

## 3.1 Character consistency references

> These are **original** character designs. Do not name or prompt any real actor or politician. The character is recognised by his costume, hair and attitude, not by copying a real face.

### ROCKY — reference sheet prompt
```
Character reference sheet, four views on a neutral dark-grey studio background: front portrait, three-quarter portrait, left side profile, full-body standing. An original fictional Indian man, age 36, South Indian features, deep warm-brown skin, strong angular jaw, high cheekbones, slightly hooded intense dark-brown eyes, thick straight eyebrows, a small faded scar through the left eyebrow, thick black wavy hair swept back and falling to the shoulders, full dense black beard trimmed to 4 cm with a clean sharp cheek line, broad-shouldered lean muscular build, 6 ft tall. Costume: black wool double-breasted long overcoat reaching the knees, black three-piece suit underneath, black shirt with no tie, black leather lace-up boots, a heavy gold signet ring on the right index finger engraved with a bold serif letter "R", a thin gold chain wristwatch on the left wrist. Expression: calm, confident, faint dangerous half-smile. Photorealistic, cinematic soft key light, 35mm film look.
```
**Locked identifiers:** shoulder-length swept-back wavy hair · 4 cm beard · left-eyebrow scar · gold "R" signet ring on the **right index finger** · black knee-length overcoat · black boots.

### RAMIKA SEN — reference sheet prompt
```
Character reference sheet, four views on a neutral dark-grey studio background: front portrait, three-quarter portrait, right side profile, full-body standing. An original fictional Indian woman politician, age 56, fair-wheatish skin, oval face, sharp straight nose, thin firm lips, piercing light-brown eyes with fine crow's feet, salt-and-pepper black hair pulled into a tight low bun at the nape, small gold stud earrings, a single thin gold bangle on the right wrist, rectangular thin gold-rimmed reading glasses hanging on a chain around her neck. Costume: a muted ivory handloom cotton-silk saree with a narrow deep-maroon border, a three-quarter-sleeve maroon blouse, a charcoal-grey pashmina shawl draped over the left shoulder. Posture: upright, still, regal. Expression: cold, controlled, unreadable. Photorealistic, cinematic soft key light, 35mm film look.
```
**Locked identifiers:** ivory saree with maroon border · charcoal shawl on the **left** shoulder · low bun · reading glasses on a chain · one gold bangle on the **right** wrist.

### THE NARRATOR — reference sheet prompt
```
Character reference sheet, four views on a neutral dark-grey studio background: front portrait, three-quarter portrait, left side profile, seated at a desk. An original fictional Indian writer and journalist, age 74, wheat-brown skin with deep wrinkles and age spots, kind but haunted dark eyes, a long thin face, sparse white hair combed back, a neatly trimmed white beard and moustache, round thin gold-rimmed spectacles. Costume: a cream khadi kurta, a brown sleeveless Nehru-style wool waistcoat, an old silver wristwatch with a leather strap on the left wrist. Expression: tired wisdom, quiet knowing. Photorealistic, warm tungsten key light, 35mm film look.
```
**Locked identifiers:** round gold spectacles · white beard · cream kurta + brown waistcoat · silver watch on the left wrist.

### INTELLIGENCE OFFICER — reference sheet prompt
```
Character reference sheet, four views on a neutral dark-grey studio background: front portrait, three-quarter portrait, right side profile, full-body standing. An original fictional Indian intelligence officer, age 45, medium-brown skin, round face, thick black moustache, receding side-parted oiled black hair, worried heavy-lidded eyes, slightly overweight. Costume: a grey-blue 1980s safari suit with four front pockets, a white undershirt visible at the collar, a black wristwatch, a government ID card clipped to the left breast pocket. Expression: nervous, dutiful. Photorealistic, cinematic soft key light, 35mm film look.
```
**Locked identifiers:** grey-blue safari suit · thick moustache · ID card on the **left** pocket. *Shot 15 variant: the top button is undone and there is sweat on his forehead.*

### Recurring props (generate these once and reuse them as references)
- **Rocky photograph:** a black-and-white 8×10 print of Rocky in a black suit, front portrait, slightly creased. Use it in shots 4, 7 and 12.
- **Gold "R" ring:** heavy 22k yellow-gold signet ring with a flat oval face and a deep-engraved serif "R". Use it in shots 11 and 19.
- **Red rotary phone:** a 1970s bakelite rotary telephone, glossy crimson. Use it in shot 14.

---

## 3.2 Per-shot image prompts (start frames)

> Every prompt is self-contained. Paste the prompt, then the **global style suffix**, and use the **universal negative prompt**. Attach the character reference where one is listed.

### SHOT 1 — Typewriter
```
Extreme macro close-up of a 1970s black manual typewriter's metal type-bar striking off-white aged paper, a single typed line reading "CLASSIFIED — K.G.F." in a typewriter monospace font with red-black ink, slightly uneven letter impressions, visible paper fibres, a single hard top light falling on the paper, everything else in deep black shadow, shallow depth of field, mysterious and ominous mood.
```
*Reference: none. If the text fails, generate blank paper and type it in the editor.*

### SHOT 2A ★ — Storm aerial
```
Extreme wide aerial drone view looking down at 60 degrees onto a violent night storm over the Indian Ocean, gigantic black waves with white foam, a large 1970s rust-red-and-black cargo ship listing 30 degrees with its bow already underwater, a few flickering amber deck lights, cargo containers sliding off the deck, a jagged lightning bolt striking the sea behind it lighting the clouds violet-white, heavy rain streaks, cold blue moonlight, the ship positioned on the lower-right third, epic scale, disaster-film realism.
```
*End frame ★: the same view, with the ship's bow deeper and the stern rising.*

### SHOT 2B — Gold sinking
```
Underwater cinematic shot in deep dark ocean water, seven heavy gold bullion bars stamped with a small crown emblem tumbling slowly downward diagonally from upper left to lower right, tiny air bubbles and a silt cloud rising, a single diffuse shaft of cold light coming from the surface above, the gold glinting warm against teal-black water, floating particles, sense of loss and finality.
```

### SHOT 3 — Radio
```
Medium shot of an old 1960s wooden valve radio with a glowing amber tuning dial, a cream cloth speaker grille and bakelite knobs, standing on a dusty wooden shelf in a dark Indian home at night, a small brass kerosene lamp burning softly out of focus on the right, the dial glow and lamp flame as the only light sources, warm antique-gold tones, deep shadows, nostalgic and ominous mood.
```

### SHOT 4 — The End (top-down)
*Reference: Rocky photograph prop; narrator sheet (hand and wrist only).*
```
Top-down 90-degree overhead shot of an old teak writer's desk at night, in the centre a thick hand-written manuscript whose final page reads "THE END" in ink, an elderly man's wrinkled hand with a silver leather-strap watch resting on it as it closes, a black-and-white photograph of a bearded long-haired man in a black suit at the upper left, faded cardboard files tied with red string labelled "K.G.F.", yellowed 1980s newspapers, a fountain pen, a green-shaded brass banker's lamp casting a warm pool of light from the left with deep falloff into shadow, symmetrical composition, melancholic storybook mood.
```

### SHOT 5 — Narrator profile
*Reference: narrator sheet.*
```
Side-profile close-up of an original elderly Indian writer, 74 years old, facing frame left, white trimmed beard, sparse combed-back white hair, deep wrinkles, wearing a cream khadi kurta and a brown wool waistcoat, holding round thin gold-rimmed spectacles in his right hand just removed from his face, eyes looking into the distance with sad knowing wisdom, his face on the right third of the frame, out-of-focus wooden bookshelves behind, warm lamp key light from the front-left and a soft cool rim light from a window behind, shallow depth of field, intimate and grave mood.
```

### SHOT 6 ★ — PM's office wide
*Reference: Ramika sheet (from behind), officer sheet.*
```
Wide slightly-low-angle shot of a grand early-1980s Indian Prime Minister's office at dusk, tall arched colonial window showing a hazy Delhi skyline with a cold blue sky, an original Indian woman politician in her fifties standing at the window with her back to camera, wearing an ivory saree with a maroon border and a charcoal shawl on her left shoulder, hair in a low bun, a near-silhouette, at the left third; at the right edge an Indian intelligence officer in a grey-blue safari suit standing respectfully just inside a tall teak door, a heavy teak desk with a green-shaded lamp, an Indian flag on a stand, framed portraits on the walls, polished marble floor reflecting the light, vast negative space, cold blue and warm tungsten contrast, tense quiet atmosphere.
```

### SHOT 7 — Ramika close-up
*Reference: Ramika sheet.*
```
Close-up of an original 56-year-old Indian woman politician seated at a desk, salt-and-pepper hair in a tight low bun, small gold stud earrings, reading glasses hanging on a chain, ivory saree with a maroon border and a charcoal shawl over her left shoulder, looking down with cold controlled satisfaction at a black-and-white photograph of a bearded long-haired man lying blurred in the lower foreground, her face on the left third, slight high angle, hard side light from a desk lamp leaving half her face in shadow, cold steel-blue shadows, authoritative and chilling mood.
```

### SHOT 8 — CLOSED stamp
```
Top-down macro shot of a worn manila government file folder labelled "K.G.F. — TOP SECRET" in typed letters, a wooden-handled rubber stamp pressing down onto the cover leaving a fresh bold red ink stamp reading "CLOSED" inside a rectangular border, a woman's hand with a thin gold bangle holding the stamp, warm desk-lamp light, the red ink as the most saturated colour, crisp detail, decisive and final mood.
```
*If "CLOSED" comes out garbled, generate the stamp mid-air over a blank file and composite the text.*

### SHOT 8B — Iron gate
```
Low-angle frontal shot of a massive rusted riveted iron double gate at the entrance of an old Indian gold mine, the two halves slamming together at the centre, a burst of dust and rust flakes in the air, a heavy chain swinging, a faded painted sign above reading "K.G.F.", harsh overcast daylight, desaturated sepia tones, brutal finality.
```

### SHOT 9 — Silent mines
```
Eye-level wide shot of an abandoned 1980s Indian gold mine complex, broken iron gates hanging off their hinges, rusted conveyor belts, a tall steel mine-shaft headframe against a hazy sky, empty ore carts on rusted rails, dust blowing across cracked red earth, no people, sun-bleached washed-out gold palette, eerie silence and decay.
```

### SHOT 10 — Settlement elders
*Reference: none (one-off extras). Keep the Rocky portrait consistent with the Rocky sheet.*
```
Medium shot in a poor mining settlement of mud-brick huts with tin roofs, three elderly Indian mine workers with grey stubble, thin weathered faces and faded cotton shirts and lungis sitting silently on a wooden bench, one holding prayer beads, behind them on a whitewashed wall a large faded hand-painted portrait of a bearded long-haired man in a black suit, in the right foreground slightly out of focus a barefoot 8-year-old boy in a torn vest standing and gazing at a distant mine headframe, late golden afternoon light, dust in the air, nostalgic and sorrowful mood.
```

### SHOT 11 — Warehouse, the ring
*Reference: ring prop.*
```
Slightly low-angle shot across a round wooden table in a dark derelict warehouse, a single bare tungsten bulb hanging above, cigarette smoke haze, in sharp foreground focus at the centre a heavy gold signet ring engraved with a serif letter "R" lying on the wood with a small brown paper luggage tag tied to it by string, the tag handwritten "RECOVERED — WRECK SITE", behind it five menacing men in 1980s suits and safari suits, faces half in shadow, two laughing, raising crystal whisky glasses in a toast, a sickly yellow-green palette, sinister celebratory mood.
```

### SHOT 12 — World map
*Reference: Rocky photograph prop.*
```
Interior of a 1980s foreign intelligence office, a large paper world map pinned to a corkboard wall, sixteen countries marked with red push pins all connected by taut red string to a black-and-white photograph of a bearded long-haired man pinned at the centre, in the lower foreground a Caucasian officer's hands with rolled white shirt sleeves opening a buff folder stamped "CLASSIFIED", an ashtray with a smouldering cigarette, a single cold fluorescent tube overhead, green-white tint, smoky air, investigative tension.
```

### SHOT 13 ★ — Cargo port
```
Night shot of a busy 1980s international cargo port, wet concrete reflecting sodium-vapour orange floodlights, a tall dockside crane lifting a large wooden crate stencilled with a small crown emblem, steam drifting, in the sharp foreground a dock worker's gloved hand holding a clipboard with a typed cargo manifest whose bold line reads "OWNER: UNKNOWN", shallow depth of field, cinematic orange and teal, secretive mood.
```
*End frame ★: the same scene with focus pulled to the crane and crate in the background.*

### SHOT 14 — Red phone
*Reference: red phone prop; Ramika sheet (hand only).*
```
Eye-level shot at desk height of a glossy crimson 1970s bakelite rotary telephone on a dark teak desk at midnight, a single green-shaded lamp creating a tight pool of warm light, everything else in deep black, a woman's hand with a thin gold bangle and the edge of an ivory saree reaching in from the left toward the receiver, a closed government file beside the phone, tense nocturnal stillness.
```

### SHOT 15 — Officer sweating
*Reference: officer sheet (Shot 15 variant).*
```
Medium close-up of an original 45-year-old Indian intelligence officer with a thick black moustache and oiled side-parted hair, wearing a grey-blue 1980s safari suit with the top button undone, a government ID card on the left pocket, beads of sweat on his forehead, pressing a black bakelite phone receiver to his right ear, his face on the right third, worried wide eyes, in the soft background a records room with shelves of ledgers and a clattering telex machine, cold green fluorescent light from above, anxious mood.
```

### SHOT 16 — Ramika tight
*Reference: Ramika sheet.*
```
Tight close-up of an original 56-year-old Indian woman politician holding a crimson telephone receiver to her left ear, salt-and-pepper low bun, gold stud earring, eyes narrowing with sudden suspicion, hard lamp key light from below-left lighting half her face, the other half in deep shadow, charcoal shawl edge visible, midnight darkness, intense and dangerous mood.
```

### SHOT 17 — Telex
*Reference: officer sheet (hand and watch).*
```
Extreme macro close-up of a 1980s telex printout on pin-feed paper with perforated edges, monospaced dot-matrix text listing bank transfers, a man's trembling index finger with a black wristwatch visible pointing at the bold line "LAST TRANSACTION: YESTERDAY", cold grey-white fluorescent light, shallow depth of field, shocking revelation mood.
```

### SHOT 18 ★ — Harbour silhouette
*Reference: Rocky sheet (silhouette and coat shape).*
```
Low wide-angle shot of a snow-covered northern European harbour at dawn, thick fog, a colossal black cargo ship bow looming out of the mist and towering over the frame, snow falling, on the wet stone pier in the centre bottom a lone tall man in a long black knee-length overcoat with shoulder-length hair standing with his back to camera, backlit by a single sodium dock lamp that creates a glowing halo and silhouette, frozen bollards and chains, cold blue palette with a single warm backlight, mythic, ominous scale.
```
*End frame ★: the same frame pushed in 15%, the man slightly larger.*

### SHOT 19 ★ — Boots to ring
*Reference: Rocky sheet (boots, coat, ring).*
```
Extreme low angle from ground level of a man's black leather lace-up boots stepping through fresh snow on a stone dock toward camera, snow crunching and spraying, the hem of a long black wool overcoat swinging above, cold blue dawn light, shallow depth of field, menacing powerful arrival.
```
*End frame ★ (separate image):*
```
Low-angle close-up of a man's right hand hanging relaxed at his side against a long black wool overcoat, a heavy gold signet ring engraved with a serif "R" on the index finger catching a warm glint from a dock lamp, snowflakes falling, cold blue background, the ring sharp at the left third, powerful reveal.
```

### SHOT 20 — Rocky reveal
*Reference: Rocky sheet (front portrait) at reference weight 85+.*
```
Centre-framed symmetrical cinematic close-up of an original fictional 36-year-old South Indian man, deep warm-brown skin, strong angular jaw, intense dark-brown eyes looking straight into the lens, thick black wavy shoulder-length hair swept back, a dense 4 cm black beard, a small faded scar through his left eyebrow, snowflakes caught in his hair and beard, the collar of a black wool overcoat turned up, a faint confident dangerous half-smile, thin wisps of fog and cigar smoke drifting across the lower face and clearing, hard warm-gold top-side key light, cold blue fill, strong rim light separating him from a black foggy background, heroic slightly-low angle, legendary comeback mood.
```

### SHOT 21 — Title (build in the editor; this is only a background plate)
```
Pure black background with subtle drifting golden embers and faint smoke, cinematic volumetric haze, empty centre space for a title, dark luxurious atmosphere.
```
*The title text itself is built as typography in the editor (Part 7). Don't AI-generate it.*
