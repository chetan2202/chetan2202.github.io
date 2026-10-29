# chetan2202.github.io

Personal landing page for **Chetan Vashistth**, served at
[chetan2202.github.io](https://chetan2202.github.io/).

## What this is

A single static `index.html` — no build step, no framework, no dependencies. All CSS
is inlined in the file. GitHub Pages serves the repository root of the `master` branch
directly (it is a GitHub *user page*, so the repo name must stay `chetan2202.github.io`).

## Structure

```
chetan2202.github.io/
  index.html   the whole page (markup + inlined CSS + a tiny inline script)
  README.md
  CLAUDE.md    working notes for AI agents
```

## Content

- Header: name, title, tagline.
- "What I work on": skill chips.
- "Projects": one card per project, each with a prominent **Download App** button
  and a smaller source-code link.
- "Elsewhere": links to the main site, GitHub, and email.

Profile details are sourced from [chetanvashistth.com](https://chetanvashistth.com)
(the main personal site, hosted separately on its own custom domain).

## Preview locally

Just open `index.html` in a browser, or serve the folder:

```
python -m http.server 8000
# then visit http://localhost:8000
```

## Deploy

Push to `master`. GitHub Pages rebuilds automatically (usually within a minute) and
publishes to https://chetan2202.github.io/. Pages is already enabled (source:
`master` branch, `/` root).

## Related

- [Family Grocery PWA](https://chetan2202.github.io/suno-app/) —
  [source](https://github.com/chetan2202/suno-app). Linked from the Projects section.
- [TennisLive](https://chetan2202.github.io/tennislive-app/) — 3D tennis game PWA.
  Built files only (`chetan2202/tennislive-app`); the source repo is private, so the
  card has no source link.
