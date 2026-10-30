# Movements

A browser-only image movement studio built with Material 3 design and motion principles.

## Try it

Open `index.html` in a browser. The initial dialog allows you to start right away with the included sample image, or you can select **Upload** to load your own image or drag and drop an image file directly onto the canvas. Adjust the slider to tune the movement intensity, and click the image to play or pause the motion. All image processing stays local to your browser.

## Material 3 Design and Motion

The interface strictly follows Google's Material 3 design system:

- **Button Shape Morph**: Buttons feature a resting shape morphing to an 8px radius on press (`:active`) using the fast spatial spring easing token.
- **Interaction States**: All interactive elements implement official Material 3 state layers (hover 8%, focus 10%, pressed 12%) and ink ripple animations.
- **Expressive Slider**: Features a 16px track height, 4px vertical pill handle with 6px track gap separation, stop indicators, and active drag expansion.
- **Dialogs**: 28px corner radius, elevation level 3 shadow, M3 typography, and emphasized entrance/exit scale-and-fade animations.
- **Color Roles**: Based on the Material 3 Baseline purple palette (`--md-sys-color-primary`, `secondary-container`, `surface`, `surface-container-high`).
- **Motion Easing**: Driven by Material 3 emphasized decel/accel curves and smooth drifting spring animations with reduced-motion support.

### References

- [Buttons and shape morph](https://m3.material.io/components/buttons/specs)
- [Interaction states](https://m3.material.io/foundations/interaction/states/overview)
- [Motion](https://m3.material.io/styles/motion/overview/how-it-works)
- [Easing and duration tokens](https://m3.material.io/styles/motion/easing-and-duration/tokens-specs)
- [Dialogs](https://m3.material.io/components/dialogs/overview)
- [Sliders](https://m3.material.io/components/sliders/overview)
- [Color system](https://m3.material.io/styles/color/system/overview)
- [Typography](https://m3.material.io/styles/typography/overview)
- [Elevation](https://m3.material.io/styles/elevation/overview)
