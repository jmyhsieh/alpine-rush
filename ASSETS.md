# Assets and licenses

## ALPINE RUSH project assets

The following project-specific bitmap assets were generated with OpenAI's
built-in image generation tool on 2026-08-01 and processed locally for this
game. No third-party image files were incorporated:

- `assets/alpine-rush/snow-detail.png`
- `assets/alpine-rush/powder-atlas.png`

Their final prompts, formats, processing notes, and runtime fallback behavior
are documented in [`assets/alpine-rush/README.md`](./assets/alpine-rush/README.md).

## KayKit Forest Nature Pack 1.0 FREE

- Creator: Kay Lousberg
- Source: https://kaylousberg.itch.io/kaykit-forest
- Retrieved: 2026-07-30
- License: Creative Commons Zero 1.0 Universal (CC0 1.0)
- Local license copy: [`assets/kaykit-forest/License.txt`](./assets/kaykit-forest/License.txt)

Included files are an unmodified subset of the free pack:

- `Tree_4_A_Color1.gltf` and `.bin`
- `Tree_4_B_Color1.gltf` and `.bin`
- `Tree_4_C_Color1.gltf` and `.bin`
- `Rock_1_J_Color1.gltf` and `.bin`
- `Bush_2_D_Color1.gltf` and `.bin`
- `forest_texture.png`

At runtime ALPINE RUSH loads this subset from the same GitHub Pages origin, bakes the shared palette texture into vertex colors, and adds a procedural snow mask. If loading fails, the game retains its procedural tree, rock, and bush fallback models.
