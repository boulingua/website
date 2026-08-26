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

Boulingua is one platform with many languages. Each language project has **its own signature accent colour**, shown as a **pentagon** in that colour, so it is recognisable on its own while still part of the whole. Every accent is **flag-safe** (the hue does not appear in that language's national flag), mutually distinct (≥20° apart on the hue wheel), kept clear of the boulingua hub blue `#1A73E8`, and contrast-checked for light and dark themes. The shared CEFR ramp (A `#4CAF50`, B `#1A73E8`, C `#8E24AA`) is independent of these.

The single source of truth is [`data/accents.yaml`](data/accents.yaml); the same values drive the sites' CSS and the branded LaTeX templates in [`kit`](https://github.com/boulingua/kit) (`latex/`). See the [Design & colours](https://boulingua.github.io/website/design/) page for a visual overview.

<!-- BEGIN generated accent table — design/build_tokens.py. Do not edit. -->
| Code | Language | Light accent | Dark accent |
|------|----------|--------------|-------------|
| `daf` | German | `#0C7F9E` | `#80CDEA` |
| `efl` | English | `#06881B` | `#83E883` |
| `fle` | French | `#5C8000` | `#B8E474` |
| `afl` | Arabic | `#5C16C0` | `#967EE8` |
| `cfl` | Chinese | `#382DC6` | `#7B8AE7` |
| `ele` | Spanish | `#008283` | `#7BE6E6` |
| `gfl` | Greek | `#C74B1F` | `#E7977E` |
| `ils` | Italian | `#871EC1` | `#B97EE7` |
| `jfl` | Japanese | `#8C7208` | `#F3D77B` |
| `lle` | Latin | `#C72238` | `#E87F7E` |
| `nsf` | Norwegian | `#787900` | `#DFE173` |
| `nvt` | Dutch | `#008558` | `#61EAAC` |
| `pfa` | Persian | `#9E6A00` | `#F2C380` |
| `pfl` | Polish | `#AA6322` | `#F0B486` |
| `ple` | Portuguese | `#BA20C2` | `#DF7DE3` |
| `rki` | Russian | `#008471` | `#6AE8CE` |
| `tfl` | Turkish | `#C7236A` | `#EB7D9F` |
| `ufl` | Ukrainian | `#CA209A` | `#ED7CC3` |
<!-- END generated accent table -->

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
