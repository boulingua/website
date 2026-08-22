# Fonts shipped by this repository

The hub self-hosts three families. All are cut by Google Fonts rather than by
`kit/design/build_fonts.py`, because the hub needs two things the kit's tiers
do not carry: a display face for one heading, and the 300 and 500 weights of
the body face. Self-hosting rather than linking `fonts.googleapis.com` is
deliberate — a webfont request from the reader's browser to a third party is a
data transfer the Datenschutzerklärung would have to declare.

These files are not covered by `kit/design/fonts/ATTRIBUTION.md`, which
documents the kit's own subsets. Gate A4 reads both.

| File | Family | Licence | Upstream |
|---|---|---|---|
| `source-sans-3-v19-latin_latin-ext-300.woff2` | Source Sans 3 | OFL 1.1 | <https://github.com/adobe-fonts/source-sans> |
| `source-sans-3-v19-latin_latin-ext-regular.woff2` | Source Sans 3 | OFL 1.1 | <https://github.com/adobe-fonts/source-sans> |
| `source-sans-3-v19-latin_latin-ext-500.woff2` | Source Sans 3 | OFL 1.1 | <https://github.com/adobe-fonts/source-sans> |
| `source-sans-3-v19-latin_latin-ext-600.woff2` | Source Sans 3 | OFL 1.1 | <https://github.com/adobe-fonts/source-sans> |
| `source-sans-3-v19-latin_latin-ext-700.woff2` | Source Sans 3 | OFL 1.1 | <https://github.com/adobe-fonts/source-sans> |
| `jetbrains-mono-v24-latin_latin-ext-regular.woff2` | JetBrains Mono | OFL 1.1 | <https://github.com/JetBrains/JetBrainsMono> |
| `jetbrains-mono-v24-latin_latin-ext-500.woff2` | JetBrains Mono | OFL 1.1 | <https://github.com/JetBrains/JetBrainsMono> |
| `permanent-marker-v16-latin-regular.woff2` | Permanent Marker | Apache-2.0 | <https://www.fontdiner.com> |

Licence texts: [`kit/design/fonts/LICENSES/`](https://github.com/boulingua/kit/tree/main/design/fonts/LICENSES).
Source Sans 3 and JetBrains Mono are the same OFL families the kit documents;
only the cut differs. Permanent Marker is Apache-2.0 and appears in no kit tier.

Consolidating onto kit cuts would mean adding a display tier and the 300/500
weights. That is font work and it is not scheduled here — this file records
what actually ships in the meantime, which is the thing that was missing.
