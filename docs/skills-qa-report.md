# Skills QA report — Testing Mode vs curriculum + gap list

**Date:** Oct 2, 2026 (Asia/Bangkok)  
**Inputs:** `testing-skills-1000.json` (1000) · `mathera-curriculum.json` (1132 core) · master gaps attachment

---

## Summary

- Testing skills: **1000** across **78** branches
- With `extends_skill_id`: **167** (invalid extends: **0**)
- Interactive ≠ none: **245**
- Gap themes with ≥1 testing skill: **33 / 33**
- Gap themes still uncovered (0 hits): **0**
- Near-duplicate name collisions vs core (heuristic): **83**

## Gap theme coverage

| Gap theme | Testing hits | Sample IDs |
|---|---:|---|
| Roman numerals | 4 | T.I.1.001, T.I.3.003, T.I.3.004, T.II.1.001 |
| Number bonds / fact fluency / times tables | 2 | T.I.4.003, T.II.2.001 |
| Money / coins | 12 | T.I.4.004, T.I.4.009, T.I.7.005, T.I.7.006, T.I.7.020 |
| Clock / elapsed / timetables | 13 | T.I.1.001, T.I.6.002, T.I.7.001, T.I.7.002, T.I.7.003 |
| Columnar / long mult / long div | 23 | T.I.4.001, T.I.4.002, T.I.4.009, T.II.1.002, T.II.1.003 |
| Imperial ↔ metric | 3 | T.II.9.001, T.II.9.022, T.II.9.024 |
| Bearings | 15 | T.III.8.003, T.V.6.004, T.V.6.017, T.V.7.001, T.V.7.002 |
| Plans and elevations | 5 | T.III.8.001, T.III.8.027, T.III.8.028, T.III.8.029, T.V.14.001 |
| Nets / surface area | 8 | T.II.9.013, T.III.8.002, T.III.8.011, T.III.8.018, T.III.8.022 |
| Circle theorems | 14 | T.V.8.001, T.V.8.002, T.V.8.003, T.V.8.004, T.V.8.005 |
| Exact trig 0/30/45/60/90 | 13 | T.III.8.019, T.V.6.001, T.V.6.002, T.V.6.011, T.V.6.019 |
| Sine/cosine rules / ½ab sin C | 6 | T.V.7.005, T.V.7.006, T.V.7.007, T.V.7.008, T.V.7.013 |
| Scale drawings | 2 | T.III.2.006, T.III.2.017 |
| Histograms unequal width / CF | 6 | T.III.9.004, T.III.9.005, T.III.9.025, T.III.9.028, T.IV.15.010 |
| Box plots / IQR | 7 | T.III.9.005, T.III.9.006, T.III.9.022, T.III.9.023, T.III.9.025 |
| Venn / tree / conditional | 17 | T.III.9.001, T.III.9.002, T.III.9.012, T.III.9.032, T.III.9.033 |
| AP Stats inference / simulation | 19 | T.III.9.015, T.IV.14.011, T.IV.14.012, T.VI.11.004, T.VI.11.006 |
| Financial / compound interest | 33 | T.III.1.006, T.III.3.003, T.III.3.004, T.III.3.005, T.III.3.006 |
| Compound units density/pressure/pay | 18 | T.II.2.008, T.III.2.001, T.III.2.002, T.III.2.003, T.III.2.004 |
| Standard form | 12 | T.III.1.001, T.III.1.002, T.III.1.003, T.III.1.004, T.III.1.005 |
| Surds / rationalise | 15 | T.III.4.004, T.III.4.005, T.III.4.006, T.III.5.004, T.IV.5.001 |
| Fractional indices | 4 | T.III.4.002, T.III.4.003, T.IV.5.004, T.IV.5.005 |
| Bounds / limits of accuracy | 21 | T.I.7.015, T.II.1.007, T.III.1.010, T.III.1.011, T.III.1.012 |
| Iteration | 9 | T.IV.7.008, T.IV.7.009, T.IV.7.010, T.IV.7.015, T.IV.7.021 |
| Product rule counting | 5 | T.III.9.007, T.IV.14.001, T.IV.14.002, T.V.10.014, T.IV.14.021 |
| Bar model / tape | 1 | T.III.2.014 |
| AP Calc FRQ / Euler / logistic | 74 | T.III.9.022, T.IV.14.014, T.IV.14.017, T.IV.14.018, T.IV.14.019 |
| Series / Taylor / polar / parametric | 52 | T.III.9.014, T.IV.2.010, T.IV.8.002, T.IV.13.004, T.IV.13.005 |
| GDC techniques | 15 | T.III.3.010, T.IV.7.014, T.IV.12.003, T.IV.12.006, T.IV.15.003 |
| Proof by induction | 3 | T.IV.13.012, T.V.1.002, T.V.1.003 |
| Voronoi / graph theory light | 4 | T.III.8.023, T.III.8.024, T.III.8.025, T.III.8.026 |
| Vectors / matrices bridge | 65 | T.IV.4.003, T.IV.4.004, T.V.7.014, T.V.13.003, T.VII.1.001 |
| Modelling cycle | 2 | T.IV.12.008, T.VI.7.009 |

## Missing or thin gap themes

### Still uncovered (0 testing skills matched)

- None of the scanned themes are fully empty.

### Thin (1–2 hits) — consider densifying later

- Number bonds / fact fluency / times tables (2)
- Scale drawings (2)
- Bar model / tape (1)
- Modelling cycle (2)

## Duplication vs core

Testing Mode is *supposed* to sit on the same branches as core. Close **name** overlap is expected for dialect drills (e.g. bearings, standard form) when core already has a thin leaf — the difference should be **wording, packaging, exam stems**, not a second Journey.

Heuristic close-name overlaps: **83**. Sample:

- `T.I.4.003` «Number bonds to 10 and 20 speed packs» ≈ core «number bonds to 10»
- `T.II.4.004` «Common factors and common multiples lists» ≈ core «common multiples»
- `T.II.5.004` «Improper fractions ↔ mixed numbers fluency» ≈ core «improper fractions»
- `T.II.6.003` «Multiply fractions by wholes and fractions» ≈ core «multiply fractions»
- `T.II.7.006` «Decimal × whole number money contexts» ≈ core «decimal × whole number»
- `T.II.9.015` «Area of triangles by counting half-squares» ≈ core «area of triangles»
- `T.III.1.009` «Absolute value equations simple (KS3)» ≈ core «absolute value equations»
- `T.III.2.007` «Sharing in a ratio three-part» ≈ core «sharing in a ratio»
- `T.III.3.003` «Compound interest (non-calc appreciation)» ≈ core «compound interest»
- `T.III.3.004` «Compound interest depreciation / decay» ≈ core «compound interest»
- `T.III.4.007` «Scientific notation vs UK standard form wording» ≈ core «scientific notation»
- `T.III.6.010` «Quadratic inequalities intro via graphs» ≈ core «quadratic inequalities»
- `T.III.8.008` «Pythagoras in 3D (space diagonal)» ≈ core «pythagoras in 3d»
- `T.III.8.022` «Surface area of spheres leave in π» ≈ core «surface area of spheres»
- `T.III.9.026` «Experimental probability long-run estimate» ≈ core «experimental probability»
- `T.IV.5.007` «Simplify expressions with mixed surds and indices» ≈ core «simplify expressions»
- `T.IV.7.001` «Completing the square exam method pack» ≈ core «completing the square»
- `T.IV.7.002` «Turning points via completing the square» ≈ core «completing the square»
- `T.IV.7.004` «Quadratic formula exact surd answers» ≈ core «quadratic formula»
- `T.IV.7.011` «Quadratic inequalities critical values method» ≈ core «quadratic inequalities»
- `T.IV.7.013` «Hidden quadratics (exp/trig substitutions)» ≈ core «trig substitution»
- `T.IV.2.001` «Function notation f(x) exam fluency» ≈ core «function notation»
- `T.IV.2.004` «Inverse functions algebraically» ≈ core «inverse functions»
- `T.IV.2.005` «Piecewise functions interpret and graph» ≈ core «piecewise functions»
- `T.IV.2.011` «Self-inverse functions recognition» ≈ core «inverse functions»
- … +58 more

### Watchlist (dialect may be too close to core)

- Skills whose `why` is thin and `extends_skill_id` is null while name ≈ core — prefer linking `extends_skill_id` in a later pass.
- Era VII testing is a **bridge**; avoid implying full lin-alg / multivariable course parity.
- Interactive flags (`desmos`/`gdc`/…) must not ship as static-only clones of core generators without the tool.

## Pedagogy / product gaps (from master list) NOT skill-bank work

These remain **out of scope** for the 1000 testing skills (need product/eng):

- Per-skill video + post-miss walkthrough
- Cool-downs / exit tickets / station rotations
- Polypad-style manipulative canvas; bar-model CPA kit build
- Teacher snapshots / diagnostics suites
- Live Era VI generators at Journey parity

## Question bank QA snapshot

- Questions: **3000** (3 × 1000)
- Unique prompts: **3000**
- Lab prompts: **245**
- Calculator mix: {'never': 1917, 'allowed': 948, 'gdc': 135}
- Track flavour: {'neutral': 1000, 'UK': 1162, 'US': 522, 'IB': 316}

## Verdict

**Pass for beta catalog:** dialect coverage hits the main UK/IB/AP gap themes (bearings, bounds, surds, standard form, circle theorems, FRQ/GDC, stats procedures). Tighten bar-model/tape packaging and any remaining thin themes in a revision pass; keep pedagogy tools on the eng roadmap.
