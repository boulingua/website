# Refinement record — 30 October 2026

This is a local engineering candidate on `refine/2026-10-30`. No hosted CI,
published release or production deployment of these changes has been observed.
The suite strategy and integration order live in the organisation repository,
`docs/refinement-2026-10-30.md` and `docs/release-candidate-2026-10-30.md`.

## Findings, implementation and verification

The website introduces the suite and links its courses and reading products. Shared assets previously had project-prefix and contrast problems; local styles used stale palette values and undersized text. The site now explicitly loads shared tokens, uses the current semantic colours, and benefits from the repaired navigation, links and landmarks in kit. Local templates are declared in boulingua.yml.

Strict Hugo build and the full local kit gate battery passed, including representative desktop/mobile browser checks, automated WCAG 2.1 AA checks and local-link verification. Browser automation blocks external requests during tests, so it does not count visits or claim third-party service availability.

Use README.md and the kit README for local setup. This is the integration hub, not evidence that all linked language courses are finished. Release depends on the matching shared kit/workflow release and review of the published navigation/status text. No deployment of this candidate has occurred.


## Analytics notice consistency — 31 October 2026

Plausible remains enabled and now names its self-hosted script URL explicitly. The privacy notice states the actual script URL and site identifier; unsupported assertions about server location, retained data and guaranteed anonymity were removed from the Plausible section.

Privacy pages declare their analytics policy, language and built URL. New kit gate C9 checks actual HTML scripts and visible notices against configuration; it rejects missing, duplicate or mismatched scripts and contradictory notices. Six gate regressions and three scaffold tests passed. Representative strict builds/C9 passed for website, nsf, nvt, gfl, Scriptlibrary and all three resource-hub notice languages; the suite integration run verifies the remaining sites. This is configuration/content evidence, not certification of the remote server or legal compliance.

The Platforms page now describes authored collections and pending educational/curriculum review, with precise collection counts and the separate reading tools. It no longer claims a complete or universally approved curriculum; resource reuse conditions are checked per source.


## Explicit release dependencies — 31 October 2026

The shared workflow caller now names the same immutable org commit in `uses` and
`org_ref`; `release-pins.json` records the actual historical kit/framework pins.
These historical pins are explicitly not the remediated release. The new org
workflow rejects absent/malformed versions, mismatched source commits and schema
bytes, and nonconforming course manifests; hubs pin dependencies without claiming
course conformance. The coordinated updater prepares exact published foundation
sets, updates consumers/checksums together and retains rollback inputs. Separate
read-only candidate CI can validate immutable pre-release commits without release
tags or deployment rights. Hosted execution and new foundation publication remain
unobserved. See the org `docs/release-pins.md`.


## Local verification — 2 November 2026

The strict candidate-kit Hugo build and complete configured gate battery passed
locally. Declined gates, warning ramps and external checks remain listed in the
battery output; this is not hosted CI or deployment evidence. The historical
release pins have not been promoted to new foundation releases.
