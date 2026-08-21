# DYRN — Portfolio

Personal portfolio for **Dyrn Zefanya** — Jakarta-based IT & digital specialist (WordPress, technical SEO, and self-hosted AI automation). A single-page, five-chapter cinematic site: a live WebGL night-temple scene carries the scroll, with real project work, skills, and contact info layered over it.

![Preview](assets/kage-preview.webp)

## What it does

- About, Selected Work (3 flagship projects + 11 more), Craft & Stack, and Contact, all inside one continuous scroll-driven WebGL scene.
- Real project screenshots (laptop mockups, Discord/Hermes AI agent screenshots, n8n workflow) layered into the cards and project grid.
- Chapter navigation, responsive mobile layout, reduced-motion behavior, and a custom cursor for precise pointer devices — inherited from the base template.

## How it is made

`index.html` contains the document structure, CSS, procedural Three.js scene, scroll choreography, and interaction logic. A vendored Three.js r149 build provides WebGL rendering without a package manager or build step. There is no framework, no build tooling, no analytics.

## Run locally

From the repository root:

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

Then visit [http://127.0.0.1:4173/](http://127.0.0.1:4173/).

## Project structure

```text
├── index.html
├── PROMPT.md                    # original build brief for the WebGL scene
├── assets/                      # portfolio screenshots (projects, AI agent, mockups)
└── secret-pathways-assets/      # fonts, three.min.js, generated plates, foreground cutouts
```

## Credit

This site is built on **[Kage](https://github.com/MengTo/kage)** by Meng To — an interactive five-chapter night walk through a Kyoto mountain temple, rendered live in Three.js. The scene engine, layout system, and motion language are his; the content (copy, project cards, screenshots, contact info) has been replaced with Dyrn Zefanya's own portfolio material. See `PROMPT.md` for the original build brief. The vendored Three.js r149 build retains its own MIT license notice.

The original Kage repository states no license is granted for reuse or redistribution of its code or artwork — this repository is kept **private** for that reason, used as a personal, non-commercial customization rather than a public redistribution.
