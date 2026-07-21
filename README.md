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
