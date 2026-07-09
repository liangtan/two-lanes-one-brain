# Two Lanes, One Brain

A split-brain reflex game: one character in each half of the screen, two lanes per side, and you control both at once. Dodge the squares, catch the orbs — miss either and the run is over. Patterns start mirrored, then the lanes split, then the timing splits.

**Play it:** https://liangtan.github.io/two-lanes-one-brain/

## Controls

| Input | Action |
| --- | --- |
| `F` / `J` | Toggle the left / right character's lane |
| `A` `D` and `←` `→` | Set the left / right lane directly |
| Tap left / right half | Same thing, for touch |
| `M` or tap the speaker | Mute |

## Development

The whole game is a single dependency-free file: `index.html`. Open it directly or serve it statically:

```sh
python3 -m http.server 8642
```

Every tunable (speeds, spawn timing, phase thresholds, colors) is a named constant at the top of the script.

## Deployment

Pushes to `main` deploy to GitHub Pages via `.github/workflows/deploy.yml`.
