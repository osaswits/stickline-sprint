# Stickline Sprint

A portrait-first, open-web 2D endless runner built with plain HTML, CSS, Canvas 2D, and JavaScript. No external dependencies, zero build step, and offline-capable in a single `index.html` file.

## Play

Open `index.html` directly in any modern desktop or mobile browser, or serve the folder over HTTP:

```bash
npx serve .
```

### Controls

- **Switch Lanes**: `←` / `→`, `A` / `D`, swipe left/right, or on-screen `◀` / `▶` buttons
- **Jump**: `↑`, `W`, `Space`, swipe up, or on-screen `▲` button
- **Slide**: `↓`, `S`, swipe down, or on-screen `▼` button
- **Pause / Resume**: `P` or `Escape`

## Features

- Fixed `1/120 s` simulation timestep inside a timestamp-driven `requestAnimationFrame` loop for consistent physics across 60 Hz and 120 Hz displays.
- Curated three-lane obstacle patterns (low barriers, overhead signal beams, trains, and token trails) verified for reachability before spawning.
- Seeded PRNG support (`?seed=12345`) for repeatable runs and fairness checks.
- Local best-score persistence via `localStorage` with graceful fallback when storage is unavailable.

## License

Released under the [MIT License](LICENSE).
