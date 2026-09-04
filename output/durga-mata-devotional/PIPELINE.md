# Durga Mata Devotional Image Pipeline

This pipeline is independent from `output/daily-adobe-stock/` and must never modify, overwrite, rename, delete, or depend on files in that existing pipeline. The existing Adobe Stock pipeline may be consulted only as a read-only reference for proven output discipline and QC patterns.

## Purpose

Create respectful, cinematic OpenAI-generated devotional still images centered on Durga Mata for:

- 16:9 devotional-song video source frames.
- Native alternate-aspect devotional artwork when useful.
- Optional Adobe Stock submission after separate review and metadata validation.

The primary output is a visually coherent 16:9 frame designed to remain useful during slow video reframing, zooming, or image-to-video animation.

## Output layout

Each production batch uses its own dated directory:

`output/durga-mata-devotional/YYYY-MM-DD/`

Recommended contents:

- Native 16:9 PNG master for every approved concept.
- Optional native 4:5 or 1:1 versions for selected concepts only.
- `durga-devotional-records.md` containing one record per generated image.

Do not create alternate aspect ratios by merely cropping the same generated image for stock submission. When an alternate aspect is needed, regenerate a composition specifically designed for that aspect.

## Aspect profiles

### VIDEO_16_9 — required master

- Exact 16:9 landscape output.
- Keep crown, halo, hands, weapons, lion, and important architecture safely inside the frame.
- Maintain generous edge safety for later pan, zoom, and lyric overlays.
- Prefer a clear foreground, readable subject silhouette, and layered background depth.
- Include deliberate copy-space variants: left, right, or balanced center.

### PORTRAIT_4_5 — optional native composition

- Regenerate vertically rather than crop the landscape master.
- Favor full-length or three-quarter deity compositions, tall temple architecture, floral arches, and vertical light shafts.

### SQUARE_1_1 — optional native composition

- Regenerate specifically for centered devotional artwork.
- Favor balanced halo, symmetrical flowers, throne, lotus, or close devotional portrait compositions.

## Respectful subject profile

Default visual direction:

- Durga Mata portrayed with dignity, serenity, strength, compassion, and divine presence.
- Classical Indian devotional visual language without copying a specific copyrighted artwork, film depiction, living artist, or identifiable performer.
- Rich red sari with refined gold detailing, ornate crown, luminous halo, traditional jewelry, and a majestic lion companion where appropriate.
- Multiple arms must be intentionally specified and anatomically coherent. The default hero profile uses eight clearly separated arms unless a concept explicitly declares another traditional presentation.
- Each hand must have a clear purpose and readable silhouette. Avoid ambiguous, fused, hidden, duplicated, or inexplicable hands and objects.
- Expressions should remain calm, benevolent, protective, or resolute rather than frightening or grotesque.

The pipeline does not claim one generated depiction to be the only canonical religious representation. Concepts should remain respectful of varied devotional traditions.

## Iconography consistency

For the default eight-arm hero profile, use a controlled set of symbolic objects distributed clearly across the composition. A concept may select from traditional devotional motifs such as trident, lotus, sword, discus, conch, bow, mace, or a blessing/open-palm gesture.

Rules:

1. Declare the intended arm count in the prompt.
2. Declare each visible hand's role or object before generation.
3. Keep weapon/object silhouettes separated from the face, crown, other hands, and frame edges.
4. Reject any output with an incorrect arm count, merged limbs, duplicated objects, impossible joints, malformed fingers, or objects emerging from the body.
5. Prefer fewer, cleaner visible symbolic objects over visually crowded arrangements.

## Concept dimensions

Every concept is defined independently across these dimensions:

- `scene_family`
- `pose_family`
- `composition_profile`
- `lighting_profile`
- `aspect_profile`
- `iconography_profile`
- `copy_space_profile`

Create a unique `concept_key` from those dimensions. Do not submit near-duplicate generations that differ only by a tiny pose, crop, or color change.

## Scene families

Use broad environmental diversity so batches feel like a devotional visual journey rather than repeated portraits:

1. Himalayan dawn sanctuary.
2. Ancient temple sanctum with diyas.
3. Grand temple courtyard at sunrise.
4. Lotus lake in soft golden light.
5. River ghat with floating lamps.
6. Sacred forest shrine.
7. Celestial cloud realm.
8. Moonlit temple courtyard.
9. Floral Navratri-inspired mandap.
10. Palace-like divine throne hall.
11. Mountain meadow with lion companion.
12. Monsoon temple steps with distant rain.
13. Deserted stone temple at blue hour.
14. Marigold and diya devotional alcove.
15. Radiant cosmic backdrop with restrained sacred geometry and no readable text.

## Pose families

Use poses that read clearly at video scale:

1. Standing frontal blessing pose.
2. Three-quarter standing blessing pose.
3. Seated on an ornate throne.
4. Seated on a lotus.
5. Riding or calmly accompanied by a lion.
6. Walking through a temple courtyard.
7. Protective warrior stance.
8. Serene contemplative side profile.
9. Compassionate maternal expression with open blessing hand.
10. Symmetrical centered divine portrait.
11. Full-body wide environmental pose.
12. Low-angle heroic yet devotional pose.

## Composition profiles

- `CENTER_HERO`: centered deity, strong symmetry, suitable for chorus or key refrain.
- `RIGHT_COPY`: subject on right third, open left side for lyrics.
- `LEFT_COPY`: subject on left third, open right side for lyrics.
- `WIDE_ENV`: deity smaller within a cinematic environment, useful for intro/interlude.
- `LOW_HERO`: slightly low camera angle, full crown/halo safely framed.
- `THREE_QUARTER`: natural dimensional view with layered background.
- `CLOSE_DEVOTIONAL`: face and upper body, serene expression, carefully managed visible arms/hands.

## Lighting profiles

- Golden sunrise.
- Warm diya illumination.
- Soft temple-window shafts.
- Cool moonlight with warm lamp accents.
- Misty Himalayan dawn.
- Gentle overcast monsoon light.
- Celestial soft radiance.
- Sunset rim light.

Lighting must preserve facial detail, jewelry detail, hand readability, and stable color separation. Avoid blown halos, crushed shadows, excessive neon saturation, or synthetic plastic skin.

## OpenAI image prompt contract

Every image-generation prompt must contain these sections in this order:

1. **Purpose:** devotional-song source frame and intended aspect/use.
2. **Subject:** Durga Mata appearance, expression, arm count, clothing, crown, halo, lion presence, and selected symbols.
3. **Pose:** body orientation, blessing/hand roles, and lion relationship.
4. **Environment:** one specific scene family with coherent physical details.
5. **Composition:** aspect profile, camera distance, subject placement, safe margins, and copy space.
6. **Lighting:** one lighting profile with physically coherent direction and exposure.
7. **Art direction:** photorealistic/cinematic devotional finish, realistic materials, consistent skin/jewelry/fabric rendering, controlled depth.
8. **Constraints:** no text, pseudo-text, logos, watermarks, modern branding, collage, split screen, duplicate faces, unintended extra arms, missing arms, fused hands, malformed fingers, duplicated weapons, floating jewelry, intersecting objects, broken lion anatomy, cropped crown, cropped halo, accidental frame-edge cuts, grotesque anatomy, or common generative artifacts.

## Video-safe framing rules

Every 16:9 master must be designed as a source frame, not merely as a poster:

- Keep at least a comfortable visual margin around crown and halo.
- Keep all critical hand gestures and symbolic objects inside the safe area.
- Avoid weapon tips touching the frame boundary.
- Keep lion face and paws fully readable when the lion is important to the concept.
- Provide environmental depth that tolerates a subtle push-in.
- At least one third of concepts in a batch should provide useful lyric copy space.
- At least one quarter should be wide environmental establishing images.
- Avoid filling every frame with a centered close portrait.

## Variation and duplicate control

For each generation batch:

- Vary the environment before varying minor ornament details.
- Vary pose and subject placement before color grading.
- Vary camera distance across close, medium, full-body, and wide environmental views.
- Use a different concept key for each final image.
- Generate multiple candidates internally if needed, but retain only the strongest approved candidate for a concept.
- Never treat a simple crop, horizontal flip, tiny facial-expression change, or slight hue shift as a new concept.

## Mandatory image QC

Reject an image if any of the following is present:

- Incorrect declared arm count.
- Fused, duplicated, hidden-without-logic, or anatomically impossible arms/hands.
- Malformed fingers or blessing gesture.
- Duplicate, melted, floating, or intersecting symbolic objects.
- Crown, halo, face, important hands, weapon tips, or lion unintentionally clipped.
- Broken lion face, paws, legs, tail, or body anatomy.
- Asymmetrical eyes or facial artifacts that distract at 100% view.
- Pseudo-text, random script, logos, signatures, labels, or watermarks.
- Unintended modern objects or branded products.
- Inconsistent reflections, shadows, scale, perspective, or architecture.
- Plastic skin, excessive sharpening, posterization, banding, obvious AI texture, or compression defects.
- Composition too cramped for 16:9 video use.
- Near duplication of another approved concept.

QC must be performed at full resolution, not only from thumbnails.

## Batch balance

A normal 30-concept batch should target approximately:

- 30 native 16:9 masters.
- 8–10 wide environmental scenes.
- 8–10 medium/full-body devotional scenes.
- 6–8 closer devotional portraits.
- 8–12 frames with deliberate left or right copy space.
- A mixture of temple, nature, mountain, water, celestial, festival, and night environments.
- Selected native 4:5 or 1:1 regenerations only when there is a real downstream need.

## Metadata record

Use one row per generated file:

| ID | Concept key | Image file | Aspect | Scene family | Pose family | Devotional title | Image-generation prompt | Video use note | Tags | QC |
|---:|---|---|---|---|---|---|---|---|---|---|

`Video use note` should identify a useful edit treatment such as subtle push-in, slow horizontal pan through copy space, lyric placement area, intro establishing frame, chorus hero frame, or interlude frame. It is an editing note only and does not require camera motion during image generation.

## File naming

Use stable descriptive names:

`NN-scene-pose-composition-aspect.png`

Examples:

- `01-himalayan-dawn-standing-right-copy-16x9.png`
- `02-temple-sanctum-throne-center-16x9.png`
- `03-lotus-lake-seated-wide-16x9.png`

Avoid names based only on timestamps or random IDs.

## Separation guarantee

The following existing path is out of scope for writes by this pipeline:

`output/daily-adobe-stock/`

Do not alter its `PIPELINE.md`, dated batches, records, images, branch workflow, or metadata schema. This Durga Mata pipeline owns only:

`output/durga-mata-devotional/`
