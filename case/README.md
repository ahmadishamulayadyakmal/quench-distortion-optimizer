# C10 · Quench distortion and cracking of large forgings — W40–W43

> **Real industrial case dossier.** Copied from the authoritative case card in
> `CASES.md` §4 so this repository stays self-contained after it is pushed to
> GitHub. Planning links: [`CASES.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/CASES.md) ·
> [`JOURNALS.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/JOURNALS.md) ·
> [`WEEKLY_PLAN.md`](https://github.com/ahmadishamulayadyakmal/metallurgy-project/blob/main/WEEKLY_PLAN.md).
> **Evidence level: A + B** · No plant data is held in this repository.

**Repository:** `e10-heat-treatment-inverse-design` · **Evidence: A + B** ·
**References:** R26, Y2R07, Y2R08.

**Industrial problem.** Water quenching of large forged blocks and high-alloy
tool steel creates thermal gradients, residual stress, distortion and cracks; a
wrong quench schedule scraps an expensive part (Y2R07, Y2R08).

**Why it happens.** Coupled thermal–phase transformation–stress behaviour, plus
damage accumulation where triaxiality and strain concentrate.

**Data (open + journal).** JMAK / Koistinen–Marburger kinetics (R26, analytical,
A); published FEM distortion and crack-location benchmarks (B, digitised);
literature property ranges with uncertainty; open surrogate geometry.

**Tool chain.** property table with uncertainty → simplified FEM thermal–phase–
stress coupling → Oyane damage criterion (Y2R08) → mesh convergence → surrogate
for quench-medium choice → Pareto study (distortion vs hardness) → surrogate
error vs full model.

**What each reference validates.**
- R26 — JMAK and martensite-fraction kinetics for the phase model.
- Y2R07 — quench-distortion FEM and the 0.5 mm **external** plant result.
- Y2R08 — Oyane damage criterion and V-notch crack-location benchmark.

**Deliverables.** `cases/forge_quench/`, `cases/quench_crack/`; sensitivity study;
distortion-vs-hardness front; damage map; threshold sensitivity; B-level
disclaimer.

**Validation.** Mesh convergence shown; surrogate error measured; digitisation
uncertainty separated; "predicted risk, not certified life" limitation stated.

**Acceptance.** No claim of matching the 0.5 mm plant result; crack-location
prediction shown sensitive to the damage threshold.

## Claim boundary

See [`evidence.md`](evidence.md) for the evidence level and the exact wording
that must be used when quoting literature numbers. All datasets and references
are listed in [`sources.md`](sources.md); the four-week execution plan is in
[`week_plan.md`](week_plan.md).
