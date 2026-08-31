# Daily Adobe Stock Wan 2.2 Pipeline

This definition is authoritative for every future batch under `output/daily-adobe-stock/YYYY-MM-DD/`.

## Image-to-video prompt contract

Every Wan 2.2 prompt must contain these fields in this order:

1. **Camera behavior:** locked tripod on rigid support; zero pan, tilt, roll, dolly, orbit, crane, zoom, reframing, handheld drift, micro-jitter, shake, parallax shift, or stabilization wobble.
2. **Intended motion:** exactly one visible motion, performed once, at low amplitude. Everything else remains static.
3. **Continuity locks:** lock identity, object count, geometry, materials, texture, background, horizon, lighting, exposure, white balance, focus, and shadows.
4. **Realistic physics:** describe only the physical behavior of the intended motion.
5. **Negative constraints:** prohibit secondary motion, morphing, duplication, temporal warping, texture crawling, unstable edges, flicker, judder, smear, and compression-like blocking.
6. **Temporal plan:** one uninterrupted 6-second shot; hold the complete source image for the first 12 frames, ease the single motion in and out once, then hold a complete stable final image for the last 12 frames.
7. **Frame integrity:** every frame must be fully rendered edge to edge; prohibit black, white, blank, transparent, corrupted, frozen, or dropped-looking frames, as well as fades, cuts, dissolves, flashes, and transitions.
8. **Output safety:** silent visual generation only; no sound or audio track; keep the moving subject safely inside frame boundaries.

Do not request camera movement. If a concept depends on a moving camera, redesign it around one local subject motion instead.

## Mandatory post-generation QC

A prompt cannot prevent encoder or container faults, so no generated video is submission-ready until it passes all checks:

- Decode every frame from start to finish without errors.
- Confirm constant frame rate and consistent frame dimensions.
- Confirm the first and final frames are nonblank, fully rendered picture frames.
- Scan for black, white, near-empty, duplicate-run, frozen, corrupt, or dropped frames.
- Inspect for shake, micro-jitter, rolling horizon, focus breathing, exposure pulses, flicker, texture crawling, warped edges, duplicated objects, and unintended secondary motion.
- Reject clips with fades, flashes, cuts, transitions, abrupt starts, abrupt stops, or subjects crossing frame boundaries.
- Remove the audio stream entirely; do not submit silent audio, malformed audio, or unexpected audio tracks.
- Export a standards-compliant MP4 with H.264 High Profile, yuv420p, constant frame rate, progressive scan, and no audio stream.
- Re-open the final exported MP4, decode every frame again, and repeat the first-frame, last-frame, blank-frame, motion-stability, and duration checks.
- Never upload a clip that fails any check; regenerate from the source image with lower motion amplitude.

## Metadata validation

Each Markdown table must retain exactly these columns:

| ID | Image file | Adobe category | Adobe Stock title | Image-generation prompt | Wan 2.2 image-to-video prompt | Adobe Stock tags, ordered by relevance |
|---:|---|---|---|---|---|---|

There must be exactly one row per image and the prompt must describe the actual corresponding frame.
