# Ship checklist — Testing Mode / The Notebooks → Mathera

**Version intent:** Mathera **1.x → Testing Mode β**  
**Date:** Oct 2, 2026 (Asia/Bangkok)  
**Title lock:** **The Notebooks** (see `NOTEBOOKS_CONCEPT.md`)

---

## 1. What lands in the Mathera app

### Schema — testing skills

Canonical file: `exam-mode/testing-skills-1000.json` (array of 1000).

| Field | Required | Notes |
|-------|----------|-------|
| `id` | ✓ | `T.{era}.{branch}.{nnn}` e.g. `T.V.7.001` |
| `name`, `description` | ✓ | Dialect-facing |
| `era`, `branch_id`, `branch_name` | ✓ | Must exist on core tree |
| `tracks` | ✓ | Subset of profile track enums |
| `mode` | ✓ | Always `"testing"` |
| `difficulty` | ✓ | `core` \| `challenge` \| `strange` |
| `interactive` | ✓ | `none` \| `desmos` \| `geometry` \| `gdc` \| `unit_circle` \| `graph` |
| `extends_skill_id` | ✓ nullable | Core skill id or null |
| `why` | ✓ | Short gap reason |
| `global_order` | ✓ | 1…1000 |
| `uncertain` | optional | IB verify-against-guide |

**Do not merge** these into core `mathera-curriculum.json`. Load as overlay.

### Schema — questions

Canonical: `exam-mode/question-bank.json` (3000 objects). Shards: `exam-mode/question-bank/questions-era-*.json`.

```json
{
  "qid": "Q.T.V.7.001.a",
  "skill_id": "T.V.7.001",
  "part": "a",
  "prompt": "…",
  "answer": "…",
  "solution": "1–3 short steps",
  "marks": 1,
  "calculator": "never|allowed|gdc",
  "track_flavor": "UK|IB|US|neutral",
  "era": "V",
  "branch_id": "V.7",
  "lab_prompt": false
}
```

Interactive-heavy skills: parts **a/b** written; part **c** often `lab_prompt: true`.

### Profile tracks

Implement `exam_mode` object per `exam-mode-profile-spec.md`:

- `enabled`, `tracks[]`, `intensity`, `include_uncertain`, `include_strange`, `interactive_prefs[]`, `auto_pack`

### Tree highlight

1. Base tree = 1132 core skills (unchanged).  
2. Branch badge when ≥1 testing skill matches profile filter.  
3. Secondary list / toggle: “Show testing”.  
4. Optional edge caption when `extends_skill_id` set.  
5. **No auto-mastery crossover** in β.

### Notebook UI

Era paper skins I–VII from `NOTEBOOKS_CONCEPT.md` + dialect badges **UK · IB · US**.

---

## 2. What needs eng work

| Item | Priority | Notes |
|------|----------|-------|
| Generators wired to `T.*` ids | P0 | Static bank is β content; generators = volume |
| GDC mode / calc-active vs inactive | P0 | Especially AP + IB AI |
| FRQ rubrics / justification sentence frames | P1 | Era VI communication marks |
| Era VI **live** practice parity | P0–P1 | Mapped skills → runnable |
| Interactive hosts (Desmos, unit circle, geometry, GDC sticky) | P1 | Honor `interactive` flags |
| Auto packs | P1 | Table in profile spec |
| Dialect credit rule (optional) | P2 | Testing ↔ core mastery |
| Bar-model / tape tool | P2 | Pedagogy gap, not just questions |
| COMPUTE terminal skin | P3 | Lounge stretch |
| Scotland/Wales/NI / TEKS tracks | P3 | Post-β |

---

## 3. GitHub viewing

### Proposal

**New public repo:** `julianlee314-hue/mathera-testing-mode`  
(Alternative folder: `math-history-101/exam/` or `mathera/exam-mode/` — prefer **dedicated repo** so Pages URL is clean and PDFs don’t bloat the main app repo.)

### Exact steps

```bash
# 1) Create repo (if not exists)
gh repo create julianlee314-hue/mathera-testing-mode \
  --public \
  --description "Mathera Testing Mode — The Notebooks: 1000 dialect skills + 3000 practice questions" \
  --source . --remote origin  # or create empty then push

# 2) From a clean publish folder containing:
#    testing-skills-1000.json
#    question-bank.json
#    question-bank/
#    *.pdf (master and/or per-era)
#    NOTEBOOKS_CONCEPT.md
#    exam-mode-profile-spec.md
#    TESTING_SKILLS_CATALOG.md
#    skills-qa-report.md
#    SHIP_TO_MATHERA.md
#    index.html (optional Pages landing)

# 3) Push
git init   # if needed
git add .
git commit -m "Testing Mode β: The Notebooks — skills, question bank, docs"
git branch -M main
git remote add origin https://github.com/julianlee314-hue/mathera-testing-mode.git
git push -u origin main

# 4) GitHub Pages
gh api repos/julianlee314-hue/mathera-testing-mode/pages \
  -X POST -f build_type=legacy -f source[branch]=main -f source[path]=/
# or: Settings → Pages → Deploy from branch main / (root) or /docs

# 5) Expected URL
# https://julianlee314-hue.github.io/mathera-testing-mode/
```

Optional: add Pages under `math-history-101` at `/exam/` only if Julius prefers one history site — still keep JSON in `mathera-testing-mode` for eng fetch.

---

## 4. Version bump notes — Mathera 1.x → Testing Mode β

| Area | 1.x | Testing Mode β |
|------|-----|----------------|
| Curriculum | 7 eras · 87 branches · 1132 skills | +1000 overlay skills (`mode: testing`) |
| Practice | Journey generators (I–V live; VI–VII mapped) | +3000 static dialect questions; generator roadmap |
| Profile | Journey prefs | +`exam_mode` tracks / intensity / packs |
| UI | Era chromatic Journey | +**The Notebooks** paper skins + UK·IB·US badges |
| Mastery | Core leaves | Testing mastery separate |
| Release tag suggestion | `v1.x` | `v1.x-testing-beta` or app flag `testingMode: true` |

**Changelog blurb (draft):**  
> Testing Mode β — *The Notebooks*. Choose UK, IB, or US tracks; the tree highlights ~1000 dialect drills without replacing the Journey. Practice pack includes 3000 starter questions. GDC/FRQ/live Era VI generators still rolling out.

---

## File checklist before push

- [x] `testing-skills-1000.json`  
- [x] `question-bank.json` + era shards  
- [x] `NOTEBOOKS_CONCEPT.md`  
- [x] `exam-mode-profile-spec.md`  
- [x] `skills-qa-report.md`  
- [x] `SHIP_TO_MATHERA.md`  
- [x] Visual PDF(s)  
- [x] GitHub repo + Pages  

