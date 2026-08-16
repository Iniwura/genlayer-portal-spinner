# GenLayer Portal Spinner

A lightweight animated loading spinner designed for the GenLayer Portal.

<p align="center">
  <img src="genlayer-validator-pulse-bw.svg" width="96" height="96" alt="GenLayer Portal Spinner" />
</p>

The animation keeps the GenLayer mark recognizable while using a simple three-part pulse to suggest validators progressing toward consensus. It is intentionally minimal so it remains clear in small loading states and frequent Portal interactions.

## Features

- Original GenLayer-focused loading animation
- Smooth infinite loop
- Black on light backgrounds
- White on dark backgrounds
- Readable at small sizes
- Pure SVG and CSS
- No JavaScript or external dependencies
- `prefers-reduced-motion` support

## Files

- `genlayer-validator-pulse-bw.svg` — animated black/white spinner preview
- `spinner.svg` — standalone animated SVG
- `spinner.css` — reusable CSS animation
- `index.html` — light/dark browser preview

## Usage

### Standalone SVG

```html
<img src="spinner.svg" width="32" height="32" alt="Loading" />
```

The standalone SVG automatically renders black in light color schemes and white in dark color schemes.

### Inline SVG + CSS

For full control over the spinner color, use the inline SVG markup from `index.html` together with `spinner.css`. The animation uses `currentColor`, so the spinner inherits the surrounding text color.

```css
.loader {
  color: #000;
}

.dark .loader {
  color: #fff;
}
```

## Motion

The three parts of the GenLayer mark pulse in sequence on a `1.08s` loop. There is no orbit, rotation, glow, or logo morphing. The mark geometry remains unchanged throughout the animation.

## Accessibility

The standalone SVG includes `role="status"` and an accessible loading label. The CSS also respects `prefers-reduced-motion` by slowing the animation.

## License

MIT
