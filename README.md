# Felt App Gallery

Interactive apps built from [Felt](https://felt.com) maps using the **building-felt-apps** skill — a few prompts from a styled map to a shareable URL.

**Live gallery:** https://makella.github.io/felt-app-gallery/

## What's here

Each app is a single self-contained HTML file that embeds a Felt map and adds interactive UI on top (stat cards, charts, filters, custom behaviors). Apps live at `apps/<slug>/index.html` and serve at `https://makella.github.io/felt-app-gallery/apps/<slug>/`. The registry `apps.json` drives the gallery index page.

## Publish an app here

After the skill builds an app, ask Claude to **"publish this app to the gallery."** It clones this repo, drops the app at `apps/<slug>/index.html`, appends an entry to `apps.json`, and pushes — live in ~60s.

## Remix an app

Open any card's **remix prompt** and paste it to Claude — it fetches that app, modifies it, and republishes to the same URL.

## Ground rules

- **Public maps only.** Apps embed Felt maps via iframe; a private map shows blank for anyone but its owner. Publish apps whose embedded map is publicly viewable.
- **No confidential data.** This repo and its Pages site are public.
- This is a pilot on a personal account; it may move to a Felt org repo later.
