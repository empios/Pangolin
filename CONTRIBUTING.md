# Contributing

Pangolin is currently an independent design-system study and static showcase. Treat it as exploratory UI work, not a stable production framework.

## Scope

Good contributions:

- Fix broken responsive behavior.
- Improve accessibility, focus states, contrast, and keyboard behavior.
- Add focused demo examples that use the existing token/component style.
- Clarify documentation, credits, and usage notes.

Avoid:

- Renaming the project around Ubuntu, Canonical, IBM, or Carbon.
- Adding official Ubuntu, Canonical, IBM, or Carbon logos/assets unless their usage is clearly licensed and documented.
- Bundling font binaries unless the corresponding font licence and notices are restored.
- Large visual rewrites that move away from Pangolin's independent identity.

## Local workflow

This is a static HTML/CSS project. Open `index.html` directly in a browser, then check the demo pages in `demos/`.

Before publishing a change, verify:

- `index.html` at desktop and mobile widths.
- `demos/dashboard.html` at desktop and mobile widths.
- `demos/desktop.html` at desktop and mobile widths.
- `demos/mobile.html` at desktop and mobile widths.

## Legal and attribution

Keep `README.md` and `THIRD_PARTY_NOTICES.md` aligned with any new third-party dependency, font, visual asset, or borrowed design convention. References to Ubuntu, Canonical, IBM, and Carbon should remain descriptive and should not imply affiliation, sponsorship, or endorsement.
