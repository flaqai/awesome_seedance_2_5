# Seedance 2.5 Use-Case and Prompt Finder

[Home](../README.md) · [72 prompt recipes](../prompts/README.md) · [Prompting guide](prompting-guide.md) · [Flaq AI workflow](flaq-ai-api-guide.md)

Choose a business goal first, then narrow the prompt by available assets, delivery format, and first-pass quality checks.

## Find a prompt by goal

| Goal | Recommended recipe IDs | Preferred starting mode | First review priority |
|---|---|---|---|
| Brand awareness | 25 library membership, 26 repair festival, 27 multi-format campaign | Reference-to-video | Mood, natural performance, format continuity |
| Ecommerce conversion | 04 sparkling tea, 28 folding bottle, 30 product rotation | Image-to-video | Product geometry, labels, feature action |
| Product education | 06 wearable, 29 cushion cutaway, 37 focus timer | Image-to-video | Correct steps, stable structure, accurate UI |
| Vertical UGC | 07 commuter bag, 08 travel diary, 09 restaurant review | Portrait reference | Speech, handheld feel, credible reactions |
| Fashion and beauty | 31 raincoat, 32 scarf styling, 33 lipstick material | Person + product | Identity, cloth physics, skin tone, item structure |
| Cinematic storytelling | 01 rescue, 02 reunion, 03 weather station | Text- or image-to-video | Timeline, blocking, spatial continuity |
| Animation prototype | 10 paper fox, 11 clay robot, 36 fabric creature | Image-to-video | Silhouette, material, limb count |
| Sports and movement | 13 climbing, 14 tennis, 15 dance | Text + action reference | Plausible physics, action order, safety |
| Music and ASMR | 16 jazz, 17 bakery, 18 radio | Audio-visual | Action sync and layer balance |
| Social creative | 40 lemon transition, 41 office-chair comedy, 42 sock detective | Text / multi-scene | Rhythm, prop continuity, clear payoff |
| Education and training | 43 wetland, 44 drill press, 45 micro-world | Diagram / person reference | Factual accuracy, disclaimer, readable labels |
| Real estate and architecture | 20 parallax, 46 apartment, 48 courtyard | Image-to-video | Honest scale, geometry, doors and furniture |
| Accessibility prototype | 38 route app, 47 café circulation, 57 exit reminder | UI / white model | Viable path, inclusive framing, no invented compliance claim |
| Mobility and robotics | 49 cargo bike, 50 sleeper train, 51 delivery robot | Product + action | Structure, road safety, motion physics |
| Nature and pets | 52 senior dog, 53 moth, 54 tomato growth | Image / multi-day reference | Species or identity, welfare, time continuity |
| Industry and logistics | 55 radio assembly, 56 cold parcel | Multi-step reference | Part count, process order, safe operation |
| Hospitality and events | 23 lobby previs, 58 cabin, 59 booth, 60 silent disco | White model / location | Honest space, no invented amenities, circulation |

## Advanced English workflow shortcuts

| Need | Recipe IDs | What the prompt protects |
|---|---|---|
| SaaS and service onboarding | 61 launch film, 68 telehealth onboarding, 70 parcel tracking | Approved UI states, exact copy, no invented metrics or personal data |
| Creator and audio promotion | 62 creator course, 69 multilingual podcast | Authorized identity and voice, credible delivery, no testimonials or voice cloning |
| Ecommerce and hospitality detail | 63 furniture assembly, 64 silver ring, 65 seasonal menu | Part count, geometry, material, ingredients, honest product behavior |
| Culture and public education | 66 museum teaser, 67 energy explainer | Artwork integrity, accurate labels, no implied endorsement or unsupported claims |
| Accessibility and inclusive events | 71 live-event welcome | Real routes and features, respectful agency, no fabricated compliance claim |
| Original entertainment concept | 72 indie game reveal | Character silhouette, level geography, reference separation, no franchise resemblance |

## Choose by available input

| What you have | Start with | Prompt strategy |
|---|---|---|
| Text idea only | [Text-to-Video](https://flaq.ai/models/bytedance/seedance-2-5-text-to-video/) | Fully define subject, world, timeline, camera, sound, and final frame |
| One product image | [Image-to-Video](https://flaq.ai/models/bytedance/seedance-2-5-image-to-video/) | Lock geometry, label region, material, part count, and liquid level |
| One portrait | Image-to-video | Lock face, hair, age, body proportions, wardrobe, and expression range |
| Several character and location images | Reference-to-video | Give every asset one job and state priority when references conflict |
| UI screenshots | UI image-to-video | Preserve approved text, state, controls, and interaction order |
| First and end frames | Image-to-video | Define each frame's role and the physical transition between them |
| Existing clip to modify | Video editing workflow | Change one dimension and repeat every invariant |
| Audio or rhythm reference | Audio-visual workflow | State whether it controls timing, ambience, dialogue, or music only |

## First-pass acceptance test

1. Identity, wardrobe, product shape, labels, and object count remain stable.
2. Doors, walls, furniture, foreground occlusion, and travel direction remain coherent.
3. Actions have plausible weight, contact, inertia, and recovery.
4. The camera follows one understandable path and reaches a deliberate stop.
5. Dialogue, ambience, foley, and music are separated and synchronized.
6. Only approved, legible text appears; no invented claims, logos, or prices.
7. Likeness, asset, music, trademark, safety, and advertising rights are reviewed.
