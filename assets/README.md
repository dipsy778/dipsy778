# Profile graphics

The profile uses repository-hosted SVG images plus native GitHub Markdown controls.

## Assets

- `profile-window-{dark,light}.svg`: 900 × 320 desktop window headers.
- `profile-window-mobile-{dark,light}.svg`: 440 × 342 mobile window headers.
- `tab-{overview,stack,parallel,docs}-{dark,light}.svg`: navigation link images.
- `parallel-banner.webp`: the original supplied Parallel banner.
- `sql.svg`: generic SQL tile.

The README's `picture` sources select a narrow header under 600 px and the appropriate colour scheme. Keep the website and documentation links underneath the Parallel banner.

## Animation and interaction

The hero uses CSS keyframes for a blinking cursor, a travelling trace and a soft glow. It remains fully readable without animation. Its `prefers-reduced-motion: reduce` rule disables motion.

SVG images embedded by GitHub cannot receive custom hover or pointer interaction. The window chrome and file labels inside the hero are decorative. The four navigation links beneath it jump to actual sections or open the documentation. Native `details/summary` elements provide the open/close interactions.

Keep biography and technology labels in Markdown as well as the graphics. The SVGs contain no JavaScript, external imports or external fonts.

