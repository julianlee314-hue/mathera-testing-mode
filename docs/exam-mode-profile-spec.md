# Exam Mode Profile Spec (Testing Mode overlay)

Short product spec for how **Testing Mode** sits on the Mathera tree without becoming a second curriculum.

## Goals

1. Learners (or teachers) select one or more **exam tracks**.
2. The existing era/branch/skill tree **highlights** matching testing skills; core journey skills stay visible.
3. Practice can be **custom** (pick tracks + branches) or **automated** (suggested packs for a named exam path).
4. Eras keep their personality via **notebook-per-era** paper designs in the testing UI.

Testing skills never replace core leaves. They are an overlay (`mode: "testing"`), linked by `branch_id` and optional `extends_skill_id`.

---

## Profile fields (track selection)

Suggested user/profile object (additive to existing Mathera profile):

```json
{
  "exam_mode": {
    "enabled": true,
    "tracks": ["UK_GCSE_H", "IB_AA_SL"],
    "intensity": "balanced",
    "include_uncertain": false,
    "include_strange": true,
    "interactive_prefs": ["desmos", "unit_circle", "gdc"],
    "auto_pack": null
  }
}
```

| Field | Type | Meaning |
|-------|------|---------|
| `enabled` | bool | Show Testing Mode overlay on the tree |
| `tracks` | string[] | Subset of `UK_KS2`, `UK_KS3`, `UK_GCSE_F`, `UK_GCSE_H`, `IB_MYP`, `IB_AA_SL`, `IB_AA_HL`, `IB_AI_SL`, `IB_AI_HL`, `US_CCSS_K5`, `US_CCSS_68`, `US_CCSS_HS`, `AP_CALC_AB`, `AP_CALC_BC`, `AP_STATS` |
| `intensity` | enum | `light` (core only) · `balanced` (core+challenge) · `full` (+strange) |
| `include_uncertain` | bool | Show IB items marked `"uncertain": true` (Voronoi, etc.) |
| `include_strange` | bool | Override/pair with intensity for niche enrichment |
| `interactive_prefs` | string[] | Prefer skills with these `interactive` flags when surfacing packs |
| `auto_pack` | string\|null | Named automated pack id, or null for fully custom |

**Track chips UX:** multi-select; show count of matching testing skills live. Warn if tracks span wildly different eras (e.g. UK_KS2 + AP_CALC_BC) but allow — Mathera refuses gates.

---

## How tree highlighting works

1. **Base tree** = core curriculum (1132 skills), unchanged.
2. **Overlay badges** on a branch when ≥1 testing skill matches the profile filter:
   - Filter = `tracks` ∩ skill.tracks nonempty
   - AND difficulty allowed by `intensity` / `include_strange`
   - AND (`include_uncertain` OR not skill.uncertain)
3. **Branch glow / pill:** e.g. `+12 testing` on `V.7 General triangles`.
4. **Skill row:** testing skills listed under the branch as a secondary list (or toggle "Show testing").
5. **Extends link:** if `extends_skill_id` is set (e.g. `V.7.08`), show a thin edge or "extends Bearings & navigation" caption — learner can jump to core then into dialect drills.
6. **No duplicate mastery:** proving a testing skill does **not** auto-prove the core skill (and vice versa), unless product later adds an explicit "dialect credit" rule.

```
Era V ▸ V.7 General triangles
  Core: V.7.01 … V.7.09
  Testing (UK_GCSE_H): T.V.7.001 Bearings: three-figure notation drills  ⚙geometry
                       T.V.7.002 Bearings: reverse bearings …
```

---

## Customizable vs automated exam modes

### Customizable (default)

Learner/teacher picks tracks + optional branch filters + intensity.  
Practice queue = generators for matching `T.*` skills (and optionally interleaved core).  
Good for: mixed classrooms, tutoring, "I need bearings + bounds this week."

### Automated packs (suggested starters)

Named packs preset `tracks`, default intensity, and a recommended era window:

| Pack id | Tracks | Focus eras | Notes |
|---------|--------|------------|-------|
| `uk_ks2_sats` | UK_KS2 | I–II | Formal methods, money, time, MD |
| `uk_gcse_f` | UK_GCSE_F, UK_KS3 | III–V | Foundation paper dialects |
| `uk_gcse_h` | UK_GCSE_H | III–V (+ light VI tease) | Surds, circle theorems, bearings, bounds, iteration |
| `ib_myp` | IB_MYP | III–V | Conceptual bridge, not eAssessment clone |
| `ib_aa_sl` | IB_AA_SL | IV–VI | Analytic emphasis, GDC where tagged |
| `ib_aa_hl` | IB_AA_HL | IV–VII light | Induction, complex, series, matrices |
| `ib_ai_sl` | IB_AI_SL | IV–VI | Modelling + stats + GDC |
| `ib_ai_hl` | IB_AI_HL | IV–VII light | Inference depth; Voronoi only if uncertain allowed |
| `us_ccss_k8` | US_CCSS_K5, US_CCSS_68 | I–III | MD/RP/SP dialects |
| `us_ccss_hs` | US_CCSS_HS | IV–V (+ VII bridge) | G-GPE, N-VM (+) |
| `ap_calc_ab` | AP_CALC_AB | VI | FRQ justification, Euler, logistic |
| `ap_calc_bc` | AP_CALC_BC | VI | + series, polar/parametric |
| `ap_stats` | AP_STATS | III–IV, VI.11 | Procedures + communication |

Automated packs are **starting profiles**, not locked rails — user can fork to custom anytime.

### Calculator / GDC policy

Respect per-skill `interactive: gdc` and future calculator enums. AP packs should expose **calc-active vs calc-inactive** practice toggles (see `T.VI.3.*` calculator-active/inactive skill).

---

## Notebook-per-era UI notes (fun paper designs)

Testing Mode practice screens can feel like **exam notebooks** without becoming grim past-paper PDFs. Each era gets a paper personality; content is still Mathera generators.

| Era | Notebook vibe | Visual cues |
|-----|---------------|-------------|
| **I Count** | Infant exercise book | Wide ruled, big margin animals/shapes stamp, soft green |
| **II Operate** | Primary jotter | Squared paper light grid, red margin line, pencil texture |
| **III Relate** | KS3 exercise book | Blue biro energy, proportion tables, "show your working" banner |
| **IV Solve** | GCSE / algebra pad | Squared + working columns; exact-answer vs approx toggle chip |
| **V Prove** | Geometry folio | Compass rose watermark, construction arcs, proof reason bank |
| **VI Change** | AP / IB pad | FRQ-style multi-part boxes (a)(b)(c); GDC sticky note; justification sentence frames |
| **VII Space** | Further / HL sketchbook | Matrix grids, vector arrows, "bridge not full Space" ribbon |

### Shared UI chrome

- **Track ribbon** at top: active track chips.
- **Mode pill:** `Testing` distinct from core `Journey`.
- **Difficulty pip:** core / challenge / strange.
- **Interactive launchers:** Desmos / unit circle / geometry / GDC when `interactive ≠ none`.
- **Why tooltip:** show skill.why (≤12 words gap reason) for teacher transparency.
- **Uncertain badge:** only if profile allows; copy: "Verify against your IB guide."

### Accessibility

- Paper textures optional (reduce motion / high contrast themes strip textures).
- Notebook metaphor must not imply real exam timing by default; optional timer is a separate toggle.

---

## Data contract

Canonical file: `exam-mode/testing-skills-1000.json`

Required fields per skill: `id`, `name`, `description`, `era`, `branch_id`, `branch_name`, `tracks`, `mode` (`"testing"`), `difficulty`, `interactive`, `extends_skill_id`, `why`, `global_order`.  
Optional: `uncertain`.

Do not push these into the core curriculum JSON; keep under `/workspace/mathera/exam-mode/`.

---

## Non-goals

- Not an exam board; not GCSE/IB/AP mark schemes as product truth.
- Not a paywalled past-paper library.
- Not a full A-level / Further Maths / Space replacement (Era VII testing is a **light bridge** only).
- Not Scotland/Wales/NI / TEKS dialects in v1 (noted as future).
