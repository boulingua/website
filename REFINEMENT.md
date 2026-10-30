# Refinement record — 30 October 2026

This is a local engineering candidate on `refine/2026-10-30`. No hosted CI,
published release or production deployment of these changes has been observed.
The suite strategy and integration order live in the organisation repository,
`docs/refinement-2026-10-30.md` and `docs/release-candidate-2026-10-30.md`.

## Findings, implementation and verification

The website introduces the suite and links its courses and reading products. Shared assets previously had project-prefix and contrast problems; local styles used stale palette values and undersized text. The site now explicitly loads shared tokens, uses the current semantic colours, and benefits from the repaired navigation, links and landmarks in kit. Local templates are declared in boulingua.yml.

Strict Hugo build and the full local kit gate battery passed, including representative desktop/mobile browser checks, automated WCAG 2.1 AA checks and local-link verification. Browser automation blocks external requests during tests, so it does not count visits or claim third-party service availability.

Use README.md and the kit README for local setup. This is the integration hub, not evidence that all linked language courses are finished. Release depends on the matching shared kit/workflow release and review of the published navigation/status text. No deployment of this candidate has occurred.
