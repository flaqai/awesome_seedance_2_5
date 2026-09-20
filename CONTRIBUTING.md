# Contributing to Awesome Seedance 2.5 Prompts

Thanks for helping make the library more practical, multilingual, and original. Contributions should add a real production workflow or improve an existing recipe in a testable way.

## Fastest way to contribute

Use the [guided Prompt Submission form](https://github.com/flaqai/awesome_seedance_2_5/issues/new?template=prompt.yml) for one tested prompt. It asks for the information maintainers need to review the result without requiring you to edit repository files.

Please include:

- one complete prompt and a specific, searchable title;
- generation mode, provider/model, duration, aspect ratio, sound choice, and seed when available;
- every input asset in upload order, with one explicit role per asset;
- the real generated video, GIF, screenshots, or a stable preview link;
- a short note about what worked, what failed, and what changed during iteration;
- the author name or handle that should receive attribution.

If you are contributing several prompts, a new language pack, documentation, or structural changes, open a pull request instead. Keep each submission reviewable and avoid mixing unrelated changes.

## What makes a useful contribution

To suggest a public example for the X video showcase, open an issue with the original status URL, attached video, explicit model-version evidence, and the exact location of the complete prompt. Keep the posting account credited and distinguish a source prompt from an editorial adaptation. Linking third-party media does not transfer its license; see the [showcase source notes](docs/x-showcase-sources.md).

- a complete prompt for a distinct business, creative, education, accessibility, or production scenario;
- a carefully localized version of an existing shared prompt;
- a clearer workflow, troubleshooting note, quality check, or rights safeguard;
- an original reference image plus a reproducible image-generation brief;
- a fix for broken navigation, misleading wording, inconsistent counts, or unreadable formatting.

Please do not submit copied prompt text, scraped collections, celebrity likeness prompts, protected characters, third-party slogans, unlicensed images, unverifiable performance claims, or hidden advertising.

## Prompt recipe format

```text
## ID. Specific scenario title

Mode: Text-to-video / Image-to-video / Reference-to-video / Edit
Format: aspect ratio
Duration: target length

[Input roles and visual invariants]
[Timed beats or clearly ordered actions]
[Camera start, path, speed, focus, and stopping point]
[Performance and physical behavior]
[Dialogue, ambience, foley, music, and synchronization]
[Continuity requirements and specific failure exclusions]
```

A submission should be directly usable after replacing only project-specific subjects, assets, and approved copy. Avoid adjective lists that do not explain action, timing, or camera behavior.

## Localization requirements

1. Preserve the original scene ID and the role of every input asset.
2. Translate camera direction, timing, audio, continuity, and exclusions—not only the title and style words.
3. Keep filenames, model settings, measurements, and approved product names exact.
4. Put required on-screen text in quotation marks and identify its target language.
5. Review speech rhythm, units, gestures, reading direction, accessibility, and cultural context with a fluent speaker.
6. For RTL languages, treat interface reading direction and camera-left/camera-right as separate decisions.

## Originality and rights checklist

- The scenario and wording were created for this contribution.
- Every image, video, voice, music reference, logo, and likeness is original, licensed, or authorized.
- No existing filmmaker, artist, photographer, brand campaign, game, or fictional character is used as a shortcut for style.
- Medical, financial, environmental, safety, accessibility, and product claims are neutral or supported by approved source material.
- Text, trademarks, pricing, legal copy, and credits are reserved for post-production when exact reproduction is required.

## Before opening a pull request

- Check every relative Markdown link.
- Confirm that all fenced prompt blocks are closed.
- Verify headings and IDs against the master index.
- Update prompt, scene, and language counts where relevant.
- Read the prompt once as a director and once as a reviewer: every important instruction should be observable in the output.

## Review and attribution

Submissions are reviewed for usefulness, reproducibility, originality, rights, safety, clarity, and fit with the library. Maintainers may normalize formatting, tighten constraints, change metadata, request evidence, merge overlapping scenarios, or decline material that cannot be verified. Accepted community prompts should retain the contributor's chosen display name and source link where provided.

By contributing, you agree that your contribution may be distributed under this repository's [MIT License](LICENSE).
