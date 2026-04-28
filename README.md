# Digital Clock

A stylish, animated digital clock built with plain HTML, CSS, and a small amount of JavaScript. The clock uses segmented-digit visuals (like a seven-segment display but custom) with layered shadows and smooth updates for hours, minutes, and seconds.

![Digital Clock Screenshot](./Screenshot%202024-07-02%20172815.png)

## Demo

Open `index.html` in any modern browser. No build step or server is required — just double-click the file or serve the folder with a static file server.

## Features

- Animated segmented digits for hours, minutes, and seconds
- Layered shadowed duplicates for a neon / glow effect
- Lightweight: pure HTML, CSS, and vanilla JavaScript (no dependencies)
- Responsive sizing using aspect-ratio so digits scale cleanly

## How it works (quick)

- index.html builds the digit elements dynamically using JavaScript and updates them once per second using requestAnimationFrame.
- style.css contains the visuals: colored segments, clip-path shapes for segment geometry, and shadow layers.

## Customize

- Change the background color in `style.css` (body { background: ... }).
- Change the digit color by editing the segment color at `.wrapper main .digits .group .digit span { background-color: #ff0000; }`.
- Adjust digit size by changing the `.wrapper main .digits .group .digit { height: 160px; }` value.

## Browser notes

The script includes a small user-agent check that adds a `safari` class for specific Safari behaviors. The clock works in modern Chromium-based browsers, Firefox, and Safari.

## File structure

- index.html — main HTML and the script that creates and updates the clock
- style.css — all styling and visual effects
- Screenshot 2024-07-02 172815.png — example screenshot shown above

## Contributing

Suggestions, improvements, and bug reports are welcome. Open an issue or submit a pull request.

## License

This repository does not include a license file. If you want others to use or contribute under a specific license, please add a LICENSE file (e.g. MIT) or specify your preferred license here.
