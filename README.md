# Quench distortion and cracking of large forgings (C10)

> Workspace folder: `e10-heat-treatment-inverse-design` · Suggested GitHub repository: `metallurgy-heat-treatment`
> Epic: E10 · Weeks: W40–W43 · Evidence level: **A + B**
> Master specification: [`CASES.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/CASES.md) §4 · Download the papers: [`JOURNALS.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/JOURNALS.md)

## Industrial problem

Water quenching of large forged blocks and high-alloy tool steel creates thermal gradients, residual stress, distortion and cracks; a wrong quench schedule scraps an expensive part.

**Why it happens.** Coupled thermal – phase transformation – stress behaviour, plus damage accumulation where triaxiality and strain concentrate.

## Data (no plant data)

Mixed: JMAK / Koistinen–Marburger kinetics are analytical (A, R26); published FEM distortion and crack-location benchmarks are digitised (B, Y2R07/Y2R08); literature property ranges with uncertainty; open surrogate geometry. No plant data is held.

> The author cannot supply factory data. This project uses **only open datasets and
> credible peer-reviewed journals**. If this is a B-level case, the case report
> must contain the exact disclaimer from `CASES.md` §1 and must **never** claim
> plant validation.

## Tool chain

Simplified FEM thermal–phase–stress coupling, Oyane damage criterion, JMAK / Koistinen–Marburger kinetics, mesh convergence, surrogate for quench-medium choice, Pareto study (distortion vs hardness), SHAP-style sensitivity.

## Journal references

- **R26** — JMAK and martensite-fraction kinetics (compound: 2 papers).
- **Y2R07** — quench-distortion FEM and the external 0.5 mm plant result.
- **Y2R08** — Oyane damage criterion and V-notch crack-location benchmark.

Each reference above is listed with its DOI or stable URL, access status and
manual download route in [`JOURNALS.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/JOURNALS.md) §4, and in the shared
BibTeX library `papers/references.bib`. Do not cite a paper you have not been
able to obtain; if it is inaccessible, record that in `JOURNALS.md` §8.

## Deliverables

`cases/forge_quench/`, `cases/quench_crack/`; sensitivity study; distortion-vs-hardness Pareto front; damage map; threshold sensitivity; B-level disclaimer.

## Validation & claims

Mesh convergence shown; surrogate error measured against the full model; digitisation uncertainty separated; crack-location prediction shown sensitive to the damage threshold.

## Limitations

B-level disclaimer required. NO claim of matching the 0.5 mm plant result. Predicted risk, not certified life.

## Definition of Done

1 merged PR · green tests · 1 new artefact · 1 README paragraph · 1 sprint note
`docs/sprints/wNN.md` · tag `wNN`. Before the case tag `c10` is created,
this README must contain all six sections: Industrial problem, Data (no plant
data), Tool chain, Journal references, Validation & claims, Limitations.

## Repository skeleton

Shared files: `CONTRIBUTING.md` (sprint contract), `.github/` (issue, PR and
CI templates), `docs/sprints/wNN.md`, `docs/vv_template.md` and
`docs/model_card.md`. `CASES.md`, `JOURNALS.md` and `REPOSITORIES.md` are in a
separate planning repository; their links above remain valid after this folder
is pushed as its own repository.

The real industrial case dossier is in `case/`: `README.md` (full case card),
`evidence.md`, `sources.md` and `week_plan.md`.

## Push this folder to GitHub

This folder is prepared but is **not** a Git repository yet:

```bash
cd e10-heat-treatment-inverse-design
git init
git branch -M main
git remote add origin https://github.com/<your-user>/metallurgy-heat-treatment.git
git add .
git commit -m "Initial import: C10 · W40–W43"
git push -u origin main
```

Use weekly tags `wNN` and one case tag `c10` inside this repository.
Never commit API keys, raw downloaded datasets or publisher PDFs.

## Language

All artefacts in this repository are written in **English**.
