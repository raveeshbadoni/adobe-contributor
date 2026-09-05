# OpenAI Prompt Template — Durga Mata Devotional

Use this template to build each image prompt. Every image must be assembled from a fresh combination of independent attributes. Do not repeatedly reuse one hero portrait formula.

## Batch variation engine

Before generating each image, choose one value from each pool below. Selection should be random or pseudo-random, but the final combination must be checked against all previously approved images in the same batch. If the combination is too similar, redraw one or more attributes before generation.

### Devotional theme pool

Choose one:

1. Durga Mata divine portrait.
2. Durga Mata with lion companion.
3. Durga Mata receiving temple worship from devotees viewed from behind or at a respectful distance.
4. Durga Mata during Navratri mandap celebration.
5. Durga Mata beside a diya-filled altar.
6. Durga Mata in a peaceful temple sanctum.
7. Durga Mata blessing a family or small devotional gathering.
8. Durga Mata at a river-ghat aarti scene.
9. Durga Mata in a celestial divine realm.
10. Durga Mata as a distant sacred presence in a grand environmental scene.

### Environment pool

Choose one and avoid repeating the same environment more than twice in a 20-image batch:

- Himalayan dawn sanctuary.
- Ancient stone temple sanctum.
- Grand temple courtyard at sunrise.
- Navratri floral mandap with marigolds and diyas.
- River ghat at blue hour with floating lamps.
- Lotus lake at golden hour.
- Sacred forest shrine with filtered morning light.
- Palace-like divine throne hall.
- Moonlit temple courtyard.
- Mountain meadow with distant peaks.
- Monsoon temple steps with soft rain atmosphere.
- Desert stone temple at dusk.
- Marigold and diya devotional alcove.
- Celestial cloud realm with restrained sacred geometry and no text.
- Village Navratri courtyard with garba lamps and festive decoration.
- Temple corridor with carved pillars and directional window light.
- Hilltop shrine above clouds.
- Riverside temple at sunrise.
- Flower-filled puja room with brass lamps.
- Wide festival pavilion prepared for Navratri worship.

### Pose/action pool

Choose one and do not repeat the same pose/action in consecutive images:

- Standing frontal blessing.
- Three-quarter standing blessing.
- Seated on an ornate throne.
- Seated on a lotus.
- Calmly accompanied by a lion.
- Riding the lion in a composed devotional presentation.
- Walking through a temple courtyard.
- Protective warrior stance.
- Serene side profile.
- Compassionate maternal blessing gesture.
- Symmetrical centered divine portrait.
- Full-body environmental pose.
- Slightly low-angle heroic devotional pose.
- Seated while devotees perform aarti in the foreground.
- Standing behind a diya-lit altar during puja.
- Blessing devotees during Navratri worship.
- Quiet contemplative pose beside temple lamps.
- Wide distant figure framed by temple architecture.

### Camera/composition pool

Choose one:

- CENTER_HERO — centered medium/full-body symmetry.
- RIGHT_COPY — subject on right third, open lyric space left.
- LEFT_COPY — subject on left third, open lyric space right.
- WIDE_ENV — deity smaller in a large cinematic environment.
- LOW_HERO — slightly low camera angle, full crown/halo safely framed.
- THREE_QUARTER — dimensional three-quarter perspective.
- CLOSE_DEVOTIONAL — face and upper body with controlled visible hands.
- OVER_DEVOTEE_SHOULDER — respectful distant devotee foreground framing, deity/altar in focus.
- ALTAR_FOREGROUND — lamps/flowers in foreground, Durga as primary background subject.
- ARCHITECTURAL_FRAME — pillars/doorway naturally frame the scene.
- HIGH_WIDE — elevated wide environmental composition.
- SIDE_WIDE — lateral cinematic view with strong environmental depth.

A 20-image batch must contain at least 5 different composition profiles, at least 5 WIDE_ENV/architectural/environment-heavy scenes, and at least 6 useful left/right copy-space frames.

### Lighting pool

Choose one:

- Golden sunrise.
- Warm diya illumination.
- Soft temple-window shafts.
- Cool moonlight with warm lamp accents.
- Misty Himalayan dawn.
- Gentle overcast monsoon light.
- Celestial soft radiance.
- Sunset rim light.
- Blue-hour ambient light with warm diyas.
- Early-morning soft natural light.
- Festival string-lamp ambience without readable signs.
- Dramatic but natural side light through temple pillars.

### Attire/color pool

Preserve respectful traditional Durga iconography while varying presentation. Choose a principal palette rather than using identical red in every frame:

- Deep crimson with antique gold.
- Vermilion red with warm gold.
- Maroon with muted gold.
- Saffron-red with ivory accents.
- Ruby red with emerald jewelry accents.
- Red and cream ceremonial textile palette.
- Deep red with subtle royal-blue environmental contrast.

Do not turn color variation into costume fantasy. Traditional sari, crown, jewelry, halo, and devotional dignity remain consistent.

### Iconography pool

Select a coherent traditional hand/object arrangement matching the declared arm count. Prefer 4, 6, or 8 clearly visible arms depending on composition complexity. Possible elements include blessing/open palm, lotus, trident, sword, discus, conch, bow, mace, or another appropriate traditional motif. Fewer cleanly separated objects are preferred over crowding.

## Hard anti-duplication rules

For every candidate, compare it with every previously approved image in the current batch. Reject and regenerate before saving if any of these are true:

1. Same devotional theme + same environment + same pose.
2. Same environment + same composition + same camera distance.
3. Same pose + same composition + same lighting profile.
4. Subject placement, silhouette, lion placement, and background layout are materially similar to an earlier image.
5. The candidate looks like a crop, color-grade variation, mirror, or minor facial-expression variation of an earlier image.
6. More than two images in the batch use the same environment.
7. More than three images use the same dominant pose family.
8. More than four images use a centered hero composition.
9. Consecutive images use the same environment, pose, or composition profile.

The batch should look like 20 separate devotional scenes from one high-quality visual collection, not 20 variations of one poster.

## Quality-first prompt template

Replace every bracketed value with concept-specific content; do not leave unresolved placeholders.

**Purpose:** Create one premium, respectful, cinematic Durga Mata devotional still as a native [ASPECT] source frame for a devotional-song video. This must be a completely independent scene, not a variation of another image. Intended use: [VIDEO_USE]. Copy-space requirement: [COPY_SPACE].

**Devotional theme:** [DEVOTIONAL_THEME]. The scene should communicate devotion, serenity, divine strength, celebration, worship, or sacred atmosphere appropriate to the selected theme.

**Subject:** Durga Mata portrayed with a serene, compassionate, powerful divine presence; refined natural facial detail; traditional [ATTIRE_PALETTE] sari with elegant gold work; ornate traditional crown; luminous controlled halo; traditional jewelry; [ARM_COUNT] intentionally visible and anatomically coherent arms; [LION_DESCRIPTION]. Hand and symbolic-object assignments: [HAND_OBJECT_MAP]. Every hand has a clear readable silhouette and physically plausible connection to the body.

**Pose/action:** [POSE_DESCRIPTION]. Body orientation: [ORIENTATION]. Expression: [EXPRESSION]. If devotees are present, show them respectfully and naturally, generally from behind, side, or at a non-dominant distance so Durga Mata remains the devotional focus. Keep blessing gestures, symbolic objects, crown, halo, and lion clearly separated and fully readable.

**Environment:** [SCENE_DESCRIPTION]. Build one specific, coherent, physically believable sacred environment with layered foreground, midground, and background. Use scene-appropriate stone, flowers, brass lamps, textiles, water, vegetation, architecture, festival decoration, mountains, clouds, or temple elements. No readable signage or script.

**Composition:** [COMPOSITION_PROFILE], [CAMERA_DISTANCE], native [ASPECT]. Place Durga Mata [SUBJECT_PLACEMENT]. Preserve [COPY_SPACE] clean visual space where requested. Use intentional cinematic depth and strong visual hierarchy. Keep crown and halo comfortably below the upper frame edge; keep important hands, symbolic objects, lion face/paws, garment edges, lamps, and devotees safely inside the frame.

**Lighting:** [LIGHTING_PROFILE]. Use physically coherent directional light, controlled highlights on gold and jewelry, natural skin rendering, readable eyes and hands, detailed fabric, balanced halo exposure, realistic volumetric atmosphere only when justified by the environment, and clean shadow structure. Avoid flat poster lighting and excessive glow.

**Image quality and art direction:** Premium cinematic devotional realism, highly resolved natural facial detail, believable skin texture, realistic fabric weave, finely crafted jewelry and metal, clean architectural detail, realistic flowers and lamps, accurate depth and perspective, nuanced color separation, subtle atmospheric perspective, controlled depth of field, crisp primary subject without oversharpening, polished high-end devotional-film key-art quality while remaining a natural scene rather than a poster. Do not imitate any specific copyrighted artwork, film depiction, living artist, photographer, or identifiable performer.

**Uniqueness instruction:** This image must differ materially from all other images in the batch in at least four of these dimensions: devotional theme, environment, pose/action, camera angle, camera distance, composition profile, subject placement, lighting profile, lion presence/placement, devotee presence, foreground elements, and dominant spatial layout. Do not reuse the same temple/Himalayan/lion hero setup unless the combination is otherwise clearly different.

**Constraints:** Exactly one final image only. No collage, grid, contact sheet, montage, split screen, border, inset, or multiple panels. No text, Hindi/Devanagari characters, English letters, Om symbol rendered as text, pseudo-script, signatures, logos, trademarks, brands, labels, banners, captions, or watermarks. No duplicated face, unintended extra arms, missing declared arms, fused arms, fused hands, malformed fingers, impossible joints, duplicated symbolic objects, floating weapons, floating jewelry, objects intersecting the face/body, weapon tips touching frame edges, broken lion anatomy, duplicate lion features, deformed paws, cropped crown, cropped halo, clipped important hands, grotesque anatomy, plastic skin, excessive smoothing, excessive sharpening, posterization, banding, random modern objects, inconsistent shadows, impossible perspective, or common generative artifacts.

## Generation procedure

For each image:

1. Randomly choose the theme, environment, pose/action, composition, lighting, attire palette, iconography, lion presence, and optional devotee/puja foreground treatment.
2. Compare the proposed combination to the batch history and redraw attributes until it passes the hard anti-duplication rules.
3. Assemble the complete prompt using the quality-first template.
4. Generate exactly one image.
5. Perform full-resolution anatomy, text, artifact, framing, and duplicate QC.
6. If it fails, regenerate that concept; do not save a defective candidate as a new variation.
7. Record all selected attributes in the batch metadata so later generations can avoid them.

## Batch target

For a normal 20-image run, aim for approximately:

- 4–5 direct Durga Mata hero/devotional portraits.
- 4–5 Durga Mata + lion scenes.
- 4–5 puja/aarti/devotee scenes.
- 4–5 Navratri/festival scenes.
- At least 5 wide environmental compositions.
- At least 6 left/right copy-space compositions.
- At least 8 distinct environments.
- At least 8 distinct pose/action choices.
- At least 5 lighting profiles.
- No more than 2 approved images from any single environment.

These are balance targets, not a requirement to force a weak image. Quality and meaningful scene diversity take priority.
