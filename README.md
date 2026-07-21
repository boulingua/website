# boulingua website

Landing page and showcase for the **boulingua** multilingual teaching
platform.

Live site: <https://boulingua.github.io/website/>

Boulingua is a free, openly licensed multilingual teaching platform created
by S. Le Boulanger. This repository hosts the public landing page that
introduces the four sister sites:

- **EFL** — English as a Foreign Language (Klassen 5–13)
  — <https://boulingua.github.io/efl/>
- **FLE** — Français Langue Étrangère (Klassen 6–13)
  — <https://boulingua.github.io/fle/>
- **DaF** — Deutsch als Fremdsprache (CEFR A1–C1)
  — <https://boulingua.github.io/daf/>
- **Ressourcen-Hub** — Curated open-licensed teaching resources
  — <https://boulingua.github.io/ressources/>

## Build locally

Requires [Hugo extended](https://gohugo.io/installation/) (≥ 0.147.0) and
Go (for module-based theme imports).

```bash
hugo mod get -u
hugo server
```

Then open <http://localhost:1313/website/>.

## Stack

- [Hugo](https://gohugo.io/) static site generator
- [hugo-coder](https://github.com/luizdepra/hugo-coder) theme (imported as
  a Hugo module)
- Deployed via GitHub Actions to GitHub Pages

## Per-language accent colours

Boulingua is one platform with many languages. Each language project has **its own signature accent colour** and **its own abstract icon**, so it is recognisable on its own while still part of the whole. Every accent is **flag-safe** (the hue does not appear in that language's national flag), mutually distinct (≥20° apart on the hue wheel), kept clear of the boulingua hub blue `#1A73E8`, and contrast-checked for light and dark themes. The shared CEFR ramp (A `#4CAF50`, B `#1A73E8`, C `#8E24AA`) is independent of these.

The single source of truth is [`data/accents.yaml`](data/accents.yaml); the same values drive the sites' CSS and the `slidegen` / `sheetgen` LaTeX templates. See the [Design & colours](https://boulingua.github.io/website/design/) page for a visual overview.

| Code | Language | Icon | Light accent | Dark accent |
|------|----------|------|--------------|-------------|
| `daf` | German | hexagon | `#1D87A7` | `#7ECEE7` |
| `efl` | English | circle | `#248D19` | `#89E77E` |
| `fle` | French | square | `#4B8D19` | `#ACE77E` |
| `afl` | Arabic | pentagon | `#4A23C7` | `#977EE7` |
| `cfl` | Chinese | triangle | `#2334C7` | `#7E89E7` |
| `ele` | Spanish | diamond | `#198D81` | `#7EE7DC` |
| `gfl` | Greek | U-shape | `#C74A23` | `#E7977E` |
| `ils` | Italian | ring | `#8023C7` | `#B97EE7` |
| `jfl` | Japanese | rounded square | `#867B18` | `#E7DC7E` |
| `lle` | Latin | semicircle | `#C72334` | `#E77E89` |
| `nsf` | Norwegian | star | `#6D8618` | `#CEE77E` |
| `nvt` | Dutch | plus | `#198D34` | `#7EE797` |
| `pfl` | Polish | chevron | `#AD701F` | `#E7B97E` |
| `ple` | Portuguese | trapezoid | `#B723C7` | `#DC7EE7` |
| `rki` | Russian | octagon | `#198D5B` | `#7EE7B9` |
| `tfl` | Turkish | arch | `#C7236A` | `#E77EAC` |
| `ufl` | Ukrainian | heptagon | `#C723A1` | `#E77ECE` |

## Licence

Dual-licensed:

- **Code** (Hugo configuration, templates, CSS, workflow YAML) — MIT
  License, see [`LICENSE`](LICENSE).
- **Content** (everything under `content/`) — Creative Commons
  Attribution-ShareAlike 4.0 International, see
  [`LICENSE-content`](LICENSE-content).

## Author

S. Le Boulanger — <https://github.com/boulingua>

## Use of LLM tools

Portions of this project were prepared with assistance from large language model tooling for narrowly defined, non-authorial tasks: copyediting, prose smoothing, Markdown/LaTeX formatting, scaffolding of boilerplate files (CI configs, build scripts), code refactoring. The tools used were Chat AI, the LLM service of KISSKI (GWDG), and a self-hosted Mistral Small (24B, Apache-2.0) run locally via Ollama and the ollamar R package — local inference only, with no data sent to third parties for the self-hosted model.
