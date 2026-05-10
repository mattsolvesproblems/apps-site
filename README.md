# apps-site

Privacy policies and marketing pages for [Praxis](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714) and related apps by Matt Peterson, served via GitHub Pages.

## Structure

Each app gets its own subfolder. Pages live at `<app>/<page>.md` and become `https://mattsolvesproblems.github.io/apps-site/<app>/<page>` once Pages is live.

| App | App Store | Pages hosted here |
|---|---|---|
| **Praxis** | [App Store](https://apps.apple.com/us/app/praxis-practice-is-the-point/id6762659714) | [privacy](https://mattsolvesproblems.github.io/apps-site/praxis/privacy) · [support](https://mattsolvesproblems.github.io/apps-site/praxis/support) · [sources](https://mattsolvesproblems.github.io/apps-site/praxis/sources) |

## Why this is a separate repo

Praxis source lives in a private repo. GitHub Pages on private repos requires a paid GitHub account; this public site repo sidesteps that. The same repo will host privacy policies and marketing pages for future apps (Theoria, Poiesis, etc.) without exposing app source code.

## Editing

Edit the markdown directly. Jekyll defaults handle rendering. Frontmatter (`title:` / `description:`) controls page metadata.
