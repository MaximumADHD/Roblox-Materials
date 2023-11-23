# Roblox Materials

This repository is a snapshot of all Roblox's PBR Material TexturePacks as of 11/23/2023.<br/>
It contains the source textures (\*.png) and the GPU compressed textures (\*.ktx)

<hr>

# Image Descriptions

|  **Image Name**           | **Description**                                                                                                                   |
|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------|
| `color.png`               | `ColorMap` of the material.                                                                                                       |
| `normal.png`              | `NormalMap` of the material.                                                                                                       |
| `metalness.png`           | `MetalnessMap` of the material.                                                                                                    |
| `roughness.png`           | `RoughnessMap` of the material.                                                                                                    |
| `height.png`              | A height map used to cross-blend materials in `Terrain`.                                                                             |
| `tintmask.png`            | Defines a mix ratio between the original color and RGB tinted color of each pixel. <br/> (i.e. `BasePart.Color`, `Terrain.MaterialColors`) |
| `optimized/color_dxt.ktx` | DXT compressed combination of `color.png (RGB)` and `tintmask.png (Alpha)`                                                        |
| `optimized/norm_dxt.ktx`  | DXT compressed version of `normalmap.png (GA)`, with the X/Y value<br/> of each pixel stored in the Green/Alpha channels respectively. |
| `optimized/spec_dxt.ktx`  | DTX compressed combination of `metalness.png (Red)`,<br/>`roughness.png (Green)` and `height.png (Alpha)` (if terrain).                            |