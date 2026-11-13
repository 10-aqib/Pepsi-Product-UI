# Pepsi Product UI

An interactive, full-viewport 3D hero landing page for a fictional zero-sugar soda brand ("Diet Soda – Pure Zero Refreshment"). Built as a single self-contained `index.html` with no build step.

## Features

- **3D soda can** rendered with Google's `<model-viewer>` that tilts toward the cursor in real time.
- **Floating 3D cherries and leaves** with layered parallax and a pointer-repulsion "force field" effect.
- **Rising bubbles** that spawn continuously from the bottom of the screen.
- **Flavor switcher** (Diet Classic / Zero Lime): clicking a card morphs the background gradient, spins the can 720° with motion blur, swaps its base-color texture at the peak, and implodes/explodes the berries, swapping cherry ↔ blueberry models.
- **Glassmorphism** header and flavor cards with a pink `#fbcfe8` accent.
- Display typography in Galada, with Inter and Manrope for body and navigation.

## Tech stack

- HTML, CSS and vanilla JavaScript in one file
- [GSAP](https://gsap.com/) 3.12.2 for the flavor-switch animations
- [`<model-viewer>`](https://modelviewer.dev/) for the 3D can, cherries, blueberries and leaves
- Google Fonts (Galada, Inter, Manrope, Outfit)

Libraries and 3D/image assets are loaded from CDNs and remote storage, so an internet connection is required.

## Getting started

No installation needed.

1. Clone the repository:
   ```bash
   git clone https://github.com/10-aqib/Pepsi-Product-UI.git
   cd Pepsi-Product-UI
   ```
2. Open `index.html` in a modern browser. For best results, serve it locally:
   ```bash
   npx serve .
   ```

## Usage

- Move the mouse to tilt the can and push the floating berries around.
- Click **Diet Classic** or **Zero Lime** in the right-hand carousel to trigger the flavor transition.

## Notes

- The page is a fixed, non-scrolling hero (`overflow: hidden`) designed for desktop viewports; a basic responsive rule applies below 1200px.
- This is a fictional design project and is not affiliated with or endorsed by any real beverage brand.
