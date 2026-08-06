# Awesome Seedance 2.5 Prompts: Practical Image-to-Video Prompt Guide

[![Seedance 2.5](https://img.shields.io/badge/Seedance-2.5-6C5CE7)](https://seed.bytedance.com/en/seedance2_5)
[![Image to Video](https://img.shields.io/badge/Image--to--Video-Prompt%20Library-FF7A59)](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

[English](README.md) · [简体中文](README_ZH.md) · [日本語](README_JA.md) · [Español](README_ES.md) · [Prompts in 12 languages](prompts/i18n/README.md)

![Original Seedance 2.5 prompt guide hero](assets/seedance-2-5-prompt-guide-hero.png)

An original, production-oriented library of **60 Seedance 2.5 prompts in 12 languages** for image-to-video, text-to-video, reference-to-video, synchronized audio, camera movement, green-screen footage, white-model previs, advertising, ecommerce, UGC, education, real estate, mobility, nature, animation, sports, travel, and cinematic storytelling.

> **Use Seedance 2.5 online:** [Open the Seedance 2.5 Image-to-Video page on Flaq AI](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/)
>
> Availability and parameters may change during rollout. Check the live page for current duration, resolution, sound, and input options.

## What makes a strong Seedance 2.5 prompt?

The official Seedance 2.5 page highlights video generation up to 30 seconds in one pass, two extensions, more precise interpretation of reference videos, broader audio-visual editing, professional camera movement, performance blocking, white-model control, and green-screen editing. A useful prompt should therefore read like a compact directing brief, not a pile of style adjectives.

```text
[Mode] Text-to-video / Image-to-video / Reference-to-video / Edit
[Goal] Use, audience, emotion, duration, aspect ratio
[Reference roles] Image 1 locks identity; Video 1 provides camera path only
[Visual anchors] Subject, wardrobe, product geometry, set, time, palette
[Timeline] Establishment -> action -> turn -> final frame
[Camera] Shot size, height, path, speed, focus, stopping point
[Performance and physics] Gaze, hands, weight, inertia, contact, cloth, water
[Audio] Dialogue, ambience, foley, music, synchronization cues
[Continuity] What must never change
[Avoid] Morphing, duplicates, extra limbs, fake text, logos, watermarks
```

## Three copy-ready examples

### Cinematic storm rescue training

```text
Use the input image as the first frame and only visual anchor. Preserve the identities and orange rain gear of the two adult volunteers, the rescue boat geometry, the number of people, the lighthouse position, and the cold storm lighting.

00:00-00:07: Track steadily from water level behind the boat. The hull rises and falls with real weight; spray briefly crosses the lens guard; the lighthouse beam sweeps through rain.
00:07-00:15: Slide forward along the side to the volunteers' shoulders. The front volunteer points toward the safe channel while the rear volunteer adjusts the throttle.
00:15-00:23: A side wave pushes the boat left. Both lower their center of gravity and correct course. Raise the camera slightly to reveal the passage through the rocks; water inertia and body balance must be physically plausible.
00:23-00:30: Enter calmer harbor water. Push past the volunteers toward the lighthouse and stop on a wide, hopeful final frame.

Audio: stereo rain, waves, engine, two short safety calls, and a very soft low string tone at the end. No casualties, added people, altered boat parts, teleporting camera, text, logos, or watermark.
```

### Premium unbranded sparkling-tea ad

```text
Use the bottle in the input image as the only product anchor. Preserve its silhouette, cap, blank-label proportions, amber liquid level, and lighting. Generate no text.

00:00-00:05: Macro focus on condensation, then rack focus to fine bubbles rising in the liquid.
00:05-00:11: Orbit clockwise by about 35 degrees while slowly pulling back. The ice pedestal refracts accurately; two tea leaves travel in the opposite direction for layered motion. The bottle remains stable.
00:11-00:17: A warm backlight passes behind the bottle. The cap lifts only slightly with a clean click and releases a natural mist, not an explosion.
00:17-00:24: Lower to a subtle hero angle. Droplets fall naturally, then stop on a clean front view with negative space above for post-production copy.

Audio: cap click, fine carbonation, light ice sound, minimal fresh rhythm. No fake text, extra bottles, label drift, melting glass, trademarks, or watermark.
```

### Paper fox leaves a sketchbook

```text
Use the input image as the art and character anchor. Preserve the red paper fox's triangular ears, pointed nose, folds, pencil texture, and proportions; preserve the café table, sketchbook, lamp, rainy window, and cup layout.

00:00-00:07: Pencil lines tremble slightly. The fox blinks and raises one front paw as the camera makes a macro push-in.
00:07-00:14: The fox steps over the page edge, transitioning naturally from flat graphite lines to dimensional folded paper with correct contact shadows.
00:14-00:21: Track parallel as it walks around pencil shavings and studies the steam above the cup.
00:21-00:27: Steam forms a brief path toward the rainy window. The fox trots after it while tiny tabletop droplets react to its steps.
00:27-00:30: It stops at the window with a consistent reflection. Raise the camera and finish on an open-ended sense of departure.

Audio: rain, paper folds, wood contact, and minimal glockenspiel. No extra animals, redesign, franchise resemblance, text, logos, or watermark.
```

## Full prompt library

Open the [60-scene master index](prompts/README.md), the [24-scene foundation library](prompts/prompt-library.md), or the [36-scene extended library](prompts/extended-scenarios.md). Together they cover:

- cinematic drama and science fiction;
- product, skincare, beverage, and wearable ads;
- vertical UGC, travel diaries, and food reviews;
- paper craft, clay animation, and living murals;
- climbing, tennis, and street dance;
- jazz, bakery ASMR, and radio drama;
- portrait micro-expressions, architectural parallax, and start/end frames;
- green screen, white-model previs, reference camera paths, and precise editing.

### Complete prompt files in more languages

- [English](prompts/i18n/prompt-library.en.md), [Traditional Chinese](prompts/i18n/prompt-library.zh-TW.md), [Japanese](prompts/i18n/prompt-library.ja.md), and [Korean](prompts/i18n/prompt-library.ko.md);
- [Spanish](prompts/i18n/prompt-library.es.md), [French](prompts/i18n/prompt-library.fr.md), [German](prompts/i18n/prompt-library.de.md), and [Brazilian Portuguese](prompts/i18n/prompt-library.pt-BR.md);
- [Arabic](prompts/i18n/prompt-library.ar.md), [Russian](prompts/i18n/prompt-library.ru.md), and [Bahasa Indonesia](prompts/i18n/prompt-library.id.md).

Each language file contains six complete, copy-ready recipes rather than translated titles alone. See the [localization rules and language matrix](prompts/i18n/README.md).

## Image-to-video checklist

- Lock identity, wardrobe, product shape, object count, composition, and key-light direction.
- Separate subject motion, environmental motion, and camera motion.
- Give each reference file one job; never say “use everything from all references.”
- Describe the camera's start, path, speed, and final stopping point.
- Reserve the final 4–6 seconds for deceleration and a deliberate end frame.
- Add dialogue, ambience, foley, and music as separate audio layers.
- Use original or properly licensed people, music, products, and visual assets.

## Sources and usage

- [Official Seedance 2.5 capability page](https://seed.bytedance.com/en/seedance2_5)
- [Seedance 2.5 Image-to-Video online page](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/)
- [Official Seedance 2.0 launch notes](https://seed.bytedance.com/en/blog/seedance-2-0-official-launch)

All prompts, scenarios, explanatory copy, and images in this repository were newly created for this collection. The examples avoid celebrity likenesses, third-party brand slogans, and protected fictional characters. Review generated output for copyright, likeness, trademark, audio, safety, and platform-policy compliance before commercial use.

The reproducible visual briefs are documented in [Original Image Prompt Notes](assets/IMAGE_PROMPTS.md).
