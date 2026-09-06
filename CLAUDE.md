# CLAUDE.md

Working notes for an AI agent operating in this repository. Read `README.md` first.

## What this repo is

The personal landing page for Chetan Vashistth, served as a GitHub **user page** at
https://chetan2202.github.io/. It is a single static `index.html` with all CSS inlined
and one tiny inline script (the footer year). No build step, no framework, no npm, no
dependencies.

## Hard constraints

- **Repo name is load-bearing.** A GitHub user page is served only from a repo named
  exactly `chetan2202.github.io` on the `chetan2202` account, from the root of the
  default branch (`master`). Do not rename the repo or move `index.html` into a
  subfolder.
- **Keep it a single self-contained file.** No bundler, no external CSS/JS, no package
  manager. If a change needs styling, edit the inlined `<style>` block in `index.html`.
  Only introduce a build step or dependencies if the owner explicitly asks.
- **Static only.** GitHub Pages serves files; there is no backend, no server code, no
  secrets. Never add analytics, trackers, or third-party scripts without being asked.

## Conventions

- No emoji in code, comments, or commit messages.
- Theme-aware: the page defines a light palette on `:root` and a dark override under
  `@media (prefers-color-scheme: dark)`. Keep both in sync when changing colors.
- Responsive and mobile-first; content is capped at `max-width: 760px`.
- Brand color is `--brand: #1f7a53` (green), hover `--brand-2: #2a9d6f`.
- Projects section: one card per project, each with a prominent **Download App**
  button (for non-technical visitors) plus a smaller source-code link. Keep that
  pattern if adding projects.

## Profile source of truth

Bio, title, skills, and contact details come from https://chetanvashistth.com (a
separate site on its own custom domain). If profile facts change, update them there
first; this page mirrors them.

## Deploy

Push to `master`; GitHub Pages rebuilds automatically. Pages is enabled with source
`master` / root. There is no CI to run and nothing to build.

## Attribution for commits

End git commit messages with:

```
Co-Authored-By: Claude Opus 4.8 <noreply@anthropic.com>
```
