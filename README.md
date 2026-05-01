# apps-site

Privacy policies and marketing pages for [Praxis](https://apps.apple.com/) and related apps by Matt Peterson, served via GitHub Pages.

## Structure

Each app gets its own subfolder. Privacy policy lives at `<app>/privacy.md`, which becomes `https://mattsolvesproblems.github.io/apps-site/<app>/privacy` once Pages is live.

| App     | Privacy policy                                                                |
|---------|-------------------------------------------------------------------------------|
| Praxis  | [praxis/privacy](https://mattsolvesproblems.github.io/apps-site/praxis/privacy) |

## Why this is a separate repo

Praxis source lives in a private repo. GitHub Pages on private repos requires a paid GitHub account; this public site repo sidesteps that. The same repo will host privacy policies and marketing pages for future apps (Theoria, Poiesis, etc.) without exposing app source code.

## Editing

Edit the markdown directly. Jekyll defaults handle rendering. Frontmatter (`title:` / `description:`) controls page metadata.
