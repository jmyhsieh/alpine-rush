# ALPINE RUSH Phase 1 Visual Assets

These project-specific bitmap assets were generated with OpenAI's built-in image generation tool on 2026-08-01. No third-party image files were incorporated.

## `snow-detail.png`

- Runtime role: world-space scalar detail for the terrain snow shader.
- Final format: 256 x 256, 8-bit grayscale PNG, power-of-two and edge blended for repeat wrapping.
- Post-processing: downsampled with Lanczos, normalized around middle gray, contrast reduced, and opposite edge bands blended with a smoothstep curve.
- Prompt: "Square, perfectly top-down seamless freshly groomed alpine snow; subtle wind-packed micro relief and compacted crystalline granules; stylized low-poly PBR-friendly material; near-white with restrained cool-blue recesses; uniform edge-to-edge density; no tracks, footprints, objects, horizon, text, logos, watermark, large dunes, or strong directional lighting."

## `powder-atlas.png`

- Runtime role: 2 x 2 particle sprite atlas for snowboard carve and landing powder.
- Final format: 256 x 256 RGBA PNG; each cell is 128 x 128.
- Post-processing: downsampled with Lanczos; source luminance was converted into the alpha channel over white RGB so normal blending has no black fringe.
- Prompt: "Four isolated snow-powder sprites in an exact 2 x 2 atlas on pure black: compact impact cloud, sideways carve fan, airy trailing wisp, broad landing burst; polished stylized alpine game VFX; white and pale icy blue; smooth fade to black; no overlap, borders, text, landscape, rider, logos, or watermark."

Both files have procedural fallbacks in `index.html`; a missing bitmap must not prevent the game from starting.
