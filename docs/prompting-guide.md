# Seedance 2.5 Prompting Guide: From Brief to Usable Video

[Home](../README.md) · [72 prompt recipes](../prompts/README.md) · [Flaq AI workflow](flaq-ai-api-guide.md) · [15-language directory](../prompts/i18n/README.md)

A useful video prompt is a production brief with testable instructions. It tells the model what to preserve, what changes over time, how the camera observes it, what should be heard, and what makes the result unacceptable.

## The nine-part prompt anatomy

| Part | Question to answer | Example |
|---|---|---|
| Mode | What kind of generation is this? | Image-to-video using one product anchor |
| Goal | Where will the clip be used? | 15-second vertical ecommerce feature demo |
| References | What job does each asset have? | Image 1 locks packaging; Image 2 controls the set only |
| Anchors | What must remain recognizable? | Bottle silhouette, cap, blank label, liquid level |
| Timeline | What happens, and when? | Macro detail → orbit → feature action → clean hero frame |
| Camera | Where does it start, travel, focus, and stop? | Eye-level medium shot, 20-degree arc, slow rack focus |
| Physics | How should matter and bodies behave? | Real weight, stable contact, one wind direction |
| Audio | What is heard and when? | Cap click at 00:08, fine bubbles, low original rhythm |
| Avoid | What failures invalidate the result? | No redesign, duplicates, fake text, clipping, watermark |

## Write for time, not just appearance

Avoid stacking events with “then” until the model has no pacing guidance. Use time ranges or numbered beats.

```text
00:00–00:04 — Establish the place and visual rule.
00:04–00:10 — Perform the primary action with one camera move.
00:10–00:15 — Introduce a reaction, reveal, or proof point.
00:15–00:20 — Decelerate into a deliberate final composition.
```

For a short clip, one strong action is usually better than four unrelated actions. If a beat needs a location change, costume change, complex VFX, and dialogue at once, split it into another generation.

## Camera direction that can be verified

Use camera terms only when they change the result. Combine the shot size, height, path, speed, focus behavior, and end position.

| Direction | Useful wording | Common conflict |
|---|---|---|
| Push in | Slowly move from medium shot to close-up | Also asking for “camera fixed” |
| Pull back | Reveal context without changing subject scale abruptly | Unspecified final framing |
| Track | Travel parallel with the subject at matching speed | Subject changes direction repeatedly |
| Orbit | Arc by a stated angle around a stable anchor | Full 360° plus multiple scene changes |
| Crane | Raise or lower while preserving geography | Teleporting from low macro to aerial view |
| Pan / tilt | Rotate from a fixed camera position | Mixing with a dolly move unintentionally |
| Rack focus | Move focus between named foreground/background anchors | No clear focal subjects |
| Handheld | Add restrained human micro-movement | “Perfectly locked tripod” in the same prompt |

## Separate three kinds of motion

```text
Subject motion: the cyclist pedals steadily, looks left once, then brakes.
Environmental motion: light rain falls diagonally; tree leaves follow the same wind.
Camera motion: track parallel at waist height, then decelerate to a locked side view.
```

This separation reduces contradictions and makes revisions precise. If the first result fails, you can change only the affected layer.

## Assign one job to every reference

Weak:

```text
Use all images as reference and make it cinematic.
```

Stronger:

```text
Image 1 locks the adult character's face, hair, age, and body proportions.
Image 2 controls only the coat: length, collar, seams, belt, and fabric.
Image 3 controls only the rainy bridge environment and cold color palette.
Do not copy the person, signage, or camera angle from Image 3.
```

When references disagree, write the priority explicitly. Never expect the model to guess whether identity, clothing, composition, or style is more important.

## Preserve identity, products, UI, and architecture

### People and characters

- lock face shape, apparent age, hair, body proportions, clothing, and accessories;
- limit expression range and specify gaze, hand use, and body balance;
- avoid simultaneous profile changes, costume changes, and extreme camera motion.

### Products

- lock silhouette, part count, materials, label region, color, liquid level, and closure;
- describe exactly which part moves and which remains fixed;
- reject extra products, altered seams, melting geometry, mirrored labels, and floating contact.

### User interfaces

- supply approved states instead of asking the model to invent screens;
- quote only the copy that must appear and keep transitions short;
- reject fabricated analytics, controls, ratings, notifications, and microtext.

### Architecture and interiors

- lock the floor plan, doors, windows, furniture count, room connections, and daylight direction;
- use human-eye perspective when honest scale matters;
- reject ultra-wide stretching, wall crossings, added rooms, and invented views.

## Sound prompting

Write audio as independent layers and attach important sounds to visible actions.

```text
Dialogue: one natural sentence from the presenter at 00:05; no voice-over overlap.
Ambience: quiet morning café, distant street, no crowd roar.
Foley: cup contact at 00:03 and zipper close at 00:09, synchronized to the hands.
Music: original minimal percussion, low under dialogue, clean ending at 00:15.
```

If sound is not needed, say so. A visually precise silent clip is easier to finish in post than an output with conflicting narration or unlicensed-sounding music.

## Negative constraints that help

Use concrete failure conditions, not a generic wall of negative adjectives.

```text
No additional people or products.
No face, wardrobe, label, or object-count drift.
No hands passing through objects or feet sliding on the floor.
No camera teleportation, sudden lens change, or unexplained scene cut.
No invented statistics, health claims, prices, logos, subtitles, or watermark.
```

The avoid list should protect the brief. It cannot rescue contradictory positive instructions.

## Troubleshooting by symptom

| Symptom | Likely cause | First revision |
|---|---|---|
| Identity drifts | Too many references or extreme pose change | Name one identity anchor and reduce pose/camera complexity |
| Product redesigns itself | Shape was described only as a style | List geometry, parts, material, label region, and invariants first |
| Camera jumps | Several paths compete | Keep one path with a start and stopping point |
| Motion feels weightless | Action lacks contact and inertia | Add support, balance, impact, drag, and recovery cues |
| Text is garbled | Too much generated typography | Supply one approved text state or add typography in post |
| Audio feels random | Sound has no layer or timing | Separate dialogue, ambience, foley, and music with sync events |
| Final frame is unusable | Prompt ends on action | Reserve the last seconds for deceleration and composition |
| Localization feels literal | Only nouns were translated | Localize speech rhythm, units, UI direction, gestures, and restrictions |

## A practical iteration ladder

1. **Anchor test:** confirm identity, geometry, composition, and object count.
2. **Motion test:** add only the primary subject action and physical behavior.
3. **Camera test:** add one coherent move and a clear stop.
4. **Timing test:** divide the clip into beats and remove overloaded events.
5. **Audio test:** add synchronized foley, ambience, dialogue, then music.
6. **Delivery test:** check aspect-ratio safety, final frame, rights, claims, and platform requirements.

Change one category at a time. Keep the prompt version, source assets, model settings, seed when available, and review notes together.

## Reusable prompt brief

```text
PROJECT
Use: [ad / social / explainer / story / previs]
Audience: [who]
Duration and ratio: [seconds], [aspect ratio]
Desired response: [emotion or action]

REFERENCES
Image 1: [one job and invariants]
Image 2: [one job and invariants]
Priority if references conflict: [rule]

DIRECTION
World: [place, time, weather, light, palette]
Subject: [identity or product anchors]
Timeline: [timed beats]
Camera: [start, path, speed, focus, stop]
Physics and performance: [contact, weight, gaze, hands, cloth, liquid]
Audio: [dialogue, ambience, foley, music, synchronization]

QUALITY GATE
Must preserve: [continuity list]
Must avoid: [specific invalidating failures]
Final frame: [composition and negative space]
```

Start with the [72-scene prompt finder](../prompts/README.md), then adapt the closest recipe instead of writing from a blank page.
