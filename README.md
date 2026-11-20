# Fabric Store · Textile Showroom

A static textile storefront built around product photography, a catalogue grid and a loyalty mailing-list layout.

[Open the live demo](https://oniseg.github.io/FabricStore/) · [View screenshot](https://raw.githubusercontent.com/onisEg/resume/23df91e50f87b60e1360d79edcc24cf77eb09b07/public/projects/fabric-store.webp)

## How the showroom is assembled

1. The opening banner leads into a textile collection. Each product tile contains an image, category, title, displayed price and a Buy Now control.
2. Choices, loyalty, features, customer reviews and the social-photo section provide the rest of the page. Product information and prices are authored in the markup.
3. Styling comes from a single CSS file with a breakpoint at 767px. The repository presents a storefront design; purchase and subscription controls have no application backend here.

## Run locally

From the repository root, serve the checked-in files with Python 3:

```sh
python -m http.server 8000
```

Open [localhost:8000](http://localhost:8000/) to load `index.html`. The browser reads the HTML, styles and assets directly. On Windows, `py -m http.server 8000` starts the same server.

## Source guide

| File or directory | What to look for |
| --- | --- |
| [index.html](index.html) | Page sections and individual textile cards. |
| [style.css](style.css) | Product-tile styling, overlays and responsive rules. |
| [imgs](imgs) | Product photography and promotional images. |

## Manual walkthrough

Edit the title, price and image of one textile card, reload and compare with adjacent cards. Test either side of the 767px breakpoint to see how image size, spacing and the product controls behave.
