# Thrad email signature images

Public image assets for the Thrad email signature. One flattened card per team
member: the desert, the logo, "Paid Ads in AI", and that person's name, title,
mobile, website and call to book are all baked into a single picture.

Nothing here is live text, which is the point. Pixels cannot be recoloured by a
client's dark mode, re-fonted when Arial is missing, auto-linked into blue, or
pulled apart when a message pane changes width.

## The files

| File | Person |
| --- | --- |
| `thrad-sig-andrea.jpg` | Andrea Tortella, Co-founder / CEO |
| `thrad-sig-marco.jpg` | Marco Visentin, Co-founder / CTO |
| `thrad-sig-giorgio.jpg` | Giorgio Toledo, Chief Operating Officer |
| `thrad-sig-roger.jpg` | Roger Dunn, Chief Commercial Officer |
| `thrad-sig-alex.jpg` | Alexandra Naomi Perez, Chief of Staff |
| `thrad-sig-amara.jpg` | Amara Parker, Head of Client Relations |
| `thrad-sig-abhinav.jpg` | Abhinav Khushalani, Founding Engineer |
| `thrad-sig-gabriel.jpg` | Gabriel Chawla, AI Operations Engineer |

Each is 880 x 316 pixels, a 440 x 158 design rendered at 2x for retina screens,
JPEG quality 0.50, about 39 KB.

## Serving

Published with GitHub Pages from the repository root:

    https://gabrielchaw.github.io/thrad-signatures/thrad-sig-<first-name>.jpg

Those URLs are what the signature markup points at. Do not rename, move or
recompress these files: every installed signature would break.

## Regenerating

The source, the renderer and the tests live outside this repository, in
`~/Projects/thrad-signatures`. Editing the roster and running `npm run cards`
rewrites every card from one renderer at one locked geometry, so the eight can
never drift apart.
