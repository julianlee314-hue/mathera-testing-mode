# The Notebooks — Testing Mode concept lock

**Working title (recommended):** **The Notebooks**  
**Alternates:** *Era Notebooks* · *The Long Lounge of Notebooks*

**Product frame:** Testing Mode is not a second curriculum. It is a **dialect overlay** on Mathera’s seven learner Eras (I–VII) — exam-flavoured practice that sits on existing `branch_id`s. Learners still walk the Journey tree; Notebooks light up when a profile track is active.

**World vibe:** Over the Garden Wall–adjacent lounge feeling only (aged paper, quiet lamps, drafting tools). **No show IP**, characters, or titles.

---

## Title recommendation

Ship as **The Notebooks** in UI chrome and marketing:

- Short, collectible, soft — not “Exam Drill Factory.”
- Leaves room for later skins (scrolls → fat notebooks → 80s/90s school terminal).
- Pair with subtitle: *Testing Mode · UK · IB · US*.

Use *Era Notebooks* if “The Notebooks” collides with another Julius product name.  
Use *The Long Lounge of Notebooks* only for landing/lore pages, not in-app nav.

---

## Media evolution across Eras (learner Eras I–VII)

These are **paper personalities**, not Chinese historical Epochs.

| Era | Name | Notebook medium | Palette / cues |
|-----|------|-----------------|----------------|
| **I** | Count | Stone tablets / tally notches | Warm tan, carved grooves, notch marks |
| **II** | Operate | Gears / early mechanism jotter | Brown–orange, cog watermarks, squared margin |
| **III** | Relate | Graph-paper coordinate lounge | Blue grid, coffee ring optional, biro energy |
| **IV** | Solve | Charcoal algebra folio | Charcoal/grey, equation gutter, working columns |
| **V** | Prove | Cream construction folio | Cream stock, compass rose, arc scratches |
| **VI** | Change | Dark green lab notebook | Forest green, FRQ (a)(b)(c) boxes, GDC sticky |
| **VII** | Space | Muted purple wireframe journal | Muted purple, matrix grids, vector arrows |

**Mood-board palette (shared):** aged paper · grids · muted tan / green / purple / charcoal · coffee ring · drafting tools (compass, set square, pencil).

### Future lounge stretch (COMPUTE skin)

Julius’s longer arc for the lounge UI:

1. **Long scrolls** — early / lore mode  
2. **Fat notebooks** — default Testing Mode (this doc)  
3. **80s/90s school computer terminal** — later skin for **COMPUTE**-flavoured testing (amber/green phosphor, block cursor, floppy-era menu chrome)

Treat (3) as a **theme pack**, not a new skill map.

---

## Dialect principles (UK / IB / US)

Dialects are **profile overlays**, not parallel trees. Spec source: `exam-mode-profile-spec.md`.

### Principles

1. **One map, many accents.** Core skill IDs stay Mathera; testing IDs are `T.{branch}.{nnn}` with `mode: "testing"`.
2. **Tracks are multi-select.** A learner can hold `UK_GCSE_H` + `IB_AA_SL` without forking the Journey.
3. **Wording follows the track.**  
   - **UK:** three-figure bearings, standard form, surds, bounds, bus-stop, “show your working.”  
   - **IB:** GDC workflows, modelling cycle language, AA vs AI flavour, induction write-ups, “uncertain” badge for verify-against-guide items.  
   - **US / AP:** FRQ justification frames, calculator-active vs inactive, SOCS, z-procedures, CCSS vocabulary where tagged.
4. **No board cosplay as truth.** Notebooks are practice dialects, not past-paper libraries or official mark schemes.
5. **Extends, doesn’t overwrite.** `extends_skill_id` may point at a core leaf; mastery is separate unless product later adds explicit dialect credit.
6. **Intensity gates density, not eras.** `light` / `balanced` / `full` (± strange / uncertain) — see profile spec.
7. **Calculator honesty.** Per-question `calculator`: `never` | `allowed` | `gdc`.

### Track chips (v1)

`UK_KS2` · `UK_KS3` · `UK_GCSE_F` · `UK_GCSE_H` · `IB_MYP` · `IB_AA_SL` · `IB_AA_HL` · `IB_AI_SL` · `IB_AI_HL` · `US_CCSS_K5` · `US_CCSS_68` · `US_CCSS_HS` · `AP_CALC_AB` · `AP_CALC_BC` · `AP_STATS`

Future (not v1): Scotland/Wales/NI, TEKS, SAT/ACT packs.

---

## UI chrome (Testing Mode)

- **Track ribbon** — active dialect chips  
- **Mode pill** — `Testing` vs Journey  
- **Difficulty pip** — core / challenge / strange  
- **Interactive launchers** — Desmos / unit circle / geometry / GDC when flagged  
- **Why tooltip** — skill.why (gap transparency)  
- **Paper textures optional** — reduce-motion / high-contrast strips textures  
- **Timer off by default** — exam timing is an explicit toggle, never implied by notebook chrome  

---

## Data anchors

| Artefact | Path |
|----------|------|
| Testing skills (1000) | `exam-mode/testing-skills-1000.json` |
| Question bank (3000) | `exam-mode/question-bank.json` |
| Era shards | `exam-mode/question-bank/questions-era-*.json` |
| Profile spec | `exam-mode/exam-mode-profile-spec.md` |
| Ship checklist | `exam-mode/SHIP_TO_MATHERA.md` |
| Skills QA | `exam-mode/skills-qa-report.md` |

---

## Non-goals

- Not an exam board  
- Not a paywalled past-paper vault  
- Not full A-level Further / complete Space replacement (Era VII testing = light bridge)  
- Not Chinese Epoch labelling for these seven media skins  

*Locked for Julius · Oct 2, 2026 (Asia/Bangkok).*
