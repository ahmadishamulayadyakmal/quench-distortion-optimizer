# Quench distortion and cracking of large forgings (C10)

## Industrial problem

Water quenching of large forged blocks and high-alloy tool steel creates thermal gradients, residual stress, distortion and cracks; a wrong quench schedule scraps an expensive part.

**Why it happens.** Coupled thermal – phase transformation – stress behaviour, plus damage accumulation where triaxiality and strain concentrate.

## Data (no plant data)

Mixed: JMAK / Koistinen–Marburger kinetics are analytical (A, R26); published FEM distortion and crack-location benchmarks are digitised (B, Y2R07/Y2R08); literature property ranges with uncertainty; open surrogate geometry. No plant data is held.

> Only open datasets and published literature are used. No plant or proprietary data are held here; plant numbers quoted from papers are external literature, not independently reproduced results.

## Tool chain

Simplified FEM thermal–phase–stress coupling, Oyane damage criterion, JMAK / Koistinen–Marburger kinetics, mesh convergence, surrogate for quench-medium choice, Pareto study (distortion vs hardness), SHAP-style sensitivity.

## Journal references

- **R26** — JMAK and martensite-fraction kinetics (compound: 2 papers).
- **Y2R07** ([DOI](https://doi.org/10.1016/j.jmapro.2020.08.042)) — quench-distortion FEM and the external 0.5 mm plant result.
- **Y2R08** ([DOI](https://doi.org/10.1016/j.engfailanal.2025.110269)) — Oyane damage criterion and V-notch crack-location benchmark.

## Deliverables

`cases/forge_quench/`, `cases/quench_crack/`; sensitivity study; distortion-vs-hardness Pareto front; damage map; threshold sensitivity; B-level disclaimer.

## Validation & claims

Mesh convergence shown; surrogate error measured against the full model; digitisation uncertainty separated; crack-location prediction shown sensitive to the damage threshold.

## Limitations

B-level disclaimer required. NO claim of matching the 0.5 mm plant result. Predicted risk, not certified life.

## Repository layout

- `README.md` — case summary, data policy, method, results and limitations.
- `CONTRIBUTING.md` — how to propose changes.
- `docs/index.md` — documentation map.
- `docs/model_card.md` and `docs/vv_template.md` — reporting templates.
- `.github/workflows/ci.yml` — automated checks.

Only open data and published literature are used. No plant or proprietary data
are included. All artefacts are written in English.
