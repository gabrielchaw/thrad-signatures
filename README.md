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
| `thrad-sig-danny.jpg` | Danny Wang, Founding Designer |

Each is 1520 x 544 pixels: a 380 x 136 design set in Inter, the wordmark's own
typeface, exported at 4x from Paper (file "Thrad Email Signatures"), JPEG quality
80, about 130 KB. The signature displays at up to 380 CSS pixels, the design size,
so the contact lines sit at 12.5px next to 14px email text, and the image carries
4 device pixels per CSS pixel: sharp on retina laptops, 4K monitors, TVs, and
under browser zoom. Keep the 380 x 136 shape: a new export can then replace a
file in place without anyone reinstalling.

## Serving

Published with GitHub Pages from the repository root:

    https://gabrielchaw.github.io/thrad-signatures/thrad-sig-<first-name>.jpg

Those URLs are what the signature markup points at. Do not rename, move or
recompress these files: every installed signature would break.

## Regenerating

The design lives in Paper, one artboard per person duplicated from the master.
Change the text, export at 4x as PNG, then run `test/paper_cards.py` in
`~/Projects/thrad-signatures`: it fails unless the logo, tagline and painting are
pixel-identical to the reference card and the contact block keeps its clearance.
