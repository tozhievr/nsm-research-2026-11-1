# Neural Stack Machine — Research (2026)

Research on a differentiable stack machine for evaluating prefix Boolean expressions. The repository documents the model, the experimental protocol, measured outcomes, and limitations.

**Research website:** https://tozhievr.github.io/nsm-research-2026-11-1/

## Experimental snapshot

- PyTorch neural stack controller with PUSH, UNARY, BINARY actions.
- 12,532 trainable parameters; hidden width 32; trained checkpoint evaluated at different stack capacities.
- On 24 targeted expressions: capacity 64 — 14/24 correct; 65 — 23/24; 66 — 24/24; 80 — 24/24. This is a targeted test set, not a generalization benchmark.
- Local cell interventions and finite-difference sensitivity measurements are exploratory, not proofs of stability.

## Reproducibility

The experiment scripts, checkpoint, and raw JSON data are available in the companion research archive. The site clearly distinguishes measured results from interpretations.

## Paper

Russian-language manuscript prepared for *Information and Mathematical Technologies in Science and Management*. Author: Roman Shamsiddinovich Tozhiev (Kamchatka State Technical University).

## GitHub Pages

Configure **Settings → Pages → Deploy from a branch → main → /docs**.

## License

No license is granted until one is explicitly selected by the author.
