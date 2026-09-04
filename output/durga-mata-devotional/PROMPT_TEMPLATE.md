# OpenAI Prompt Template — Durga Mata Devotional

Use this template to build each image prompt. Replace every bracketed value with concept-specific content; do not leave unresolved placeholders in generation prompts.

## Prompt template

**Purpose:** Create a respectful cinematic devotional still of Durga Mata as a native [ASPECT] source image for a devotional-song video. The frame should remain useful for [VIDEO_USE], with [COPY_SPACE] copy space and comfortable safe margins for later editing.

**Subject:** Durga Mata portrayed with a serene, compassionate, powerful divine presence; refined natural facial detail; rich red sari with elegant gold detailing; ornate traditional crown; luminous controlled halo; traditional jewelry; [ARM_COUNT] intentionally visible and anatomically coherent arms; [LION_DESCRIPTION]. Hand and symbolic-object assignments: [HAND_OBJECT_MAP]. Every hand has a clear readable silhouette and a physically plausible connection to the body.

**Pose:** [POSE_DESCRIPTION]. Body orientation: [ORIENTATION]. Expression: [EXPRESSION]. Keep blessing gestures, symbolic objects, crown, halo, and lion clearly separated and fully readable.

**Environment:** [SCENE_DESCRIPTION]. Build one coherent environment with realistic architecture/nature, layered depth, restrained devotional decoration, and no readable signage or script.

**Composition:** [COMPOSITION_PROFILE], [CAMERA_DISTANCE], native [ASPECT]. Place Durga Mata [SUBJECT_PLACEMENT]. Preserve [COPY_SPACE] clean visual space for lyrics where requested. Keep crown and halo comfortably below the upper frame edge; keep important hands, symbolic objects, lion face/paws, and garment edges safely inside the frame. No accidental cropping of important devotional elements.

**Lighting:** [LIGHTING_PROFILE]. Physically coherent light direction, controlled highlights on gold and jewelry, natural skin rendering, readable eyes and hands, detailed red fabric, balanced halo exposure, stable background illumination, cinematic depth without excessive glow.

**Art direction:** High-detail cinematic photorealistic devotional imagery; dignified Indian sacred visual language; realistic fabric, jewelry, stone, flowers, lamps, mountains, water, or clouds appropriate to the scene; rich but restrained color; natural dimensionality; clean depth separation; no imitation of a specific copyrighted artwork, film depiction, living artist, or identifiable performer.

**Constraints:** No text, letters, pseudo-script, signatures, logos, trademarks, brands, labels, watermarks, collage, grid, contact sheet, split screen, border, duplicated face, unintended extra arms, missing declared arms, fused arms, fused hands, malformed fingers, impossible joints, duplicated symbolic objects, floating weapons, floating jewelry, objects intersecting the face or body, weapon tips touching frame edges, broken lion anatomy, duplicate lion features, deformed paws, cropped crown, cropped halo, clipped important hands, grotesque anatomy, plastic skin, excessive sharpening, posterization, banding, random modern objects, inconsistent shadows, impossible perspective, or common generative artifacts.

## Hand/object-map example

Use a compact explicit map rather than vague phrases such as “holding many weapons.” Example for an eight-arm concept:

- Front right hand: open palm in blessing gesture.
- Front left hand: lotus held away from the torso.
- Upper right 1: trident angled upward with tip safely inside frame.
- Upper right 2: discus held clearly behind and away from the face.
- Upper right 3: sword held outward with visible hilt and blade.
- Upper left 1: conch held clearly in the palm.
- Upper left 2: bow held vertically with clean silhouette.
- Upper left 3: mace held outward and separated from adjacent arms.

The exact selection may change by concept. The number of declared hands must always match the declared arm count.

## 16:9 example skeleton

**Purpose:** Respectful cinematic Durga Mata devotional still, native 16:9 landscape source frame for a devotional song; suitable for a subtle push-in and lyric placement on the left.

**Subject:** Durga Mata with serene protective expression, red sari with refined gold border, ornate crown, controlled luminous halo, traditional jewelry, eight intentionally visible anatomically coherent arms, majestic lion companion standing calmly beside her. [Insert explicit eight-hand map.]

**Pose:** Three-quarter standing blessing pose, shoulders relaxed but powerful, front blessing palm toward the viewer, lion looking calmly toward camera.

**Environment:** Misty Himalayan sanctuary at sunrise, ancient stone steps, distant snow peaks, a few marigold flowers and small oil lamps in the foreground, no signage or readable script.

**Composition:** RIGHT_COPY, medium full-body cinematic view, native 16:9. Durga Mata and lion on the right third, broad atmospheric mountain space on the left for lyrics. All crown, halo, arms, symbolic objects, and lion paws comfortably inside the frame.

**Lighting:** Misty Himalayan dawn with warm sunrise rim light from behind-right and soft cool ambient fill; controlled gold highlights and fully readable face/hands.

**Art direction:** High-detail cinematic photorealistic devotional image, dignified sacred visual language, realistic sari fabric, metal jewelry, stone, flowers, mountain atmosphere, restrained rich color, no copying of a specific artwork or performer.

**Constraints:** Apply the full constraints list from the pipeline.

## Prompt assembly checklist

Before generation, verify:

1. The aspect is explicitly native, not described as a crop.
2. The arm count is explicit.
3. The hand/object map matches the arm count exactly.
4. The pose and environment are specific.
5. Copy-space placement is explicit when needed.
6. Safe margins around crown, halo, hands, objects, and lion are explicit.
7. Lighting direction is coherent.
8. Full negative constraints are present.
9. No artist, celebrity, film, or copyrighted depiction is referenced.
10. The concept key differs materially from previously approved concepts.
