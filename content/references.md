---
title: "References"
date: 2026-05-05
---

Boulingua draws on a small set of public, openly available frameworks
and tools. This page lists those references, acknowledges the
inspiration behind the curricula, and provides a citation entry for
anyone wishing to cite the project.

## Frameworks and standards

- **Common European Framework of Reference for Languages (CEFR / GER).**
  Council of Europe, *Common European Framework of Reference for
  Languages: Learning, teaching, assessment* (2001) and *Companion
  Volume* (2020).
  <https://www.coe.int/en/web/common-european-framework-reference-languages>
- **Bildungsplan Baden-Württemberg** — Gesamtschule curriculum
  reference for the EFL and FLE sister sites.
  <https://www.bildungsplaene-bw.de/>

## Inspiration for examination formats

The DaF examination-format YAMLs are structurally inspired by the
publicly documented model-exam handbooks of the **Goethe-Institut**
("Prüfungsziele, Testbeschreibung" / "Modellsatz Erwachsene"),
**ÖSD**, and **telc**. Boulingua is **not affiliated** with these
institutions, and **no actual stimulus material from any official
model exam is reproduced**; only the structural parameters
(number of parts, item counts, timing, scoring weights, rubric
dimensions) inform the format YAMLs. All stimulus texts on the
sites are original to S. Le Boulanger.

A full bibliography of model-exam handbooks consulted lives on
each respective subsite — see for example
[DaF · Literatur](https://boulingua.github.io/daf/literatur.html).

## Tools and platforms

- **[Quarto](https://quarto.org/)** — used to author the EFL, FLE,
  DaF and Ressourcen-Hub subsites.
- **[Hugo](https://gohugo.io/)** with the
  **[hugo-coder](https://github.com/luizdepra/hugo-coder)** theme
  — used for this landing page.
- **GitHub Pages** + **GitHub Actions** — hosting and CI.

## Open-content acknowledgements

Curated external resources linked from the Ressourcen-Hub come
from public-service and institutional sources only — among
others Deutsche Welle, the British Council, Radio France
Internationale, TV5Monde, and the Goethe-Institut's freely
published practice exercises. No commercial textbook material
is paraphrased or reproduced.

## Licensing

- Website code (Quarto config, Hugo templates, Lua filters,
  Python helpers, SCSS): **MIT**.
- Written content (units, exam exemplars, learning aims):
  **CC-BY-SA 4.0**.

## Citing Boulingua

Machine-readable metadata is provided in each subsite's
`CITATION.cff`. A suggested citation for the project as a whole:

> Le Boulanger, S. (2026). *Boulingua — Multilingual Teaching
> Platform (EFL · FLE · DaF · Ressourcen).* boulingua.
> <https://boulingua.github.io/>

BibTeX:

```bibtex
@misc{leboulanger_boulingua_2026,
  author       = {Le Boulanger, S.},
  title        = {{Boulingua --- Multilingual Teaching Platform
                   (EFL {\textperiodcentered} FLE {\textperiodcentered}
                   DaF {\textperiodcentered} Ressourcen)}},
  year         = {2026},
  howpublished = {boulingua},
  url          = {https://boulingua.github.io/},
  note         = {MIT (code) / CC-BY-SA 4.0 (content)}
}
```

To cite a specific subsite, use its `CITATION.cff`:

- [EFL](https://github.com/boulingua/efl/blob/main/CITATION.cff)
- [FLE](https://github.com/boulingua/fle/blob/main/CITATION.cff)
- [DaF](https://github.com/boulingua/daf/blob/main/CITATION.cff)
- [Ressourcen](https://github.com/boulingua/ressources/blob/main/CITATION.cff)
