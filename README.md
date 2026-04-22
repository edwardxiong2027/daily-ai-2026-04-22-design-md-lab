# Design MD Lab

Design MD Lab is a tiny browser-native playground inspired by Google's newly open-sourced DESIGN.md concept in Stitch.

Live app: pending deployment

## What it does

- Edit a simple DESIGN.md-style spec in the browser
- Lint the spec for missing sections and weak agent handoff quality
- Preview a product surface from tokens + intent
- Run WCAG-style contrast checks on key token pairs
- Export a `DESIGN.md` file for use with design and coding agents

## Why this is timely

This project is built around a genuinely fresh signal rather than an old generic AI demo:

1. Google said Stitch's `DESIGN.md` draft specification is now open source so AI systems can understand design intent and validate choices against accessibility rules.
2. Google also launched Deep Research Max and framed autonomous research agents as a major next-generation workflow category.
3. Brex launched CrabTrap, an LLM-as-a-judge proxy for securing agents in production, which reinforces the broader shift toward agent infrastructure and structured control surfaces.

Together these point to a near-term opportunity: model-readable design artifacts that are understandable by both humans and autonomous systems.

## Sources

- Google Stitch / DESIGN.md: https://blog.google/innovation-and-ai/models-and-research/google-labs/stitch-design-md/
- Google Deep Research Max: https://blog.google/innovation-and-ai/models-and-research/gemini-models/next-generation-gemini-deep-research/
- Brex CrabTrap: https://www.brex.com/crabtrap

## Local use

Open `index.html` in a browser, or serve locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Files

- `index.html` — full app, styles, templates, parser, linter, preview, export
- `README.md` — project context and sources
- `LICENSE` — MIT

## Notes

This is not an official validator for Google's evolving draft spec. It is a practical, static playground inspired by the concept and optimized for one-run shipping.
