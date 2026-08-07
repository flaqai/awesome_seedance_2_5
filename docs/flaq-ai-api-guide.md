# Flaq AI + Seedance 2.5: Model and API Workflow Guide

[Home](../README.md) · [72 prompt recipes](../prompts/README.md) · [Advanced prompting guide](prompting-guide.md) · [15-language directory](../prompts/i18n/README.md)

Flaq AI provides model pages that connect prompt experimentation with an API-oriented production workflow. For Seedance 2.5, choose the model by the asset you already have—not by which page sounds more advanced.

> Treat the live Flaq AI model pages as the source of truth for limits, input fields, output behavior, pricing, and API schemas. This guide avoids hard-coding endpoints or request bodies that may change.

## Choose the right Seedance 2.5 workflow

| Starting point | Recommended model page | Best for | Your prompt must supply |
|---|---|---|---|
| An idea, script, or shot list | [Seedance 2.5 Text-to-Video](https://flaq.ai/models/bytedance/seedance-2-5-text-to-video/) | Concept films, social hooks, atmosphere tests, narrative scenes, previsualization | Subject, environment, timeline, camera, motion, sound, final frame |
| A product photo, character sheet, key art, first frame, or end frame | [Seedance 2.5 Image-to-Video](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/) | Product ads, portraits, branded assets, illustration animation, before/after transitions | What the image locks, allowed motion, camera path, continuity, exclusions |

### Use Text-to-Video when

- visual exploration matters more than matching an existing asset;
- you need multiple art-direction options before producing a key image;
- the scene is driven by blocking, atmosphere, or a camera idea;
- you can describe every important object and continuity rule in text.

### Use Image-to-Video when

- identity, packaging, clothing, layout, or composition must remain recognizable;
- you already have approved campaign art or an ecommerce image;
- the first or final composition is part of the brief;
- review depends on comparing the output to a supplied source.

## Controls visible on the Flaq model pages

The current model-page interfaces present the following creative controls. Their exact availability and accepted values may change during rollout.

| Control | What it changes | Prompt-writing implication |
|---|---|---|
| Prompt | The creative and directing brief | Put invariants first, then the timeline, camera, audio, and exclusions |
| Translate | Converts the input prompt for model use | Preserve quoted on-screen copy, proper nouns, units, and asset labels during review |
| Optimize Prompt | Expands or restructures prompt wording | Compare with the original; make sure optimization does not invent products, claims, or shots |
| Enable Sound | Requests audio with the video | Separate dialogue, ambience, foley, and music; identify exact synchronization cues |
| Camera Fixed | Reduces camera movement | Still describe subject and environment motion; avoid contradictory dolly or orbit instructions |
| Seed | Supports repeatable exploration when the service honors it | Keep prompt and settings unchanged while comparing one variable at a time |
| Duration | Sets the clip length | Fit the number of beats to the selected duration; reserve time for deceleration |
| Aspect ratio | Frames the composition for a destination | State safe zones, subject placement, and negative space for post-production copy |
| Resolution | Selects the output size | Validate motion and continuity before spending on final-resolution iterations |
| Start / End Frame | Available in the image-to-video interface | State what each frame controls and describe the transition between them |

## Workflow A: prompt-first text-to-video

1. Pick one outcome: hook, explainer, product mood, story beat, or previs.
2. Write a one-sentence creative contract: audience, emotion, duration, and format.
3. Define the subject and environment with observable details.
4. Break the clip into two to four timed beats.
5. Give the camera one coherent path and a stopping point.
6. Add sound layers only after the visual sequence works.
7. Generate a low-risk exploration, review it, and change one variable per iteration.

```text
Create a [duration] [aspect ratio] video for [audience/use].

Subject and world: [who/what, location, time, lighting, material, palette].
00:00–00:__: [establishing beat and camera start].
00:__–00:__: [main action, performance, and physical reaction].
00:__–00:__: [turn, reveal, or payoff].
Final frame: [composition, emotion, negative space, camera stop].

Audio: [dialogue] + [ambience] + [foley] + [original music direction].
Continuity: [identity, wardrobe, object count, geography, light direction].
Avoid: [morphing, duplicates, anatomy errors, fake text, logos, watermark].
```

## Workflow B: anchor-first image-to-video

1. Confirm that every uploaded asset is original, licensed, or authorized.
2. Assign one explicit job to each image: identity, product, wardrobe, environment, first frame, or end frame.
3. List the visual properties that must never change.
4. Describe allowed movement separately for the subject, environment, and camera.
5. Set contact, weight, inertia, occlusion, cloth, liquid, and reflection behavior where relevant.
6. End on an intentional frame that can be used in editing or as a thumbnail.

```text
Image 1 is the only [identity/product/composition] anchor. Preserve [specific invariants].
Image 2 controls only [wardrobe/environment/end frame]. Do not borrow [excluded properties].

Subject motion: [action, pace, gaze, hands, contact, weight].
Environmental motion: [wind, water, particles, traffic, practical light].
Camera: start at [shot/height], move [single path] at [speed], stop at [final framing].
Timeline: [timed sequence].
Audio: [layers and synchronized events].
Avoid: [reference drift, redesign, extra objects, clipping, fake text, logos, watermark].
```

## Production checklist

- Keep a record of prompt version, input assets, model page, duration, ratio, sound choice, seed, and review notes.
- Test identity and product geometry before adding elaborate effects or multi-character action.
- Check spelling and numbers frame by frame; add final typography in post when exact text is critical.
- Evaluate outputs on continuity, physical plausibility, camera logic, audio sync, and final-frame usability.
- Verify likeness permission, trademarks, music rights, location restrictions, safety claims, and local advertising rules.
- Use the live Flaq pages for the current service status and API documentation; do not depend on screenshots of pre-release controls.

## Continue exploring

- [Seedance 2.5 Text-to-Video on Flaq AI](https://flaq.ai/models/bytedance/seedance-2-5-text-to-video/)
- [Seedance 2.5 Image-to-Video on Flaq AI](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/)
- [72-scene prompt finder](../prompts/README.md)
- [Prompt engineering and troubleshooting](prompting-guide.md)
- [Originality and asset notes](../assets/IMAGE_PROMPTS.md)
