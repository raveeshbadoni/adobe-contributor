# Durga Mata Batch Execution Rules

These rules harden the devotional image pipeline against the failed contact-sheet/collage workflow.

## Non-negotiable generation contract

1. One OpenAI image-generation call produces exactly one final asset.
2. Never request a contact sheet, grid, collage, storyboard, montage, multi-panel layout, or composite image.
3. Every concept is generated independently from its own scene prompt.
4. Each generated image is saved as its own file using the pipeline naming convention.
5. Required production aspect is native 16:9 landscape.
6. No captions, filenames, borders, labels, watermarks, banners, readable text, pseudo-text, or UI elements may appear inside the artwork.
7. Do not create individual assets by cropping cells out of a collage or contact sheet.

## File-integrity gate before GitHub upload

Every image must pass all of these checks before it may be committed:

- File decodes successfully from start to finish.
- Actual format matches extension.
- Width and height are readable and non-zero.
- Image is 16:9 within normal pixel rounding tolerance.
- Image is RGB or safely convertible to RGB.
- Re-open the final encoded JPG/PNG after writing it; decoding must succeed again.
- Reject zero-byte, truncated, malformed, or partially decoded files.
- Record filename, dimensions, encoded byte size, and SHA-256 in `MANIFEST.md`.

## GitHub transfer contract

- Binary images must be uploaded as binary blobs using base64 encoding, never as UTF-8 text.
- Upload in small groups when needed, but all files in a batch must ultimately live on one batch branch.
- After updating the branch, fetch/compare the branch against `main` and verify the expected file count before opening the PR.
- Do not open the PR until every expected image and its manifest/records are present.

## Batch acceptance

A 20-image run is successful only when:

- Exactly 20 independent image files exist.
- Every file passes the integrity gate.
- All 20 are present in the GitHub branch.
- `MANIFEST.md` lists all 20 and their verification data.
- The PR is open and references the exact batch directory.

The existing `output/daily-adobe-stock/` pipeline remains read-only and out of scope.
