# Movements — Pixel Studio

An interactive browser-only image studio built with Material 3 design, rotary knob controls, and vertical stackable effect sliders.

## Controls & Architecture

- **UPLOAD (Top Knob)**:
  - Click to browse and upload any image file.
  - Drag vertically or scroll to cycle through built-in sample presets.
  - Drag and drop image files directly onto the screen box.
- **INTENSITY (Middle Knob)**:
  - An interactive 270-degree rotary potentiometer knob (-135° to +135°).
  - Drag vertically or scroll to modulate the master blending intensity (`0%` to `100%`) across all stacked pixel effects.
- **RESET (Bottom Knob)**:
  - Click or turn to reset all 8 effect sliders back to `0%` and master intensity back to `100%` with a smooth 360° spring return animation.
- **White Screen Box (100% Fill & High-DPI Display)**:
  - Automatically center-crops and fills the display area without borders or distortion.
  - Rendered at 2× Retina resolution with hardware-accelerated typed array pixel manipulation.
  - Hover reveals a save badge; clicking downloads the processed image as a PNG.
- **8 Vertical Stackable Sliders**:
  - Drag any dot upward to increase its effect intensity (from `0%` at the bottom to `100%`).
  - Double-clicking any dot resets that individual slider to `0%`.
  - Arrow keys and PageUp/PageDown provide full keyboard accessibility.
  - Live tooltip badges display the exact percentage during interaction.
  - Effects stack sequentially on the pixel buffer in real time:
    1. **Pixel**: Block aggregation.
    2. **Grain**: Organic procedural film grain.
    3. **Sharp**: 3×3 convolution kernel sharpening.
    4. **Poster**: RGB channel quantization.
    5. **Sepia**: Warm tone color grading.
    6. **Contrast**: Midpoint luminance thresholding.
    7. **Vignette**: Radial luminance falloff.
    8. **Invert**: RGB inversion.
