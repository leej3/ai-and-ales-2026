# My agent workbench

A five-minute show-and-tell by John Lee for Jamestown Frontier Society's AI & Ales at Billsburg Brewery, Williamsburg, on October 15, 2026.

[Open the presentation](https://leej3.github.io/ai-and-ales-2026/).
[All project links and downloads](https://leej3.github.io/ai-and-ales-2026/links.html).

## Present tonight

Download `index.html` and open it in a browser.
Every slide image is embedded, so presenting requires no internet connection.
Use arrow keys, space, or touch swipes to move between slides.
Press **F** for fullscreen and **N** for speaker notes.
The footer links to these sources and the download page.
External project links require an internet connection.

The eight slides have a five-minute timing plan and a roughly 700-word [speaking script](speaker-notes.md).
The [PowerPoint](downloads/ai-and-ales.pptx) embeds images, links, and speaker notes.
The [PDF](downloads/ai-and-ales.pdf) is a static backup with clickable links.
None of these files has password protection.

## Edit and rebuild

`content.json` is the editorial and layout source.
It contains slide text, image paths, positions, links, speaker notes, and timings.
`assets/` contains the saved visuals.
`scripts/build.mjs` builds the browser deck and can also build a PowerPoint draft.

With Node.js 22 or later, the browser deck requires no packages:

```sh
node scripts/build.mjs --web-only
```

To build the PowerPoint draft, run the same script without `--web-only` in an environment with OpenAI's `@oai/artifact-tool` package available.
Set `ARTIFACT_MODULE_ROOT` to the package installation's `node_modules` directory when it is outside this checkout.
The draft is written to `.build/draft.pptx`.
Set `RENDER_PPTX=1` to render individual slide previews for visual inspection.
The checked PowerPoint is included in `downloads/` for use without that runtime.

To export the PDF, open `index.html` in Chrome and print to PDF.
The print stylesheet includes all eight slides at 16:9, with no browser controls.
Disable headers and footers and enable background graphics.

## Attribution

OpenAI Codex assisted with source review, drafting, layout, and build checks.
Source links and image credits are in [SOURCES.md](SOURCES.md).
The STAMPED slide connects the Zenodo study record and poster PR to the next research workshop.
Improved performance and transfer remain hypotheses to test.

Original presentation prose and code are copyright 2026 John Lee.
Third-party and institutional material retains its existing rights and notices.
See [NOTICE.md](NOTICE.md).
