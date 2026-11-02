# Ticker Morph

A vanilla HTML/CSS/JS recreation of a stock-ticker "shared element" animation: a compact TSLA row springs open into a detailed card. A cursor scrubs the chart while the price digits roll like an odometer, the change turns red below the previous close, and then everything collapses back into the row.

**Live:** https://hedonistjugend.github.io/ticker-morph/

- Single `index.html`, no build step.
- The whole animation runs on one virtual clock (`t += dt * speed`), so the **1x / 0.25x / 0.1x** buttons slow down every part of it, including the springs and digit rolls.
- URL params: `?speed=0.25` sets the starting speed. `?t=2.6` freezes the animation at a moment in the 4.6 s loop. `?compare` hides the UI and renders at 1:1 scale for side-by-side comparison with the source video.
