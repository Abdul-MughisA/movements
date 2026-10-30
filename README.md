# Movements — Pixel Studio

An interactive browser-only image studio that allows pixel-level image adjustments and stacking, built to match the custom hardware-inspired interface.

## Interface & Controls

- **UPLOAD (Top-Left Circle)**: Open the file picker to upload any image file. You can also drag and drop images directly onto the white box.
- **INTENSITY (Middle-Left Circle)**: Adjusts the master intensity mix across all stacked effects (cycles 100% → 75% → 50% → 25% → 0%).
- **RESET (Bottom-Left Circle)**: Smoothly animates all active effect slider dots back to 0% with spring physics.
- **The White Display Box**: Renders the image on an HTML5 `<canvas>` with real-time TypedArray pixel manipulation. Clicking on the white box downloads the processed PNG.
- **Vertical Stackable Sliders (The 8 Dots)**:
  - Dragging any dot upward increases the strength of that effect (from 0% at rest up to 100%).
  - The effects stack sequentially on the pixel buffer in real time:
    1. **Pixelate**: Block-level pixel aggregation.
    2. **Film Grain**: Organic procedural grain/noise.
    3. **Sharpen**: 3x3 convolution edge enhancement.
    4. **Posterize**: Quantized color channel stepping.
    5. **Sepia**: Warm tone matrix transformation.
    6. **Contrast**: Luminance threshold expansion.
    7. **Vignette**: Radial luminance falloff.
    8. **Invert**: Pixel color inversion.
