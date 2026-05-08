# Affiliation badges — TODO list for Harsh

These are the institution logos used in two places:
1. The **Vitae** section on the about page (each entry's badge)
2. The **affiliations strip** at the bottom of the about page

Files referenced from `_includes/affiliations.liquid` and `_timeline/*.md`
(`badge_image:` field).

## Current files

| File         | Format | Source                                                                                          | Status            |
| ------------ | ------ | ----------------------------------------------------------------------------------------------- | ----------------- |
| `ethz.svg`   | SVG    | [Wikimedia](https://commons.wikimedia.org/wiki/File:ETH_Z%C3%BCrich_Logo_black.svg)             | ✅ proper vector  |
| `samsung.svg`| SVG    | [Wikimedia](https://commons.wikimedia.org/wiki/File:Samsung_Black_icon.svg)                     | ✅ proper vector  |
| `safari.jpg` | JPEG   | [safari.ethz.ch](https://safari.ethz.ch/wp-content/uploads/2020/02/SAFARI_logo_github_square.jpg) | 🟡 raster — needs SVG |
| `rvce.png`   | PNG    | [Wikimedia](https://commons.wikimedia.org/wiki/File:New_RV_College_logo.png)                    | 🟡 raster — needs SVG |

The two raster ones use CSS `mix-blend-mode: multiply` to hide their white
backgrounds against the cream page. They look fine, but they pixelate when
scaled up (e.g. on retina screens) and aren't truly resolution-independent.

## TODO — get proper SVG versions of SAFARI & RVCE

### SAFARI

- Ask Onur or someone in the SAFARI infrastructure team if a vector
  version of the logo is available — research groups often have one in
  their press / brand assets.
- Failing that, ask a designer (or use Adobe Illustrator / Inkscape /
  Affinity) to manually trace the high-res raster
  (`SAFARI_logo_github_square.jpg` is 908×907px, plenty to trace cleanly)
  and produce a multi-color SVG that preserves the original colors.
- Drop the resulting file in this directory as `safari.svg`.

### RVCE

- The RVCE logo on Wikipedia (`New_RV_College_logo.png`) is only 120×120
  and has multiple colors (red, gold, blue, white).
- Best path: ask RVCE alumni/communications for the original vector file,
  OR commission a hand-traced SVG.
- A free auto-trace site (e.g. https://vectormagic.com or Inkscape's
  built-in trace bitmap) on a higher-resolution version of the seal
  should give a usable result.
- Drop the resulting file in this directory as `rvce.svg`.

## How to swap in the new SVGs

Once you have `safari.svg` and `rvce.svg` ready:

```bash
# 1. Drop them into this directory
cp safari.svg assets/img/badges/
cp rvce.svg   assets/img/badges/

# 2. Update the references (one sed each)
sed -i 's/safari\.jpg/safari.svg/' \
    _includes/affiliations.liquid \
    _timeline/*.md
sed -i 's/rvce\.png/rvce.svg/' \
    _includes/affiliations.liquid \
    _timeline/*.md

# 3. Optional cleanup -- you can also delete the rasters:
#    rm assets/img/badges/safari.jpg assets/img/badges/rvce.png
```

## Reverted attempt: monochrome auto-trace

Earlier I generated `safari.svg` and `rvce.svg` automatically using
`potracer` (Python potrace) but they came out monochrome (single dark
color, no brand identity). Reverted at user's request -- the rasters
are still cleaner-looking until proper full-color vectors arrive.
