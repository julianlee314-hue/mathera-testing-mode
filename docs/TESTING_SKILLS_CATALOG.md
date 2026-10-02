# Mathera Testing Mode Skill Catalog

~1000 supplemental **testing-mode / dialect** skills that sit **on top of** the core Mathera curriculum (7 eras · 87 branches · 1132 skills).

These are **not** a parallel journey. They are exam-flavoured overlays: UK formal methods and GCSE Higher packaging, IB GDC/modelling dialects, AP Calc FRQ justification language, AP Stats procedures, and niche paper topics (bearings, bounds, unequal histograms, circle theorems, surds, standard form, financial math, etc.).

Every skill maps to an existing `branch_id`. Field `mode` is always `"testing"`. IDs use `T.{branch_id}.{nnn}` with global_order 1…N.

Source gap papers (Oct 2026): Mathera vs UK NC · Mathera vs IB · Mathera vs CCSSM+AP · Khan context.

---

## Summary counts

**Total skills:** 1000

### By era

| Era | Name | Skills | Design target |
|-----|------|-------:|--------------:|
| I | Count | 56 | ~120 I–II |
| II | Operate | 97 | (with I) |
| III | Relate | 176 | ~150 |
| IV | Solve | 181 | ~180 |
| V | Prove | 216 | ~220 |
| VI | Change | 201 | ~200 |
| VII | Space | 73 | ~50 |
| **I+II** | primary dialects | **153** | ~120 |

### By track

| Track | Skills tagged |
|-------|-------------:|
| `UK_KS2` | 153 |
| `UK_KS3` | 147 |
| `UK_GCSE_F` | 115 |
| `UK_GCSE_H` | 473 |
| `IB_MYP` | 148 |
| `IB_AA_SL` | 490 |
| `IB_AA_HL` | 458 |
| `IB_AI_SL` | 373 |
| `IB_AI_HL` | 211 |
| `US_CCSS_K5` | 15 |
| `US_CCSS_68` | 26 |
| `US_CCSS_HS` | 124 |
| `AP_CALC_AB` | 135 |
| `AP_CALC_BC` | 206 |
| `AP_STATS` | 92 |

### Difficulty & interactive

- Difficulty: core 646 · challenge 311 · strange 43
- Interactive flags: none 755, geometry 91, desmos 77, gdc 35, unit_circle 28, graph 14
- Trig branches V.6–V.10: **166** skills · of which interactive: **95**
- Marked `uncertain: true` (verify IB guide): **8**

---

## Full list by branch

### Era I — Count

#### `I.1` Counting (6)

- `T.I.1.001` **Count in Roman numerals to XII** — `UK_KS2`
- `T.I.1.002` **Cardinality: last number said is how many** — `US_CCSS_K5,UK_KS2`
- `T.I.1.003` **Subitize small sets without counting** — `US_CCSS_K5,UK_KS2`
- `T.I.1.004` **Skip-count by 2, 5, 10 exam drills** — `UK_KS2,US_CCSS_K5`
- `T.I.1.005` **Count in steps of 3 and 4** — `UK_KS2`
- `T.I.1.006` **Count back through zero into negatives** — `UK_KS2,UK_KS3` · challenge

#### `I.2` Comparing & ordering (3)

- `T.I.2.001` **Compare using more/fewer/equal SATs stems** — `UK_KS2`
- `T.I.2.002` **Order lengths and masses with units** — `UK_KS2,US_CCSS_K5`
- `T.I.2.003` **Order numbers to 100 with inequality signs** — `UK_KS2,US_CCSS_K5`

#### `I.3` Place value (6)

- `T.I.3.001` **Partition with UK part–whole models** — `UK_KS2`
- `T.I.3.002` **Write numbers in expanded form (UK wording)** — `UK_KS2`
- `T.I.3.003` **Roman numerals to 100 (I–C)** — `UK_KS2`
- `T.I.3.004` **Roman numerals to 1,000 (M)** — `UK_KS2` · challenge
- `T.I.3.005` **Exchange ten ones for one ten** — `UK_KS2,US_CCSS_K5`
- `T.I.3.006` **Flexibly partition numbers many ways** — `UK_KS2,US_CCSS_K5`

#### `I.4` Addition & subtraction (9)

- `T.I.4.001` **Column addition (Appendix formal method)** — `UK_KS2`
- `T.I.4.002` **Column subtraction with exchange** — `UK_KS2`
- `T.I.4.003` **Number bonds to 10 and 20 speed packs** — `UK_KS2`
- `T.I.4.004` **Add/subtract money in £ and p** — `UK_KS2`
- `T.I.4.005` **Worded multi-step add/sub (SATs style)** — `UK_KS2` · challenge
- `T.I.4.006` **Near doubles addition strategies** — `UK_KS2,US_CCSS_K5`
- `T.I.4.007` **Bridging through 10 subtraction** — `UK_KS2`
- `T.I.4.008` **Inverse operations check add/sub** — `UK_KS2,US_CCSS_K5`
- `T.I.4.009` **Column methods with money £.p** — `UK_KS2`

#### `I.5` Patterns & logic (2)

- `T.I.5.001` **Repeating pattern SAT stems** — `UK_KS2,US_CCSS_K5`
- `T.I.5.002` **Missing-number sentences with boxes** — `UK_KS2`

#### `I.6` Shape & space (4)

- `T.I.6.001` **Name 2D shapes with UK vocabulary** — `UK_KS2`
- `T.I.6.002` **Turns: quarter, half, three-quarter, full** — `UK_KS2`
- `T.I.6.003` **Left/right and compass directions early** — `UK_KS2`
- `T.I.6.004` **Symmetry: complete mirror patterns** — `UK_KS2,US_CCSS_K5`

#### `I.7` Measure & data (26)

- `T.I.7.001` **Tell time to the nearest minute (analogue)** — `UK_KS2`
- `T.I.7.002` **12-hour clock with am/pm** — `UK_KS2`
- `T.I.7.003` **24-hour clock conversion** — `UK_KS2`
- `T.I.7.004` **Read simple bus/train timetables** — `UK_KS2` · challenge
- `T.I.7.005` **British coins and notes identification** — `UK_KS2`
- `T.I.7.006` **Give change from £1, £5, £10, £20** — `UK_KS2`
- `T.I.7.007` **Temperature in °C: read and compare** — `UK_KS2`
- `T.I.7.008` **Tally charts exam pack** — `UK_KS2`
- `T.I.7.009` **Pictograms with keys (one symbol = many)** — `UK_KS2`
- `T.I.7.010` **Block diagrams / bar charts simple scale** — `UK_KS2`
- `T.I.7.011` **Measure length in cm and mm** — `UK_KS2`
- `T.I.7.012` **Mass in g and kg comparison** — `UK_KS2`
- `T.I.7.013` **Capacity in ml and l** — `UK_KS2`
- `T.I.7.014` **CCSS line plots with fractional lengths** — `US_CCSS_K5,UK_KS2` · challenge
- `T.I.7.015` **Elapsed time across hour boundaries** — `UK_KS2` · challenge
- `T.I.7.016` **Calendar: days in months fluency** — `UK_KS2`
- `T.I.7.017` **Compare durations in hours and minutes** — `UK_KS2`
- `T.I.7.018` **Weigh using scales reading dials** — `UK_KS2`
- `T.I.7.019` **Capacity practical measuring jugs** — `UK_KS2`
- `T.I.7.020` **Money change multi-item shop 1** — `UK_KS2`
- `T.I.7.021` **Money change multi-item shop 2** — `UK_KS2`
- `T.I.7.022` **Money change multi-item shop 3** — `UK_KS2`
- `T.I.7.023` **Money change multi-item shop 4** — `UK_KS2`
- `T.I.7.024` **Timetable reading scenario 1** — `UK_KS2`
- `T.I.7.025` **Timetable reading scenario 2** — `UK_KS2`
- `T.I.7.026` **Timetable reading scenario 3** — `UK_KS2`

### Era II — Operate

#### `II.1` Place value to millions (11)

- `T.II.1.001` **Roman numerals review in large-number context** — `UK_KS2`
- `T.II.1.002` **Formal column addition multi-digit exam pack** — `UK_KS2`
- `T.II.1.003` **Formal column subtraction multi-digit exam pack** — `UK_KS2`
- `T.II.1.004` **Round to estimate before calculating (UK)** — `UK_KS2`
- `T.II.1.005` **Numbers to 10 million reading/writing** — `UK_KS2`
- `T.II.1.006` **Negative numbers on number lines (Y5)** — `UK_KS2`
- `T.II.1.007` **Count forwards/backwards in powers of 10** — `UK_KS2`
- `T.II.1.008` **Compare numbers using place-value charts** — `UK_KS2`
- `T.II.1.009` **Formal column methods mixed 1** — `UK_KS2`
- `T.II.1.010` **Formal column methods mixed 2** — `UK_KS2`
- `T.II.1.011` **Formal column methods mixed 3** — `UK_KS2`

#### `II.2` Multiplication (11)

- `T.II.2.001` **12×12 tables fluency milestone pack** — `UK_KS2`
- `T.II.2.002` **Long multiplication (formal written method)** — `UK_KS2`
- `T.II.2.003` **Grid / area-model to column bridge** — `UK_KS2,US_CCSS_K5`
- `T.II.2.004` **Multiplication worded multi-step SATs** — `UK_KS2` · challenge
- `T.II.2.005` **Multiply by 10, 100, 1000 place-value moves** — `UK_KS2`
- `T.II.2.006` **Square numbers visual arrays pack** — `UK_KS2`
- `T.II.2.007` **Distributive property for mental mult** — `UK_KS2`
- `T.II.2.008` **Multiples vs factors language traps** — `UK_KS2`
- `T.II.2.009` **Long multiplication accuracy set 1** — `UK_KS2`
- `T.II.2.010` **Long multiplication accuracy set 2** — `UK_KS2`
- `T.II.2.011` **Long multiplication accuracy set 3** — `UK_KS2`

#### `II.3` Division (10)

- `T.II.3.001` **Long division formal method (one-digit divisor)** — `UK_KS2`
- `T.II.3.002` **Long division by two-digit divisors** — `UK_KS2` · challenge
- `T.II.3.003` **Division with remainders as fractions/decimals** — `UK_KS2`
- `T.II.3.004` **Short division (bus-stop) method fluency** — `UK_KS2`
- `T.II.3.005` **Division worded multi-step SATs** — `UK_KS2` · challenge
- `T.II.3.006` **Chunking division as bridge method** — `UK_KS2`
- `T.II.3.007` **Worded division sharing vs grouping** — `UK_KS2`
- `T.II.3.008` **Long division accuracy set 1** — `UK_KS2`
- `T.II.3.009` **Long division accuracy set 2** — `UK_KS2`
- `T.II.3.010` **Long division accuracy set 3** — `UK_KS2`

#### `II.4` Factors & multiples (4)

- `T.II.4.001` **Prime numbers to 100 recognition drills** — `UK_KS2,UK_KS3`
- `T.II.4.002` **HCF and LCM worded problems (UK)** — `UK_KS2,UK_KS3`
- `T.II.4.003` **Square and cube numbers recall pack** — `UK_KS2`
- `T.II.4.004` **Common factors and common multiples lists** — `UK_KS2`

#### `II.5` Fractions I (6)

- `T.II.5.001` **Unit fractions of amounts (UK wording)** — `UK_KS2`
- `T.II.5.002` **Non-unit fractions of amounts** — `UK_KS2` · challenge
- `T.II.5.003` **Equivalent fractions wall fluency** — `UK_KS2,US_CCSS_K5`
- `T.II.5.004` **Improper fractions ↔ mixed numbers fluency** — `UK_KS2`
- `T.II.5.005` **Fractions greater than 1 on number lines** — `UK_KS2`
- `T.II.5.006` **Fraction of a set with remainders context** — `UK_KS2` · challenge

#### `II.6` Fractions II (8)

- `T.II.6.001` **Add/subtract fractions same denominator exam** — `UK_KS2`
- `T.II.6.002` **Add/subtract mixed numbers exam pack** — `UK_KS2,UK_KS3`
- `T.II.6.003` **Multiply fractions by wholes and fractions** — `UK_KS2`
- `T.II.6.004` **Divide fractions by wholes (Y6)** — `UK_KS2`
- `T.II.6.005` **Fraction ↔ decimal ↔ percent early bridge** — `UK_KS2`
- `T.II.6.006` **Simplify fractions to lowest terms** — `UK_KS2`
- `T.II.6.007` **Fraction of a remaining amount multi-step** — `UK_KS2,UK_KS3` · challenge
- `T.II.6.008` **Compare fractions with different denominators** — `UK_KS2`

#### `II.7` Decimals (7)

- `T.II.7.001` **Money calculations with £ and p (two decimals)** — `UK_KS2`
- `T.II.7.002` **Rounding money to nearest pound/penny** — `UK_KS2`
- `T.II.7.003` **Decimal ordering to 3 d.p. exam drills** — `UK_KS2`
- `T.II.7.004` **Multiply/divide decimals by 10/100/1000** — `UK_KS2`
- `T.II.7.005` **Thousandths place value (Y5–6)** — `UK_KS2`
- `T.II.7.006` **Decimal × whole number money contexts** — `UK_KS2`
- `T.II.7.007` **Decimal problems in measure contexts** — `UK_KS2`

#### `II.8` Expressions (5)

- `T.II.8.001` **Simple formulae in words then letters (Y6)** — `UK_KS2`
- `T.II.8.002` **Find pairs of numbers satisfying an equation** — `UK_KS2`
- `T.II.8.003` **Generate and describe linear sequences (Y6)** — `UK_KS2,UK_KS3`
- `T.II.8.004` **Use simple ratio language (Y6)** — `UK_KS2`
- `T.II.8.005` **Enumerate possibilities systematically (Y6)** — `UK_KS2` · challenge

#### `II.9` Measurement & geometry (25)

- `T.II.9.001` **Imperial ↔ metric approximate equivalences** — `UK_KS2`
- `T.II.9.002` **Convert between metric units fluently** — `UK_KS2`
- `T.II.9.003` **Area and perimeter of rectilinear shapes** — `UK_KS2`
- `T.II.9.004` **Volume of cubes and cuboids (cm³)** — `UK_KS2`
- `T.II.9.005` **Estimate angles; classify acute/obtuse/reflex** — `UK_KS2`
- `T.II.9.006` **Draw and measure angles to nearest degree** — `UK_KS2`
- `T.II.9.007` **Translation parallel to axes only (Y5 constraint)** — `UK_KS2` · ⚙geometry
- `T.II.9.008` **Reflection in lines parallel to axes** — `UK_KS2` · ⚙geometry
- `T.II.9.009` **Coordinates in first quadrant plot & read** — `UK_KS2`
- `T.II.9.010` **Four-quadrant coordinates intro (Y6)** — `UK_KS2`
- `T.II.9.011` **Missing angles on a straight line / at a point** — `UK_KS2`
- `T.II.9.012` **Properties of regular polygons (sides/angles)** — `UK_KS2,UK_KS3` · challenge
- `T.II.9.013` **Net of cubes and cuboids recognition** — `UK_KS2` · ⚙geometry
- `T.II.9.014` **Identify 3D faces, edges, vertices** — `UK_KS2`
- `T.II.9.015` **Area of triangles by counting half-squares** — `UK_KS2`
- `T.II.9.016` **Scale factor enlarge by integer (Y6)** — `UK_KS2` · ⚙geometry
- `T.II.9.017` **Perimeter of polygons with missing sides** — `UK_KS2` · challenge
- `T.II.9.018` **Draw circles with compass; label radius/diameter** — `UK_KS2` · ⚙geometry
- `T.II.9.019` **Time duration worded crossing midnight** — `UK_KS2` · challenge
- `T.II.9.020` **Convert hours–minutes–seconds** — `UK_KS2`
- `T.II.9.021` **Find missing angle in triangle (Y6)** — `UK_KS2`
- `T.II.9.022` **Imperial-metric estimation set 1** — `UK_KS2`
- `T.II.9.023` **Axis-parallel transform drill 1** — `UK_KS2` · ⚙geometry
- `T.II.9.024` **Imperial-metric estimation set 2** — `UK_KS2`
- `T.II.9.025` **Axis-parallel transform drill 2** — `UK_KS2` · ⚙geometry

#### `II.10` Data (10)

- `T.II.10.001` **Pie charts: interpret simple sectors (Y6)** — `UK_KS2`
- `T.II.10.002` **Calculate the mean (Y6 statutory)** — `UK_KS2`
- `T.II.10.003` **Line graphs: interpret dual scales carefully** — `UK_KS2` · challenge
- `T.II.10.004` **Timetables and dual bar charts combined** — `UK_KS2` · challenge
- `T.II.10.005` **CCSS measurement data displays pack** — `US_CCSS_K5,UK_KS2`
- `T.II.10.006` **Mode and range early (UK secondary bridge)** — `UK_KS2,UK_KS3`
- `T.II.10.007` **Interpret misleading graphs critically** — `UK_KS2,US_CCSS_68` · strange
- `T.II.10.008` **Dual bar charts compare categories** — `UK_KS2`
- `T.II.10.009` **Pie chart and mean combo 1** — `UK_KS2` · challenge
- `T.II.10.010` **Pie chart and mean combo 2** — `UK_KS2` · challenge

### Era III — Relate

#### `III.1` Integers & rationals (21)

- `T.III.1.001` **Standard form A×10ⁿ introduction (KS3)** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F`
- `T.III.1.002` **Convert ordinary ↔ standard form fluency** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.003` **Order numbers in standard form** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.004` **Calculate with standard form (non-calc)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.1.005` **Standard form with calculator (GCSE)** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_AA_SL,IB_AI_SL` · ⚙gdc
- `T.III.1.006` **Negative numbers in financial contexts** — `UK_KS3,IB_MYP,US_CCSS_68`
- `T.III.1.007` **Recurring decimal notation (dot notation UK)** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.008` **Convert recurring decimals to fractions** — `UK_GCSE_H` · challenge
- `T.III.1.009` **Absolute value equations simple (KS3)** — `UK_KS3,IB_MYP,US_CCSS_68`
- `T.III.1.010` **Error intervals from rounded values intro** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.011` **Upper and lower bounds of rounded measurements** — `UK_GCSE_H`
- `T.III.1.012` **Bounds in calculations (sum/product/quotient)** — `UK_GCSE_H` · challenge
- `T.III.1.013` **Limits of accuracy wording exam pack** — `UK_GCSE_H`
- `T.III.1.014` **Bounds to 1 d.p. from truncated measurements** — `UK_GCSE_H` · challenge
- `T.III.1.015` **Error intervals for continuous measures** — `UK_GCSE_H`
- `T.III.1.016` **Bounds: upper and lower for truncated data** — `UK_GCSE_H` · challenge
- `T.III.1.017` **Calculator vs non-calculator standard form** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙gdc
- `T.III.1.018` **Standard form applied science context 1** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.019` **Standard form applied science context 2** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.020` **Standard form applied science context 3** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.1.021` **Bounds of a calculated perimeter/area** — `UK_GCSE_H` · challenge

#### `III.2` Ratios & rates (25)

- `T.III.2.001` **Compound measure: speed (m/s and km/h)** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.2.002` **Compound measure: density (mass÷volume)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.III.2.003` **Compound measure: pressure** — `UK_GCSE_H`
- `T.III.2.004` **Rates of pay and unit pricing** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.2.005` **Currency conversion with exchange rates** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_MYP`
- `T.III.2.006` **Map scales as ratios (1:n)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_KS3,IB_MYP,US_CCSS_68`
- `T.III.2.007` **Sharing in a ratio three-part** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.2.008` **Ratio given difference or total variants** — `UK_GCSE_H` · challenge
- `T.III.2.009` **Direct proportion graphs through origin** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.2.010` **Inverse proportion intro (xy=k)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_MYP`
- `T.III.2.011` **Speed–distance–time with unit changes** — `UK_GCSE_F,UK_KS3,IB_MYP` · challenge
- `T.III.2.012` **Population density and area ratios** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_AI_SL,IB_AI_HL`
- `T.III.2.013` **Recipe scaling and mixture ratios** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.2.014` **CCSS RP: tape diagrams for percent/ratio** — `US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.2.015` **CCSS RP: percent as ratio of part to whole** — `US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.2.016` **Mixing problems with ratios** — `UK_GCSE_H` · challenge
- `T.III.2.017` **Scale drawings measure and interpret** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.2.018` **Proportion word problems multi-step** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP` · challenge
- `T.III.2.019` **Average speed for multi-leg journeys** — `UK_GCSE_H` · challenge
- `T.III.2.020` **Convert compound units step by step** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.2.021` **Compound measures mixed drill 1** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.2.022` **Compound measures mixed drill 2** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.2.023` **Compound measures mixed drill 3** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.2.024` **Compound measures mixed drill 4** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.2.025` **Compound measures mixed drill 5** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge

#### `III.3` Percent (22)

- `T.III.3.001` **Find original value after % change (reverse %)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.III.3.002` **Simple interest exam pack (I=PRT/100)** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.003` **Compound interest (non-calc appreciation)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL` · challenge
- `T.III.3.004` **Compound interest depreciation / decay** — `UK_GCSE_H`
- `T.III.3.005` **VAT and sales tax multi-step** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.006` **Hire purchase and interest comparisons** — `UK_GCSE_F,UK_KS3,IB_MYP` · challenge
- `T.III.3.007` **Successive percentage changes (not additive)** — `UK_GCSE_H` · challenge
- `T.III.3.008` **Express one quantity as % of another** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.009` **Percentage profit and loss** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.010` **Repeated percentage growth GDC workflow** — `IB_AI_SL,IB_AI_HL,IB_AI_HL` · ⚙gdc
- `T.III.3.011` **Bank statements and balance tracking** — `UK_KS3,IB_MYP,US_CCSS_68,UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.012` **Best-buy percentage vs absolute saving** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.013` **Percentage multipliers one-step fluency** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.3.014` **Find % when given two related quantities** — `UK_GCSE_H` · challenge
- `T.III.3.015` **Inflation and real-terms value (simple)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · challenge
- `T.III.3.016` **Express changes using percentage multipliers chain** — `UK_GCSE_H` · challenge
- `T.III.3.017` **Financial % multi-step scenario 1** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H` · challenge
- `T.III.3.018` **Financial % multi-step scenario 2** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H` · challenge
- `T.III.3.019` **Financial % multi-step scenario 3** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H` · challenge
- `T.III.3.020` **Financial % multi-step scenario 4** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H` · challenge
- `T.III.3.021` **Financial % multi-step scenario 5** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H` · challenge
- `T.III.3.022` **Reverse percentage after successive changes** — `UK_GCSE_H` · challenge

#### `III.4` Exponents & roots (11)

- `T.III.4.001` **Laws of indices exam pack (integer)** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_MYP`
- `T.III.4.002` **Fractional indices as roots** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.III.4.003` **Negative and fractional indices combined** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.III.4.004` **Surds: simplify √(ab) and √(a/b)** — `UK_GCSE_H`
- `T.III.4.005` **Surds: expand and simplify (a+√b)(c+√d)** — `UK_GCSE_H` · challenge
- `T.III.4.006` **Rationalise denominators (monomial and binomial)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.III.4.007` **Scientific notation vs UK standard form wording** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.4.008` **Estimate powers and roots without calc** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.4.009` **Zero and negative indices meaning pack** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.4.010` **Work in standard form then convert back** — `UK_GCSE_H` · challenge
- `T.III.4.011` **Evaluate with fractional/negative indices non-calc** — `UK_GCSE_H` · challenge

#### `III.5` Expressions (11)

- `T.III.5.001` **Expand single and double brackets exam pack** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_MYP`
- `T.III.5.002` **Factorise linear expressions fully** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.5.003` **Factorise quadratics a=1 exam pack** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.III.5.004` **Factorise difference of two squares** — `UK_GCSE_H`
- `T.III.5.005` **Algebraic fractions simplify (linear)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.III.5.006` **Write expressions from worded contexts** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.5.007` **Identities vs equations recognition** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.III.5.008` **Collect like terms with multiple variables** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.5.009` **Substitution including negatives and powers** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.5.010` **Expand three binomials (Higher)** — `UK_GCSE_H` · challenge
- `T.III.5.011` **Factorise by grouping (four terms)** — `UK_GCSE_H` · challenge

#### `III.6` Equations & inequalities (11)

- `T.III.6.001` **Solve linear equations with fractions** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.002` **Form and solve equations from geometry** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.003` **Inequalities on number lines (UK open/closed)** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.004` **Solve linear inequalities and list integers** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.005` **Simultaneous equations elimination (KS3/4)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.III.6.006` **Simultaneous equations substitution** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.007` **Graphical solution of simultaneous equations** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙desmos
- `T.III.6.008` **Equations with unknown on both sides** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.009` **Inequalities with negative coefficients** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.6.010` **Quadratic inequalities intro via graphs** — `UK_GCSE_H` · ⚙desmos · challenge
- `T.III.6.011` **Trial and improvement (legacy dialect)** — `UK_GCSE_H` · strange

#### `III.7` Lines & first functions (11)

- `T.III.7.001` **Gradient from coordinates (UK wording)** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.7.002` **Equation of a line y=mx+c fluency** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_MYP`
- `T.III.7.003` **Parallel and perpendicular gradients** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.III.7.004` **Midpoint and length of a line segment** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.7.005` **Real graphs: conversion and distance–time** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙graph
- `T.III.7.006` **Speed from distance–time graph gradients** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙graph
- `T.III.7.007` **Instantaneous rate of change on a curve (KS4 tease)** — `UK_GCSE_H` · ⚙desmos · challenge
- `T.III.7.008` **Find equation of parallel line through a point** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.7.009` **Interpret intercepts in context** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙graph
- `T.III.7.010` **Solve linear equations graphically on Desmos** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_AA_SL,IB_AI_SL` · ⚙desmos
- `T.III.7.011` **Find intercepts algebraically and graphically** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙desmos

#### `III.8` Basic Non-Proof Geometry (29)

- `T.III.8.001` **Plans and elevations of 3D shapes** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.III.8.002` **Nets of pyramids, prisms, cylinders** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.003` **Bearings intro: three-figure bearings** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.8.004` **Construct triangles given SSS/SAS/ASA** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.8.005` **Loci: set of points equidistant** — `UK_GCSE_H` · ⚙geometry
- `T.III.8.006` **Loci: regions satisfying inequalities** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.III.8.007` **Pythagoras exam worded (2D)** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.008` **Pythagoras in 3D (space diagonal)** — `UK_GCSE_H` · challenge
- `T.III.8.009` **Circle area/circumference exact answers in π** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.010` **Arc length and sector area (GCSE)** — `UK_GCSE_H`
- `T.III.8.011` **Volume/surface area formula selection pack** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.012` **Similar shapes length/area/volume scale factors** — `UK_GCSE_H` · challenge
- `T.III.8.013` **Congruence conditions SSS SAS ASA RHS** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.III.8.014` **Enlargement with fractional and negative SF** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.III.8.015` **Describe transformations fully (GCSE language)** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.016` **Interior/exterior angles of polygons exam** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.017` **Tessellation angle conditions** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry · strange
- `T.III.8.018` **Surface area of cylinders exact and decimal** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.019` **Exact trig values preview: 30–60–90 links** — `UK_GCSE_H`
- `T.III.8.020` **Isometric drawing of 3D shapes** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.8.021` **Exact answers leave in terms of π pack** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.8.022` **Surface area of spheres leave in π** — `UK_GCSE_H`
- `T.III.8.023` **Voronoi diagrams nearest-site partitioning** — `IB_AI_HL` · ⚙geometry · strange · uncertain
- `T.III.8.024` **Voronoi applications: services catchment** — `IB_AI_HL` · strange · uncertain
- `T.III.8.025` **Graph theory: walks trails paths cycles (light)** — `IB_AI_HL` · strange · uncertain
- `T.III.8.026` **Shortest path / Chinese Postman light** — `IB_AI_HL` · strange · uncertain
- `T.III.8.027` **Plans elevations practice figure 1** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.8.028` **Plans elevations practice figure 2** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.III.8.029` **Plans elevations practice figure 3** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry

#### `III.9` Statistics & probability (35)

- `T.III.9.001` **Venn diagrams for probability (two sets)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_MYP`
- `T.III.9.002` **Venn diagrams three sets** — `UK_GCSE_H` · challenge
- `T.III.9.003` **Frequency trees for probability** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.004` **Histograms with unequal class widths** — `UK_GCSE_H` · challenge
- `T.III.9.005` **Cumulative frequency curves and medians** — `UK_GCSE_H` · ⚙graph
- `T.III.9.006` **Box plots from CF and compare distributions** — `UK_GCSE_H`
- `T.III.9.007` **Product rule for counting (KS4 Higher)** — `UK_GCSE_H`
- `T.III.9.008` **Sample space diagrams for two events** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.009` **Relative frequency vs theoretical probability** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.9.010` **Capture–recapture estimation (UK contexts)** — `UK_GCSE_H` · strange
- `T.III.9.011` **Stratified sampling calculations** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.012` **Two-way tables probability conditional** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.013` **Pie chart construction from data** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.014` **Moving averages (time series intro)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · challenge
- `T.III.9.015` **CCSS SP: chance device simulations middle school** — `US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.9.016` **CCSS SP: bivariate categorical associations** — `US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.9.017` **Mean from frequency table (estimated)** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.018` **Modal class and median class from grouped data** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.019` **Probability scale 0 to 1 language** — `UK_KS3,IB_MYP,US_CCSS_68`
- `T.III.9.020` **Expectation from theoretical probability** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.021` **AP Stats: describing distributions SOCS** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.022` **AP Stats: comparing dual boxplots FRQ** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.023` **IB AI: boxplots and outliers 1.5×IQR rule** — `IB_AI_SL,IB_AI_HL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.024` **Misleading scales and truncated axes critique** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_68,UK_KS3,IB_MYP,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.III.9.025` **Cumulative frequency ↔ box plot pipeline** — `UK_GCSE_H` · ⚙graph
- `T.III.9.026` **Experimental probability long-run estimate** — `UK_KS3,IB_MYP,US_CCSS_68,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.9.027` **Questionnaire bias and leading questions** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_KS3,IB_MYP,US_CCSS_68`
- `T.III.9.028` **Frequency polygon from histogram** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙graph
- `T.III.9.029` **Pie chart angle calculation exam** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.030` **Combine probabilities mutually exclusive lists** — `UK_GCSE_F,UK_KS3,IB_MYP`
- `T.III.9.031` **Sampling variability dotplot intuition** — `AP_STATS,IB_AI_HL,IB_AI_SL,US_CCSS_68,UK_KS3,IB_MYP`
- `T.III.9.032` **Venn probability exam set 1** — `UK_GCSE_H`
- `T.III.9.033` **Venn probability exam set 2** — `UK_GCSE_H`
- `T.III.9.034` **Venn probability exam set 3** — `UK_GCSE_H`
- `T.III.9.035` **Histogram unequal width frequency density set** — `UK_GCSE_H` · challenge

### Era IV — Solve

#### `IV.1` Equations & inequalities (4)

- `T.IV.1.001` **Inequalities regions on graphs (linear)** — `UK_GCSE_H` · ⚙desmos
- `T.IV.1.002` **Set notation for solution sets (UK)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.1.003` **Exact vs approximate solutions language** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.1.004` **Inequalities with fractions clear carefully** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge

#### `IV.2` Functions (13)

- `T.IV.2.001` **Function notation f(x) exam fluency** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.IV.2.002` **Domain and range from graphs and equations** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos
- `T.IV.2.003` **Composite functions fog and gof** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.2.004` **Inverse functions algebraically** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.2.005` **Piecewise functions interpret and graph** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_HL` · ⚙desmos
- `T.IV.2.006` **Transformations of graphs y=f(x) exam pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.IV.2.007` **Modulus function graphs and equations** — `UK_GCSE_H,IB_AA_HL` · ⚙desmos · challenge
- `T.IV.2.008` **Vertical line test and function definition exam** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AI_SL` · ⚙desmos
- `T.IV.2.009` **1–1 and onto language for inverses** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · challenge
- `T.IV.2.010` **Parametric definition of functions intro** — `IB_AA_SL,IB_AA_HL,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.IV.2.011` **Self-inverse functions recognition** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.IV.2.012` **Restrict domain to make inverse** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos · challenge
- `T.IV.2.013` **Function arithmetic (sum product quotient)** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos

#### `IV.3` Linear functions (5)

- `T.IV.3.001` **Perpendicular bisector equation** — `UK_GCSE_H`
- `T.IV.3.002` **Distance from point to line formula use** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.3.003` **Equation of circle centre origin + tangent (GCSE H)** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.IV.3.004` **Equation of circle general; find centre/radius** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.IV.3.005` **Find intersection of two circles algebraically** — `UK_GCSE_H,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · challenge

#### `IV.4` Systems (6)

- `T.IV.4.001` **Simultaneous three equations intro** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · challenge
- `T.IV.4.002` **Non-linear simultaneous exam pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.4.003` **Matrices 2×2 multiply and inverse (GCSE+)** — `UK_GCSE_H,IB_AA_HL,IB_AI_HL,US_CCSS_HS` · challenge
- `T.IV.4.004` **Matrix transformations of the plane intro** — `IB_AI_HL,IB_AA_HL,US_CCSS_HS` · ⚙geometry · challenge
- `T.IV.4.005` **Graphical linear programming light (regions)** — `IB_AI_HL,UK_GCSE_H` · ⚙desmos · strange
- `T.IV.4.006` **Determinant condition for unique solution 2×2** — `UK_GCSE_H,IB_AA_HL,US_CCSS_HS`

#### `IV.5` Exponents & radicals (13)

- `T.IV.5.001` **Surds GCSE Higher full toolkit pack** — `UK_GCSE_H` · challenge
- `T.IV.5.002` **Rationalise two-term denominators under time** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.5.003` **Surds in exact geometric answers** — `UK_GCSE_H`
- `T.IV.5.004` **Fractional indices ↔ radical form conversions** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.5.005` **Solve equations with fractional indices** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_HL` · challenge
- `T.IV.5.006` **Nested radicals simplify (strange)** — `UK_GCSE_H,IB_AA_HL` · strange
- `T.IV.5.007` **Simplify expressions with mixed surds and indices** — `UK_GCSE_H` · challenge
- `T.IV.5.008` **Rationalise with conjugate under radicals** — `UK_GCSE_H` · challenge
- `T.IV.5.009` **Surds non-calc paper segment 1** — `UK_GCSE_H` · challenge
- `T.IV.5.010` **Surds non-calc paper segment 2** — `UK_GCSE_H` · challenge
- `T.IV.5.011` **Surds non-calc paper segment 3** — `UK_GCSE_H` · challenge
- `T.IV.5.012` **Surds in exact trig non-calc hybrids** — `UK_GCSE_H` · challenge
- `T.IV.5.013` **Index equations leading to quadratics** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge

#### `IV.6` Polynomials (10)

- `T.IV.6.001` **Factor theorem exam use** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.6.002` **Remainder theorem exam use** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.6.003` **Algebraic division of cubics** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.6.004` **Sketch cubic and quartic from factorised form** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.IV.6.005` **Expand and factorise mixed higher exam set** — `UK_GCSE_H`
- `T.IV.6.006` **Binomial expansion positive integer n** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.6.007` **Binomial approximation (1+x)^n for small x** — `IB_AA_HL,UK_GCSE_H` · challenge
- `T.IV.6.008` **Sketch from leading term and roots only** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.IV.6.009` **Factorise cubics fully after one root** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.6.010` **Polynomial division with remainders interpreted** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`

#### `IV.7` Quadratics (27)

- `T.IV.7.001` **Completing the square exam method pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.7.002` **Turning points via completing the square** — `UK_GCSE_H`
- `T.IV.7.003` **Sketch quadratics from completed square** — `UK_GCSE_H` · ⚙desmos
- `T.IV.7.004` **Quadratic formula exact surd answers** — `UK_GCSE_H`
- `T.IV.7.005` **Discriminant: number of roots exam stems** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.7.006` **Form quadratic equations from roots/context** — `UK_GCSE_H`
- `T.IV.7.007` **Quadratic simultaneous with linear** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.7.008` **Iteration: rearrange to x=g(x) form** — `UK_GCSE_H`
- `T.IV.7.009` **Iteration: show a root lies in an interval** — `UK_GCSE_H`
- `T.IV.7.010` **Iteration: perform and interpret convergence** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙gdc · challenge
- `T.IV.7.011` **Quadratic inequalities critical values method** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.7.012` **Projectile worded GCSE/IB pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.7.013` **Hidden quadratics (exp/trig substitutions)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.7.014` **Quadratic model fitting with GDC** — `IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.7.015` **Sign-change decimal search before iteration** — `UK_GCSE_H`
- `T.IV.7.016` **Intersecting chord/quadratic geometry link** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.IV.7.017` **Completing square exam battery 1** — `UK_GCSE_H` · challenge
- `T.IV.7.018` **Completing square exam battery 2** — `UK_GCSE_H` · challenge
- `T.IV.7.019` **Completing square exam battery 3** — `UK_GCSE_H` · challenge
- `T.IV.7.020` **Completing square exam battery 4** — `UK_GCSE_H` · challenge
- `T.IV.7.021` **Iteration numerical table 1** — `UK_GCSE_H` · ⚙gdc
- `T.IV.7.022` **Iteration numerical table 2** — `UK_GCSE_H` · ⚙gdc
- `T.IV.7.023` **Iteration numerical table 3** — `UK_GCSE_H` · ⚙gdc
- `T.IV.7.024` **Completing square with a≠1 fluency** — `UK_GCSE_H` · challenge
- `T.IV.7.025` **Iteration: cobweb diagram interpretation** — `UK_GCSE_H` · ⚙desmos · strange
- `T.IV.7.026` **Quadratic inequalities on number line shading** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.7.027` **Worded optimisation without calculus (complete square)** — `UK_GCSE_H` · challenge

#### `IV.8` Complex numbers (6)

- `T.IV.8.001` **Argand diagram exam plotting** — `IB_AA_HL,IB_AA_SL` · ⚙geometry
- `T.IV.8.002` **Modulus-argument form conversions** — `IB_AA_HL`
- `T.IV.8.003` **De Moivre exam applications** — `IB_AA_HL` · challenge
- `T.IV.8.004` **Complex loci |z−a|=r and arg(z−a)=θ** — `IB_AA_HL` · challenge · uncertain
- `T.IV.8.005` **Solve equations in complex numbers** — `IB_AA_HL` · challenge
- `T.IV.8.006` **Powers of i cycle fluency** — `IB_AA_HL,IB_AA_SL`

#### `IV.9` Function toolkit (7)

- `T.IV.9.001` **Even/odd functions recognition** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.9.002` **Absolute value inequalities** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.9.003` **Asymptotes of rational functions exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos
- `T.IV.9.004` **Combined transformations order matters** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos · challenge
- `T.IV.9.005` **Step functions and floor in modelling (light)** — `IB_AI_SL,IB_AI_HL` · ⚙desmos · strange
- `T.IV.9.006` **Oblique asymptotes by division** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_HL` · ⚙desmos · challenge
- `T.IV.9.007` **Graph y=1/f(x) from y=f(x) features** — `UK_GCSE_H,IB_AA_SL,IB_AA_HL` · ⚙desmos · challenge

#### `IV.10` Polynomial functions (1)

- `T.IV.10.001` **Polynomial inequalities on number line** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL`

#### `IV.11` Rational & radical functions (4)

- `T.IV.11.001` **Solve rational equations check extraneous** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.IV.11.002` **Radical equations isolate and check** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.11.003` **Graphical solution of radical/rational eqs** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AI_SL` · ⚙desmos
- `T.IV.11.004` **Domain of radical and rational combined** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`

#### `IV.12` Exponential & logarithmic (18)

- `T.IV.12.001` **Compound interest continuous (A=Pe^{rt})** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.IV.12.002` **GCSE growth and decay worded pack** — `UK_GCSE_H`
- `T.IV.12.003` **IB GDC exponential regression workflow** — `IB_AI_SL,IB_AI_HL,IB_AA_SL,IB_AI_SL` · ⚙gdc
- `T.IV.12.004` **Log scales interpretation** — `IB_AI_SL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙graph
- `T.IV.12.005` **Solve exp/log equations exam mixed pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.12.006` **Change of base in exam calculations** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙gdc
- `T.IV.12.007` **Half-life multi-step worded** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · challenge
- `T.IV.12.008` **Modelling cycle: formulate–solve–interpret–evaluate** — `IB_AI_SL,IB_AI_HL,IB_AI_HL` · challenge
- `T.IV.12.009` **Compare linear vs exponential models** — `IB_AI_SL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙gdc · challenge
- `T.IV.12.010` **Logarithmic linearisation of data** — `IB_AI_SL,IB_AI_HL,IB_AI_HL` · ⚙gdc · challenge
- `T.IV.12.011` **Newton's law of cooling discrete steps** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · challenge
- `T.IV.12.012` **Effective annual rate vs nominal** — `IB_AI_SL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · challenge
- `T.IV.12.013` **Exp/log modelling context 1** — `IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙gdc · challenge
- `T.IV.12.014` **Exp/log modelling context 2** — `IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙gdc · challenge
- `T.IV.12.015` **Exp/log modelling context 3** — `IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙gdc · challenge
- `T.IV.12.016` **Compound interest vs simple interest compare** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.12.017` **Solve for time in exponential models** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.IV.12.018` **Doubling time from continuous and discrete models** — `IB_AI_SL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · challenge

#### `IV.13` Sequences & series (21)

- `T.IV.13.001` **nth term of linear sequences (GCSE)** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.13.002` **Quadratic sequences nth term** — `UK_GCSE_H` · challenge
- `T.IV.13.003` **Geometric sequences GCSE/IB worded** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.IV.13.004` **Arithmetic series exam applications** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.13.005` **Infinite geometric series |r|<1 condition** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.13.006` **Sigma notation exam fluency** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.13.007` **Recurrence relations xₙ₊₁=axₙ+b** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.13.008` **Fibonacci-type sequences properties** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_MYP` · strange
- `T.IV.13.009` **Sequences modelling IB AI contexts** — `IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.13.010` **Prove a sequence is arithmetic/geometric** — `IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.13.011` **Financial series: annuities simple** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · challenge
- `T.IV.13.012` **IB AA HL induction on sequences preview** — `IB_AA_HL` · challenge
- `T.IV.13.013` **Compare arithmetic vs geometric growth stories** — `IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.13.014` **Sequences GCSE mixed paper 1** — `UK_GCSE_H` · challenge
- `T.IV.13.015` **Sequences GCSE mixed paper 2** — `UK_GCSE_H` · challenge
- `T.IV.13.016` **Sequences GCSE mixed paper 3** — `UK_GCSE_H` · challenge
- `T.IV.13.017` **Sequences GCSE mixed paper 4** — `UK_GCSE_H` · challenge
- `T.IV.13.018` **nth term from practical sequences contexts** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.13.019` **Sum of first n naturals / odds identities** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.IV.13.020` **Geometric series in repeating decimals link** — `UK_GCSE_H,IB_AA_SL,IB_AA_HL`
- `T.IV.13.021` **GCSE Higher special sequences (triangular)** — `UK_GCSE_H` · strange

#### `IV.14` Counting & probability (22)

- `T.IV.14.001` **Product rule and permutations exam pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.14.002` **Combinations in probability contexts** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.14.003` **Conditional probability tree diagrams (GCSE H)** — `UK_GCSE_H`
- `T.IV.14.004` **Independent vs mutually exclusive exam traps** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.IV.14.005` **Venn ↔ tree ↔ two-way translation** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL` · challenge
- `T.IV.14.006` **Expected value decision problems (S-MD)** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.14.007` **Bayes with medical/test contexts** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL` · challenge
- `T.IV.14.008` **Inclusive exclusive counting with Venn** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.14.009` **Conditional probability given complementary info** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.010` **At least one complement strategy pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.14.011` **Law of large numbers simulation demo** — `AP_STATS,IB_AI_HL,IB_AI_SL,US_CCSS_68,UK_KS3,IB_MYP`
- `T.IV.14.012` **Rare event rule intuition** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.14.013` **Expected value of games fair/unfair** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.14.014` **Conditional probability medical screening FRQ** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.015` ** mutually exclusive addition rule drills** — `UK_GCSE_F,UK_KS3,IB_MYP,AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.14.016` **Tree diagrams with three stages** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.017` **Conditional probability FRQ-style 1** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.018` **Conditional probability FRQ-style 2** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.019` **Conditional probability FRQ-style 3** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.020` **Conditional probability given restricted sample space** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.14.021` **Counting with restrictions (no two adjacent)** — `UK_GCSE_H,IB_AA_SL,IB_AA_HL` · challenge
- `T.IV.14.022` **Probability with without replacement trees** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_STATS,IB_AI_HL,IB_AI_SL`

#### `IV.15` Data & distributions (24)

- `T.IV.15.001` **Normal distribution empirical rule exam** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.002` **z-score calculations and interpretation** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.003` **Binomial probability GDC workflow** — `IB_AI_SL,IB_AI_HL,AP_STATS,IB_AI_HL,IB_AI_SL,IB_AA_SL` · ⚙gdc
- `T.IV.15.004` **Scatter plots: describe strength/direction/form** — `AP_STATS,IB_AI_HL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.IV.15.005` **Correlation vs causation exam stems** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.IV.15.006` **Least-squares residual interpretation** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.15.007` **Outliers effect on mean/median/regression** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.15.008` **Comparing distributions with multiple measures** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.15.009` **Percentiles and cumulative relative frequency** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.15.010` **Skew interpretation from histograms/boxplots** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.15.011` **Binomial vs geometric settings recognition** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.012` **Geometric distribution probability** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.013` **Normal probability GDC invNorm/normalcdf** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.15.014` **Assessing normality: plots and rules** — `AP_STATS,IB_AI_HL,IB_AI_SL` · ⚙gdc
- `T.IV.15.015` **Transforming data: effect on mean/SD** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.IV.15.016` **Residual plots: pattern means non-linear** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.15.017` **Combining random variables mean/variance** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.IV.15.018` **Linear regression prediction vs extrapolation** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.IV.15.019` **Discrete RV probability distribution tables** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.020` **Inverse normal cut-points for percentiles** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.IV.15.021` **Effect of coding data (subtract/divide)** — `AP_STATS,IB_AI_HL,IB_AI_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.IV.15.022` **Empirical rule vs Chebyshev light contrast** — `AP_STATS,IB_AI_HL,IB_AI_SL` · strange
- `T.IV.15.023` **Binomial mean np and SD √(npq) fluency** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.IV.15.024` **Lurking variables in observational studies** — `AP_STATS,IB_AI_HL,IB_AI_SL`

### Era V — Prove

#### `V.1` Logic & proof (7)

- `T.V.1.001` **GCSE Higher geometric proof write-ups** — `UK_GCSE_H` · challenge
- `T.V.1.002` **Proof by induction AA HL staple pack** — `IB_AA_HL` · challenge
- `T.V.1.003` **Induction: inequalities and sequences** — `IB_AA_HL` · challenge
- `T.V.1.004` **Counterexample hunting exam style** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.1.005` **Two-column congruence proof drills** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.1.006` **IB exploration mini-write structure** — `IB_MYP,IB_AA_SL,IB_AA_HL,IB_AI_SL,IB_AI_HL` · strange
- `T.V.1.007` **Indirect proof (contradiction) geometry classic** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge

#### `V.2` Lines & angles (2)

- `T.V.2.001` **Parallel line angle chase exam pack** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.2.002` **Prove corresponding/alternate equal** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`

#### `V.3` Triangles (5)

- `T.V.3.001` **Congruence proof multi-step GCSE/US** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.3.002` **Isosceles triangle theorem proofs** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.3.003` **Points of concurrency justification pack** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.3.004` **Exterior angle of triangle proof applications** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry
- `T.V.3.005` **CPCTC in multi-triangle proofs** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge

#### `V.4` Polygons (3)

- `T.V.4.001` **Interior angle sum proof for polygons** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.4.002` **Regular polygon exterior angle proofs** — `UK_GCSE_H`
- `T.V.4.003` **Tessellation and interior angle conditions proof** — `UK_GCSE_H` · ⚙geometry · strange

#### `V.5` Similarity (6)

- `T.V.5.001` **Similar triangles exam multi-step** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AI_SL`
- `T.V.5.002` **AA/SSS/SAS similarity justification** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.5.003` **Area ratios of similar shapes exam** — `UK_GCSE_H` · challenge
- `T.V.5.004` **Intercept theorems (basic proportionality)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.V.5.005` **Shadow and mirror similar-triangle measurement** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry
- `T.V.5.006` **Parallel lines ⇒ similar triangles patterns** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry

#### `V.6` Right-triangle trig (32)

- `T.V.6.001` **Exact trig values 0°,30°,45°,60°,90° pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.6.002` **Exact value multi-step without calculator** — `UK_GCSE_H` · challenge
- `T.V.6.003` **Angle of elevation multi-step exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.V.6.004` **Angle of depression with bearings mix** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.6.005` **SOHCAHTOA worded GCSE Foundation/Higher** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.6.006` **Find sides with reciprocal ratios** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.V.6.007` **Trig in isosceles / split base techniques** — `UK_GCSE_H`
- `T.V.6.008` **3D trigonometry: angle between line and plane** — `UK_GCSE_H,IB_AA_SL` · ⚙geometry · strange
- `T.V.6.009` **3D trigonometry: angle between two planes** — `UK_GCSE_H,IB_AA_HL` · ⚙geometry · strange
- `T.V.6.010` **3D Pythagoras + trig combined** — `UK_GCSE_H` · challenge
- `T.V.6.011` **Right-trig calculator vs exact decision** — `UK_GCSE_H`
- `T.V.6.012` **Inverse trig range awareness (principal values)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.6.013` **Clinometer / practical elevation contexts** — `UK_GCSE_F,UK_KS3,IB_MYP,IB_MYP` · ⚙geometry
- `T.V.6.014` **Trig ratios as slopes and unit rates** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.6.015` **Exact tan 30/45/60 without calculator** — `UK_GCSE_H`
- `T.V.6.016` **Two-triangle elevation problems** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.6.017` **Bearing and distance from trig in right Δ** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.V.6.018` **Trigonometric ratios of complementary angles** — `UK_GCSE_H`
- `T.V.6.019` **Exact values for related angles 120°,135°,150°** — `UK_GCSE_H` · ⚙unit_circle
- `T.V.6.020` **Slope angle of a roof / ramp accessibility** — `UK_GCSE_F,UK_KS3,IB_MYP,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.6.021` **Trigonometry non-calc paper strategies** — `UK_GCSE_H`
- `T.V.6.022` **Double triangle ladder against wall classic** — `UK_GCSE_H` · ⚙geometry
- `T.V.6.023` **Trigonometry in non-right by dropping altitude** — `UK_GCSE_H` · ⚙geometry
- `T.V.6.024` **Inclination of a line from tanθ = m** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.6.025` **Exact values application set 1** — `UK_GCSE_H`
- `T.V.6.026` **Exact values application set 2** — `UK_GCSE_H`
- `T.V.6.027` **Exact values application set 3** — `UK_GCSE_H`
- `T.V.6.028` **Exact values application set 4** — `UK_GCSE_H`
- `T.V.6.029` **3D trig optional challenge 1** — `UK_GCSE_H,IB_AA_SL` · ⚙geometry · strange
- `T.V.6.030` **3D trig optional challenge 2** — `UK_GCSE_H,IB_AA_SL` · ⚙geometry · strange
- `T.V.6.031` **3D trig optional challenge 3** — `UK_GCSE_H,IB_AA_SL` · ⚙geometry · strange
- `T.V.6.032` **Exact values memory palace exam warm-up** — `UK_GCSE_H`

#### `V.7` General triangles (23)

- `T.V.7.001` **Bearings: three-figure notation drills** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.V.7.002` **Bearings: reverse bearings (+180° rule)** — `UK_GCSE_H` · ⚙geometry
- `T.V.7.003` **Bearings: multi-leg route problems** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.004` **Bearings: exam worded navigation Qs** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.005` **Bearings with cosine/sine rule** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.006` **Law of sines ambiguous case SSA deep pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · challenge
- `T.V.7.007` **Law of cosines rearrange for angles** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.V.7.008` **Area ½ab sin C exam pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.V.7.009` **Heron vs sine-area method choice** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.V.7.010` **Surveying triangulation exam contexts** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.V.7.011` **Solve any triangle mixed timed set** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.7.012` **Area of triangle given SAS multi-step** — `UK_GCSE_H`
- `T.V.7.013` **Obtuse triangles cosine rule careful signs** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL` · challenge
- `T.V.7.014` **Navigation: wind/current vector triangle** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙geometry · challenge
- `T.V.7.015` **Ambiguous case: height vs given side decision tree** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry · challenge
- `T.V.7.016` **Largest angle opposite largest side justification** — `UK_GCSE_H`
- `T.V.7.017` **Flight path bearings with ground speed** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AI_SL,IB_AI_HL` · ⚙geometry · challenge
- `T.V.7.018` **Bearings: airport runway / orienteering contexts** — `UK_GCSE_H` · ⚙geometry
- `T.V.7.019` **Bearings navigation paper 1** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.020` **Bearings navigation paper 2** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.021` **Bearings navigation paper 3** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.022` **Bearings navigation paper 4** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.7.023` **Bearings reverse and multi-leg combo challenge** — `UK_GCSE_H` · ⚙geometry · challenge

#### `V.8` Circles (22)

- `T.V.8.001` **Circle theorems: angle in a semicircle** — `UK_GCSE_H`
- `T.V.8.002` **Circle theorems: centre angle is twice** — `UK_GCSE_H`
- `T.V.8.003` **Circle theorems: angles in same segment** — `UK_GCSE_H`
- `T.V.8.004` **Circle theorems: opposite angles cyclic quad** — `UK_GCSE_H`
- `T.V.8.005` **Circle theorems: alternate segment** — `UK_GCSE_H` · challenge
- `T.V.8.006` **Circle theorems: tangent-chord angle** — `UK_GCSE_H` · challenge
- `T.V.8.007` **Circle theorems mixed proof pack** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.008` **Equation of circle centre origin + tangent** — `UK_GCSE_H`
- `T.V.8.009` **Tangent from external point length** — `UK_GCSE_H`
- `T.V.8.010` **Intersecting chords length theorem** — `UK_GCSE_H,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.8.011` **Sector/segment area exact exam** — `UK_GCSE_H` · challenge
- `T.V.8.012` **Radians arc/sector IB/AP bridge** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.8.013` **Proof: tangent ⊥ radius** — `UK_GCSE_H,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry
- `T.V.8.014` **Arc length vs sector vs segment decision** — `UK_GCSE_H`
- `T.V.8.015` **Trig in circle: chord length via sine** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙geometry · challenge
- `T.V.8.016` **Circle theorems + trig hybrid problems** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.017` **Circle theorems: radius to tangent proof write** — `UK_GCSE_H` · ⚙geometry
- `T.V.8.018` **Circle theorems mixed figure 1** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.019` **Circle theorems mixed figure 2** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.020` **Circle theorems mixed figure 3** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.021` **Circle theorems mixed figure 4** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.8.022` **Circle theorems mixed figure 5** — `UK_GCSE_H` · ⚙geometry · challenge

#### `V.9` Trig functions (54)

- `T.V.9.001` **Unit circle: verticality of sine** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.002` **Unit circle: horizontality of cosine** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.003` **Unit circle: tangent as slope of radius** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.004` **Unit circle special angles exact coordinates** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.005` **Reference angles across four quadrants drills** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.006` **ASTC / CAST diagram fluency (UK)** — `UK_GCSE_H` · ⚙unit_circle
- `T.V.9.007` **Coterminal angles in degrees and radians** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.V.9.008` **Radians as arc length on unit circle** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.009` **Graph sine: build from unit circle animation** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.010` **Graph cosine: build from unit circle animation** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.011` **Amplitude/period/phase exam transformations** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.V.9.012` **Desmos: match equation to trig graph challenges** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.013` **Periodic modelling: tides and ferris wheels** — `IB_AI_SL,IB_AI_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙desmos
- `T.V.9.014` **Graph tangent with asymptotes exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.V.9.015` **Inverse trig graphs and ranges** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos
- `T.V.9.016` **Composition arcsin(sin θ) pitfalls** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.V.9.017` **Desmos: explore a sin(bx+c)+d parameters live** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.V.9.018` **Unit circle: project to axes interactively** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.019` **Negative angles on unit circle** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.020` **Co-terminal and reference mixed mega-drill** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle · challenge
- `T.V.9.021` **Desmos: compare sin x vs sin(2x) vs 2sin x** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos
- `T.V.9.022` **Unit circle: quiz coordinates at π/6 multiples** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.023` **Convert DMS ↔ decimal degrees exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.V.9.024` **Angular speed and linear speed link** — `IB_AI_SL,IB_AI_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.V.9.025` **Graph cosec/sec/cot from sine/cosine** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos · challenge
- `T.V.9.026` **Phase shift left/right common student errors** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.V.9.027` **Interactive: drag angle see sin/cos update** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.028` **Fourier intuition: sum of sines preview** — `IB_AA_HL,AP_CALC_BC,IB_AA_HL` · ⚙desmos · strange
- `T.V.9.029` **Desmos: find period from two zeros** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.V.9.030` **Unit circle symmetry: odd/even visual proof** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.031` **Model daylight hours with cosine** — `IB_AI_SL,IB_AI_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.032` **Radians exclusively: no degree crutches** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle · challenge
- `T.V.9.033` **Interactive geometry: isolate sin vs cos projections** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.034` **Desmos: solve sin x = cos x graphically and exactly** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.V.9.035` **Amplitude from max−min; midline average** — `IB_AI_SL,IB_AI_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.V.9.036` **Unit circle: memory palace for special angles** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙unit_circle
- `T.V.9.037` **Desmos: Fourier square-wave tease with odd harmonics** — `IB_AA_HL,AP_CALC_BC,IB_AA_HL` · ⚙desmos · strange
- `T.V.9.038` **Unit circle fluency round 1** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.039` **Unit circle fluency round 2** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.040` **Unit circle fluency round 3** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.041` **Unit circle fluency round 4** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.042` **Unit circle fluency round 5** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.043` **Unit circle fluency round 6** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.044` **Unit circle fluency round 7** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.045` **Desmos trig graph challenge 1** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.046` **Desmos trig graph challenge 2** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.047` **Desmos trig graph challenge 3** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.048` **Desmos trig graph challenge 4** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.049` **Desmos trig graph challenge 5** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.050` **Desmos trig graph challenge 6** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.051` **Desmos trig graph challenge 7** — `IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.9.052` **Unit circle: verticality drill with readout** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.053` **Unit circle: horizontality drill with readout** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙unit_circle
- `T.V.9.054` **Desmos: rebuild tide model from data points** — `IB_AI_SL,IB_AI_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge

#### `V.10` Identities & equations (35)

- `T.V.10.001` **Prove identities structured exam write-ups** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.V.10.002` **Pythagorean identities rearrange toolkit** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.V.10.003` **Compound angle applications: expand sin(A±B)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,IB_AA_HL`
- `T.V.10.004` **Compound angle applications: find exact values** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.005` **Double-angle in equation solving** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.10.006` **Half-angle and t-formulae (where on syllabus)** — `IB_AA_HL` · strange · uncertain
- `T.V.10.007` **Harmonic form R sin(θ±α) exam pack** — `UK_GCSE_H,IB_AA_HL` · challenge
- `T.V.10.008` **Graphical solutions of trig equations** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.V.10.009` **General solutions in degrees and radians** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.V.10.010` **Trig equations with multiple angles** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.011` **Factor formulae applications (HL)** — `IB_AA_HL` · challenge
- `T.V.10.012` **Desmos: verify identity numerically then prove** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙desmos
- `T.V.10.013` **Exam mixed identity + equation mega-set** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.014` **Linear combinations to single sinusoid modelling** — `IB_AI_SL,IB_AI_HL,IB_AA_HL` · ⚙desmos
- `T.V.10.015` **cos(A−B) expansion applications** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.10.016` **sin(A+B) in wave interference light model** — `IB_AI_SL,IB_AI_HL` · ⚙desmos · strange
- `T.V.10.017` **Product-to-sum formulas light use** — `IB_AA_HL` · strange
- `T.V.10.018` **Solve trig equations on restricted intervals** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.V.10.019` **Identity proof: split into cases strategy** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · challenge
- `T.V.10.020` **Equations: quadratic in sin/cos** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.021` **Compound angle: expand cos(A+B) then simplify** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.10.022` **Prove sin(A+B) from area or Ptolemy light** — `IB_AA_HL` · strange
- `T.V.10.023` **Exam: which identity first? decision drills** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.024` **Hard identity: multi-formula chain** — `IB_AA_SL,IB_AA_HL,IB_AA_HL` · challenge
- `T.V.10.025` **Identities exam pack 1** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.026` **Identities exam pack 2** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.027` **Identities exam pack 3** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.028` **Identities exam pack 4** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.029` **Identities exam pack 5** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.V.10.030` **Trig equations graphical+algebraic 1** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.10.031` **Trig equations graphical+algebraic 2** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.10.032` **Trig equations graphical+algebraic 3** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.10.033` **Trig equations graphical+algebraic 4** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.V.10.034` **Compound angle application: sin(75°) exact** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.V.10.035` **Compound angle application: cos(15°) exact** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`

#### `V.11` Coordinate geometry (4)

- `T.V.11.001` **Coordinate proofs of parallelograms/rhombus** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.11.002` **Equation of perpendicular bisector loci link** — `UK_GCSE_H`
- `T.V.11.003` **G-GPE: circle and parabola algebraically** — `US_CCSS_HS`
- `T.V.11.004` **Partition section formula internal/external** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge

#### `V.12` Conic sections (2)

- `T.V.12.001` **Complete square to identify conics** — `US_CCSS_HS,UK_GCSE_H,IB_AA_SL,IB_AA_SL,IB_AA_HL`
- `T.V.12.002` **Eccentricity and focus-directrix exam (light)** — `IB_AA_HL,US_CCSS_HS` · strange · uncertain

#### `V.13` Transformations (5)

- `T.V.13.001` **Describe fully: translation reflection rotation enlargement** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.V.13.002` **Invariant points and lines under transforms** — `UK_GCSE_H` · challenge
- `T.V.13.003` **Matrix representation of 2D transformations** — `IB_AI_HL,IB_AA_HL,US_CCSS_HS` · ⚙geometry
- `T.V.13.004` **Composition of transformations exam order** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_HL,IB_AI_HL` · challenge
- `T.V.13.005` **Enlargement negative SF with centre** — `UK_GCSE_H` · ⚙geometry · challenge

#### `V.14` Solids (5)

- `T.V.14.001` **Plans elevations link to volume estimates** — `UK_GCSE_H`
- `T.V.14.002` **G-GMD Cavalieri justification language** — `US_CCSS_HS`
- `T.V.14.003` **Density design problems (mass = density×volume)** — `UK_GCSE_H`
- `T.V.14.004` **Frustum volume (where assessed)** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL` · challenge
- `T.V.14.005` **Cross-sections of cubes/pyramids exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · ⚙geometry

#### `V.15` Constructions (11)

- `T.V.15.001` **Exam construction: perpendicular bisector** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.V.15.002` **Exam construction: angle bisector** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.V.15.003` **Exam construction: equilateral / 60°** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.V.15.004` **Exam construction: regular hexagon in circle** — `UK_GCSE_H` · ⚙geometry
- `T.V.15.005` **Exam construction: parallel through point** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.V.15.006` **Loci constructions combined with regions** — `UK_GCSE_H` · ⚙geometry · challenge
- `T.V.15.007` **Construct 45° and 90° exam techniques** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.V.15.008` **Construct triangle given ASA accurately** — `UK_GCSE_F,UK_KS3,IB_MYP` · ⚙geometry
- `T.V.15.009` **Construction accuracy drill 1** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.V.15.010` **Construction accuracy drill 2** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry
- `T.V.15.011` **Construction accuracy drill 3** — `UK_GCSE_F,UK_KS3,IB_MYP,UK_GCSE_H,IB_AA_SL,IB_AI_SL` · ⚙geometry

### Era VI — Change

#### `VI.1` Limits & continuity (14)

- `T.VI.1.001` **AP FRQ: limit justification from table/graph** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.1.002` **Formal limit language where AP demands precision** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.1.003` **IVT justification FRQ stems** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.1.004` **Continuity checklist FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.1.005` **Limits analytically vs numerically GDC** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙gdc
- `T.VI.1.006` **Squeeze theorem justification write-ups** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.1.007` **Horizontal asymptotes via limits at infinity FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.1.008` **Vertical asymptotes vs holes FRQ language** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.1.009` **Epsilon-N / epsilon-delta light AP+** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · strange
- `T.VI.1.010` **One-sided limits for piecewise continuity** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.1.011` **Limit & continuity FRQ variant 1** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.1.012` **Limit & continuity FRQ variant 2** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.1.013` **Limit & continuity FRQ variant 3** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.1.014` **Limit of piecewise defined at junction** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`

#### `VI.2` Derivatives (12)

- `T.VI.2.001` **AP FRQ: definition of derivative as limit** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.002` **Differentiability vs continuity FRQ traps** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.003` **L'Hôpital packaging as named AP topic** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.004` **Implicit differentiation AP FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.005` **Related rates setup sentence frames** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.006` **Calculator-active derivative estimates** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙gdc
- `T.VI.2.007` **Chain rule layered AP items** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.008` **Second derivative from parametric (BC)** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.2.009` **Logarithmic differentiation AP items** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.2.010` **Motion along a line: when particle at rest** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.011` **Approximate derivative from table FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.2.012` **Product and quotient rule mixed AP set** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`

#### `VI.3` Applications of derivatives (23)

- `T.VI.3.001` **MVT justification FRQ stems** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.002` **EVT / Extreme Value Theorem justification** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.003` **Candidates test write-up discipline** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.004` **f, f', f'' sign chart FRQ classic** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.3.005` **Optimization AP contextual FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.006` **Linearisation / tangent approx error talk** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.007` **Particle motion: velocity/acceleration FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.008` **Newton's method AP/IB numerical** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙gdc
- `T.VI.3.009` **Related rates classic cone/ladder/shadow** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.010` **Concavity and inflection FRQ write-ups** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.3.011` **L'Hôpital repeated applications** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.012` **Graphing calculator: find zeros of f'** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙gdc
- `T.VI.3.013` **AP calculator-active vs inactive practice modes** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙gdc
- `T.VI.3.014` **Absolute extrema on closed interval FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.015` **AP FRQ justification practice 1** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.016` **AP FRQ justification practice 2** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.017` **AP FRQ justification practice 3** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.018` **AP FRQ justification practice 4** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.019` **AP FRQ justification practice 5** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.020` **AP FRQ justification practice 6** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.021` **AP FRQ justification practice 7** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.3.022` **Related rates with similar triangles** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.3.023` **Curve sketching from calculus summary table** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos

#### `VI.4` Integrals (14)

- `T.VI.4.001` **Riemann sum notation left/right/mid FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.4.002` **FTC graphical accumulation FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph
- `T.VI.4.003` **Average value theorem applications** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.4.004` **Definite integral properties FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.4.005` **Trapezoidal rule approximation FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.4.006` **FTC derivative of integral with variable limits** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.4.007` **AP numerical integration on GDC** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙gdc
- `T.VI.4.008` **Accumulation from rate-in rate-out FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph · challenge
- `T.VI.4.009` **Signed area vs total area language** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph
- `T.VI.4.010` **FTC accumulation FRQ variant 1** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph · challenge
- `T.VI.4.011` **FTC accumulation FRQ variant 2** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph · challenge
- `T.VI.4.012` **FTC accumulation FRQ variant 3** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph · challenge
- `T.VI.4.013` **Midpoint Riemann sum vs trapezoid compare** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.4.014` **Fundamental theorem verbal interpretations** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`

#### `VI.5` Integration techniques (5)

- `T.VI.5.001` **Integration by parts IB AA / AP BC** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL`
- `T.VI.5.002` **Partial fractions integration exam** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.5.003` **Improper integrals convergence tests light** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.5.004` **Trigonometric integrals powers of sin/cos** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.5.005` **Trigonometric substitution light (BC/HL)** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · strange

#### `VI.6` Applications of integrals (10)

- `T.VI.6.001` **Area between curves AP FRQ classic** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.6.002` **Disk/washer volume FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.6.003` **Known cross-section volume FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.6.004` **Net change theorem worded FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.6.005` **Arc length setup (BC)** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.6.006` **Shell method when washer awkward** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.6.007` **Work pumping liquid FRQ style** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.6.008` **Probability density integral applications** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,AP_STATS,IB_AI_HL,IB_AI_SL` · strange
- `T.VI.6.009` **Displacement from velocity graph areas** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙graph
- `T.VI.6.010` **Washer method horizontal axis vs vertical** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge

#### `VI.7` Differential equations I (20)

- `T.VI.7.001` **Slope fields sketch and match FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.7.002` **Euler's method table FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.7.003` **Logistic DE: dP/dt=kP(M−P) exam pack** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.7.004` **Separable DE with initial condition FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL`
- `T.VI.7.005` **Growth/decay DE contextual FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AI_SL,IB_AI_HL`
- `T.VI.7.006` **Newton cooling DE exam** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AI_SL,IB_AI_HL`
- `T.VI.7.007` **Mixing problems DE setup** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.7.008` **Equilibrium solutions stability talk** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL`
- `T.VI.7.009` **IB DE modelling emphasis pack** — `IB_AI_SL,IB_AI_HL,IB_AA_SL,IB_AA_HL` · challenge
- `T.VI.7.010` **Particular vs general solution language** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.7.011` **Euler vs analytic solution comparison** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙gdc
- `T.VI.7.012` **Logistic carrying capacity interpretation** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.7.013` **Slope field: draw solution through a point** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos
- `T.VI.7.014` **Euler method stepped table 1** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.7.015` **Logistic model interpretation 1** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.7.016` **Euler method stepped table 2** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.7.017` **Logistic model interpretation 2** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.7.018` **Euler method stepped table 3** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL`
- `T.VI.7.019` **Logistic model interpretation 3** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.7.020` **Verify a proposed solution to a DE** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL`

#### `VI.8` Parametric & polar (19)

- `T.VI.8.001` **Parametric derivatives dy/dx FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.002` **Parametric arc length FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.003` **Particle path parametric motion FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.004` **Polar area ½∫r² dθ FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.005` **Polar slope dy/dx in polar form** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.8.006` **Common polar curves recognition pack** — `AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.VI.8.007` **Convert polar ↔ cartesian exam** — `AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL`
- `T.VI.8.008` **Area between polar curves FRQ** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.8.009` **Desmos polar graphing exploration** — `AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL` · ⚙desmos
- `T.VI.8.010` **Vector-valued position/velocity/acceleration** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.011` **Polar to area of roses petals count** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.012` **Eliminate parameter then differentiate check** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.013` **Polar area shared regions careful bounds** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.014` **Polar/parametric FRQ segment 1** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.015` **Polar/parametric FRQ segment 2** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.016` **Polar/parametric FRQ segment 3** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.017` **Polar/parametric FRQ segment 4** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos · challenge
- `T.VI.8.018` **Speed vs velocity parametric distinction** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.8.019` **Polar intercepts and symmetry tests** — `AP_CALC_BC,IB_AA_HL` · ⚙desmos

#### `VI.9` Sequences & series (17)

- `T.VI.9.001` **Series tests battery: nth-term first** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.002` **Integral test with remainder estimate** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.003` **Comparison and limit comparison drills** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.004` **Alternating series test + error bound** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.005` **Ratio test radius of convergence workflow** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.006` **Absolute vs conditional convergence FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.007` **Which test? decision tree mega-drill** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.008` **p-series and geometric recognition speed** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.9.009` **Root test when ratio inconclusive** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.010` **Telescoping series recognition** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.011` **Limit comparison with asymptotic equivalence** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.012` **Series tests mixed battery 1** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.013` **Series tests mixed battery 2** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.014` **Series tests mixed battery 3** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.015` **Series tests mixed battery 4** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.016` **Series tests mixed battery 5** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.9.017` **Geometric series of functions radius** — `AP_CALC_BC,IB_AA_HL`

#### `VI.10` Power & Taylor series (17)

- `T.VI.10.001` **Taylor/Maclaurin polynomial construction FRQ** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL`
- `T.VI.10.002` **Lagrange error bound FRQ** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.10.003` **Alternating series error for Taylor** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.10.004` **Manipulate known Maclaurin series** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL`
- `T.VI.10.005` **Interval of convergence endpoint checks** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.10.006` **Series for e^x, sin x, cos x, 1/(1−x) fluency** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL`
- `T.VI.10.007` **Approximate integrals via series FRQ** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.10.008` **IB AA HL Maclaurin exam packaging** — `IB_AA_HL` · challenge
- `T.VI.10.009` **Binomial series expansion (1+x)^k** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.10.010` **Taylor series for ln(1+x) and arctan** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.10.011` **Error bounds choose Lagrange vs alternating** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.10.012` **Replace x by x² etc. in Maclaurin** — `AP_CALC_BC,IB_AA_HL`
- `T.VI.10.013` **Taylor error bound practice 1** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.10.014` **Taylor error bound practice 2** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.10.015` **Taylor error bound practice 3** — `AP_CALC_BC,IB_AA_HL` · challenge
- `T.VI.10.016` **Center of Taylor series not zero** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · challenge
- `T.VI.10.017` **Series solution approximation of DE light** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · strange

#### `VI.11` Statistical inference (48)

- `T.VI.11.001` **Study design: experiment vs observational** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.002` **Sampling methods named pack** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.003` **Bias types: undercoverage, nonresponse, response** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.004` **Simulation-based inference pedagogy** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.005` **One-proportion z-interval procedure** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.006` **One-proportion z-test procedure** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.007` **Two-proportion z procedures** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.008` **One-sample t-interval for mean** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.009` **One-sample t-test for mean** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.010` **Two-sample t procedures / paired data** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.011` **Chi-square GOF test** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL`
- `T.VI.11.012` **Chi-square independence / homogeneity** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL` · challenge
- `T.VI.11.013` **Slope inference / CI for regression slope** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL` · challenge
- `T.VI.11.014` **AP Stats FRQ investigative communication** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.015` **Formula sheet / table fluency (z,t,χ²)** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.016` **IB AI inference GDC workflows** — `IB_AI_HL,IB_AI_SL` · ⚙gdc
- `T.VI.11.017` **Type I / Type II errors in context** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL`
- `T.VI.11.018` **Conditions check mantra before every procedure** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.019` **Pooling for two-proportion z-test** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.020` **df for t and χ² fluency** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.021` **Confidence level vs interval width tradeoff** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.022` **Writing hypotheses H0 Ha templates** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.023` **Conclusion sentence frames AP style** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.024` **IB AI bivariate: Pearson r interpretation** — `IB_AI_SL,IB_AI_HL` · ⚙gdc
- `T.VI.11.025` **IB AI: Spearman rank correlation (if in guide)** — `IB_AI_HL` · strange · uncertain
- `T.VI.11.026` **Margin of error from CI half-width** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.027` **AP Stats 2026 CED Unit checklist overlay** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.028` **Chi-square expected counts computation** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_HL`
- `T.VI.11.029` **Blocking in experiments** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.030` **Interpreting slope and intercept in context** — `AP_STATS,IB_AI_HL,IB_AI_SL,IB_AI_SL,IB_AI_HL`
- `T.VI.11.031` **Standard error vs standard deviation language** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.032` **Full inference write-up timed drills** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.033` **Power of a test conceptually** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.034` **Interpreting P-value correctly (language drills)** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.035` **IB AI χ² GDC and critical value methods** — `IB_AI_HL` · ⚙gdc
- `T.VI.11.036` **Matched pairs design advantages** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.037` **AP Stats: interpreting r² in context** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.038` **AP Stats procedure write-up 1** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.039` **AP Stats procedure write-up 2** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.040` **AP Stats procedure write-up 3** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.041` **AP Stats procedure write-up 4** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.042` **AP Stats procedure write-up 5** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge
- `T.VI.11.043` **IB AI inference GDC task 1** — `IB_AI_HL,IB_AI_SL` · ⚙gdc · challenge
- `T.VI.11.044` **IB AI inference GDC task 2** — `IB_AI_HL,IB_AI_SL` · ⚙gdc · challenge
- `T.VI.11.045` **IB AI inference GDC task 3** — `IB_AI_HL,IB_AI_SL` · ⚙gdc · challenge
- `T.VI.11.046` **Interpreting confidence interval correctly** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.047` **Randomization in experiments vs sampling** — `AP_STATS,IB_AI_HL,IB_AI_SL`
- `T.VI.11.048` **Simulation of sampling distribution of phat** — `AP_STATS,IB_AI_HL,IB_AI_SL` · challenge

#### `VI.12` Mechanics (2)

- `T.VI.12.001` **SUVAT links to calculus motion FRQ** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AI_HL`
- `T.VI.12.002` **Variable acceleration from a(t)** — `AP_CALC_AB,AP_CALC_BC,IB_AA_HL,IB_AA_SL,IB_AA_HL`

### Era VII — Space

#### `VII.1` Vectors in ℝⁿ (29)

- `T.VII.1.001` **Column vectors GCSE notation** — `UK_GCSE_H`
- `T.VII.1.002` **Vector geometry: midpoint and section formula** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.VII.1.003` **Vector proof: parallelogram / midpoint theorem** — `UK_GCSE_H` · challenge
- `T.VII.1.004` **Vector proof: collinearity and ratio** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · challenge
- `T.VII.1.005` **Position vectors in plane exam pack** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.VII.1.006` **Magnitude and unit vectors GCSE/IB** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AI_SL`
- `T.VII.1.007` **Vector geometric proof exercise 1** — `UK_GCSE_H` · challenge
- `T.VII.1.008` **Vector geometric proof exercise 2** — `UK_GCSE_H` · challenge
- `T.VII.1.009` **Vector geometric proof exercise 3** — `UK_GCSE_H` · challenge
- `T.VII.1.010` **N-VM (+) vectors applications bridge** — `US_CCSS_HS`
- `T.VII.1.011` **Dot product: perpendicular test exam** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.1.012` **Vector equation of a line (IB)** — `IB_AA_SL,IB_AA_HL,IB_AA_HL`
- `T.VII.1.013` **Angle between vectors exam** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.1.014` **IB AI/AA vector applications in geometry** — `IB_AA_SL,IB_AA_HL,IB_AI_SL,IB_AI_HL` · challenge
- `T.VII.1.015` **Unit vector in direction of motion** — `IB_AA_SL,IB_AA_HL,AP_CALC_BC,IB_AA_HL`
- `T.VII.1.016` **Scalar projection applications** — `IB_AA_SL,IB_AA_HL,AP_CALC_BC,IB_AA_HL`
- `T.VII.1.017` **3D coordinates distance and midpoint** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.VII.1.018` **Vector proof of median concurrency light** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL` · strange
- `T.VII.1.019` **Displacement vs position vector clarity** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.VII.1.020` **IB AA HL vector product magnitude area** — `IB_AA_HL` · challenge
- `T.VII.1.021` **Resultant forces as vector sums** — `IB_AI_SL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.VII.1.022` **Unit vector i,j,k notation fluency** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.VII.1.023` **Parallel vectors scalar multiple test** — `UK_GCSE_H,IB_AA_SL,IB_AI_SL,IB_AA_SL,IB_AA_HL`
- `T.VII.1.024` **Vector journeys multi-stage collinearity** — `UK_GCSE_H` · challenge
- `T.VII.1.025` **Component form from magnitude and direction** — `IB_AA_SL,IB_AA_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL,AP_CALC_BC,IB_AA_HL`
- `T.VII.1.026` **Vector geometry GCSE Higher 1** — `UK_GCSE_H` · challenge
- `T.VII.1.027` **Vector geometry GCSE Higher 2** — `UK_GCSE_H` · challenge
- `T.VII.1.028` **Vector geometry GCSE Higher 3** — `UK_GCSE_H` · challenge
- `T.VII.1.029` **Vector geometry GCSE Higher 4** — `UK_GCSE_H` · challenge

#### `VII.2` Linear systems (4)

- `T.VII.2.001` **Gaussian elimination exam discipline** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.2.002` **Consistent vs inconsistent systems language** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.2.003` **Augmented matrix notation fluency** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.2.004` **Parameter count for infinite solutions** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`

#### `VII.3` Matrix algebra (19)

- `T.VII.3.001` **IB HL matrices for 2D transformations pack** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry
- `T.VII.3.002` **Solve 2×2 systems with inverse matrices** — `IB_AA_HL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL,US_CCSS_HS`
- `T.VII.3.003` **Determinant 2×2 geometric area link** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.3.004` **Matrix multiplication non-commutativity demos** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.3.005` **AP Precalc / (+) matrices systems bridge** — `US_CCSS_HS`
- `T.VII.3.006` **Inverse of 2×2 formula fluency** — `IB_AA_HL,IB_AI_HL,UK_GCSE_H,IB_AA_SL,IB_AI_SL`
- `T.VII.3.007` **Identity and zero matrix roles** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.3.008` **Transpose properties (A+B)^T etc.** — `IB_AA_HL,IB_AI_HL`
- `T.VII.3.009` **Solving matrix equations AX=B** — `IB_AA_HL,IB_AI_HL` · challenge
- `T.VII.3.010` **Coded messages / Hill cipher light (fun)** — `IB_AA_HL,IB_AI_HL` · strange
- `T.VII.3.011` **US Precalculus matrix applications pack** — `US_CCSS_HS`
- `T.VII.3.012` **Exam mixed 2×2 matrix mega-set** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · challenge
- `T.VII.3.013` **Matrix encoding of simultaneous equations** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.3.014` **Matrix representation of complex multiply light** — `IB_AA_HL` · strange
- `T.VII.3.015` **Matrix transform exam figure 1** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry · challenge
- `T.VII.3.016` **Matrix transform exam figure 2** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry · challenge
- `T.VII.3.017` **Matrix transform exam figure 3** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry · challenge
- `T.VII.3.018` **Matrix transform exam figure 4** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry · challenge
- `T.VII.3.019` **Matrix transform area scale |det| interpretation** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry

#### `VII.4` Vector spaces (2)

- `T.VII.4.001` **Linear independence of 2–3 vectors in R2/R3** — `IB_AA_HL,IB_AI_HL`
- `T.VII.4.002` **Basis of R² standard and rotated** — `IB_AA_HL` · strange

#### `VII.5` Linear transformations (11)

- `T.VII.5.001` **Geometric linear maps: stretch shear rotate** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry
- `T.VII.5.002` **Composition of matrix transformations order** — `IB_AA_HL,IB_AI_HL` · challenge
- `T.VII.5.003` **Kernel and image geometric meaning (light)** — `IB_AA_HL` · strange
- `T.VII.5.004` **Reflection matrices in x/y axes and y=x** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry
- `T.VII.5.005` **Rotation matrices by θ standard form** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS` · ⚙geometry
- `T.VII.5.006` **Enlargement matrix kI** — `IB_AA_HL,IB_AI_HL` · ⚙geometry
- `T.VII.5.007` **Shear matrices and invariant lines** — `IB_AI_HL,IB_AA_HL` · ⚙geometry · challenge
- `T.VII.5.008` **Inverse transformation matrix meaning** — `IB_AA_HL,IB_AI_HL`
- `T.VII.5.009` **Determinant as oriented area scale factor** — `IB_AA_HL,IB_AI_HL` · ⚙geometry · challenge
- `T.VII.5.010` **Standard matrix recognition 1** — `IB_AA_HL,IB_AI_HL` · ⚙geometry
- `T.VII.5.011` **Standard matrix recognition 2** — `IB_AA_HL,IB_AI_HL` · ⚙geometry

#### `VII.6` Determinants (3)

- `T.VII.6.001` **Determinant expand vs row-reduce choice** — `IB_AA_HL,IB_AI_HL`
- `T.VII.6.002` **Singular matrices and no inverse** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`
- `T.VII.6.003` **Cramer's rule 2×2 (optional method)** — `IB_AA_HL,IB_AI_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL` · strange

#### `VII.7` Eigenvalues & eigenvectors (2)

- `T.VII.7.001` **Eigenvalues 2×2 exam pack (light)** — `IB_AA_HL,IB_AI_HL` · challenge
- `T.VII.7.002` **Diagonalisation idea for matrix powers light** — `IB_AA_HL` · strange

#### `VII.8` Orthogonality (1)

- `T.VII.8.001` **Orthogonal vectors in R² exam** — `IB_AA_SL,IB_AA_HL,US_CCSS_HS,UK_GCSE_H,IB_AA_SL`

#### `VII.10` Functions of several variables (1)

- `T.VII.10.001` **Partial derivatives notation exam light** — `IB_AA_HL,AP_CALC_BC,IB_AA_HL` · strange

#### `VII.14` Vector calculus (1)

- `T.VII.14.001` **Vector fields intuition AP+ bridge** — `AP_CALC_BC,IB_AA_HL,IB_AA_HL` · ⚙desmos · strange

---

## Trig interactive / Desmos exercise ideas

Concrete prompts for V.6–V.10 testing skills flagged `desmos` / `unit_circle` / `geometry` / `graph`. Use with Desmos Graphing Calculator, unit-circle widgets, or geometry tools.

1. **Vertical sine:** On a unit circle, drag θ and plot (θ, y-coordinate) live — label the y-readout as sin θ.
2. **Horizontal cosine:** Same circle; plot (θ, x-coordinate) as cos θ; toggle vertical vs horizontal projection overlays.
3. **Tangent as slope:** Show the terminal ray; display its slope next to tan θ; sync a tan graph.
4. **Special-angle coordinates:** Quiz mode — hide labels; tap π/6, π/4, π/3 points and type exact (x,y).
5. **CAST signs:** Colour quadrants; student predicts sign of sin/cos/tan before revealing.
6. **Reference-angle machine:** Input any degree/radian; animate reduction to reference + sign.
7. **Build sine from motion:** Trace a point on the circle while a linked point draws y=sin θ.
8. **Build cosine from motion:** Same for x=cos θ; compare phase to sine.
9. **Parameter playground:** Sliders for a, b, c, d in y=a sin(bx+c)+d; write verbal effect cards.
10. **Match equation ↔ graph:** Desmos card sort — 8 graphs, 8 equations (amplitude/period/phase/midline).
11. **sin x vs sin(2x) vs 2sin x:** Three overlays; students annotate which change is which.
12. **Tide model fit:** Paste tide height table; fit a sine; interpret a, period, phase, midline.
13. **Ferris-wheel height:** Parametric or sine model; find times above a height.
14. **Daylight hours cosine:** Fit daylight data; predict solstice/eqinox features.
15. **Tangent asymptotes:** Sketch y=tan x with correct asymptotes; check against Desmos.
16. **Inverse ranges:** Graph arcsin/arccos/arctan with forced ranges; test composition traps.
17. **arcsin(sin θ) pitfall:** Slider θ through multiple turns; plot arcsin(sin θ) vs θ.
18. **Solve sin x = cos x:** Graphical intersections + exact π/4 + general solution.
19. **Period from two zeros:** Given two consecutive zeros on a blank graph, recover period and a candidate equation.
20. **Amplitude from max−min:** Given max/min only, recover a and midline; then fit phase.
21. **Identity verify then prove:** Plot LHS−RHS for a proposed identity; then write formal proof.
22. **Harmonic form:** Convert a sinθ + b cosθ; overlay R sin(θ−α) and match.
23. **Compound-angle exact:** Compute sin75° / cos15° via sum/difference; confirm numerically.
24. **Double-angle solver:** Graph sin2θ = k; list solutions on [0,2π]; check algebra.
25. **Multiple-angle:** Solve cos3θ = 1/2 graphically and algebraically; compare counts.
26. **Restricted-interval solutions:** Shade [0,360°] or [0,2π]; mark all solutions.
27. **Bearings geometry:** Dynamic diagram — north arrow, three-figure bearing, reverse bearing +180°.
28. **Multi-leg bearings:** Vector chain on a map grid; find final displacement and bearing home.
29. **Ambiguous case SSA:** Drag side length through the critical height; show 0/1/2 triangles.
30. **Area ½ab sin C:** Interactive triangle; live area; compare to Heron.
31. **Circle theorems pack:** Geogebra/Desmos geometry — toggle theorems; student fills reasons.
32. **Segment area:** Sector minus triangle animation; exact π form toggle.
33. **Chord via sine:** Chord = 2r sin(θ/2) with draggable central angle.
34. **3D trig optional:** Cuboid with space diagonal; show angle line-to-plane (mark optional).
35. **Elevation/depression:** Clinometer-style diagram; two-triangle shared height.
36. **Polar roses:** Desmos r=a cos(nθ); count petals; shade one petal area.
37. **Parametric particle:** Trace (x(t),y(t)); show velocity vector; speed readout.
38. **Fourier tease:** Sum odd harmonics toward square wave; link to V.9 strange skill.
39. **Radians-only mode:** Disable degree display; solve a set staying in radians.
40. **Projection toggle:** Unit-circle tool with buttons 'show sin (vertical)' / 'show cos (horizontal)' only.
41. **Negative angles:** Clockwise θ; connect to odd/even visual proof.
42. **Coterminal spiral:** Show θ and θ±2πk on circle; list three coterminal measures.
43. **DMS converter:** Input 35°20';; convert; use in a right-trig solve.
44. **Reciprocal graphs:** Derive csc/sec/cot from sin/cos graphs with asymptotes.
45. **Phase-shift error clinic:** Deliberately wrong equations; students diagnose left/right mistakes.
46. **Ladder against wall:** Dynamic right triangle; exact vs calculator decision prompt.
47. **Roof pitch:** Rise/run → tanθ → inclination; accessibility ramp check.
48. **Navigation triangle:** Airspeed/wind/groundspeed vector triangle with bearings.
49. **Graphical trig equation mega-set:** 6 equations; Desmos intersections; general solutions write-up.
50. **Unit-circle fluency rounds:** Timed 20-question coordinate/sign drills (skills T.V.9.* rounds).
51. **Exact-value application geometry:** Isosceles/split-base figures needing 30-60-90 exact values.
52. **Tangent graph match:** Match three tan transforms to graphs including asymptote shifts.
53. **Periodic model residuals:** After fitting tide model, plot residuals; discuss systematic error.
54. **Law of cosines obtuse:** Drag angle through 90°; watch cos sign and side opposite.
55. **Circle + trig hybrid:** Inscribed angle with trig length chase in one figure.
56. **Desmos activity: rebuild from verbal description** — 'period 4π, amplitude 3, shifted left π/2, mid 1'.

---

## Missing regions summary (UK / IB / US → skill-id ranges)

Gap themes from the three comparison papers, mapped to Testing Mode skill-id prefixes.

### UK National Curriculum → Testing skills

| Gap theme | Primary branch / id range | Tracks |
|-----------|---------------------------|--------|
| Roman numerals | `T.I.1.*`, `T.I.3.*`, `T.II.1.*` | UK_KS2 |
| British money £/p & change | `T.I.4.*`, `T.I.7.*`, `T.II.7.*` | UK_KS2 |
| 12/24-hour clock & timetables | `T.I.7.*` | UK_KS2 |
| Imperial↔metric equivalences | `T.II.9.*` | UK_KS2 |
| Formal column / long mult / long div | `T.I.4.*`, `T.II.1–3.*` | UK_KS2 |
| 12×12 tables milestone | `T.II.2.*` | UK_KS2 |
| Axis-parallel translation/reflection | `T.II.9.*` | UK_KS2 |
| Standard form A×10ⁿ | `T.III.1.*` | UK_KS3, GCSE |
| Financial % / compound interest | `T.III.3.*`, `T.IV.12.*` | UK_KS3–GCSE_H |
| Compound measures (speed/density/pressure) | `T.III.2.*` | UK_KS3–GCSE |
| Bearings (3-figure, reverse, multi-leg) | `T.III.8.*`, `T.V.7.*` | GCSE |
| Plans & elevations | `T.III.8.*` | GCSE |
| Circle theorems Higher | `T.V.8.*` | UK_GCSE_H |
| Exact trig values | `T.V.6.*`, `T.V.9.*` | UK_GCSE_H |
| Sine/cosine rules & ½ab sin C | `T.V.7.*` | UK_GCSE_H |
| Surds / fractional indices | `T.III.4.*`, `T.IV.5.*` | UK_GCSE_H |
| Bounds / limits of accuracy | `T.III.1.*` | UK_GCSE_H |
| Iteration | `T.IV.7.*` | UK_GCSE_H |
| Unequal histograms & CF | `T.III.9.*` | UK_GCSE_H |
| Venn probability / product rule | `T.III.9.*`, `T.IV.14.*` | GCSE_H |
| Vector geometric proof | `T.VII.1.*` | UK_GCSE_H |
| Circle equation + tangent (origin) | `T.IV.3.*`, `T.V.8.*` | UK_GCSE_H |

### IB MYP / DP AA–AI → Testing skills

| Gap theme | Primary branch / id range | Tracks |
|-----------|---------------------------|--------|
| GDC workflows | many `interactive: gdc` across III–VI | IB_* |
| Modelling cycle (AI) | `T.IV.12.*`, `T.VI.7.*` | IB_AI_* |
| Hypothesis tests / CIs (AI HL) | `T.VI.11.*` | IB_AI_HL, AP_STATS |
| Chi-square / bivariate tech | `T.VI.11.*`, `T.IV.15.*` | IB_AI_HL |
| Voronoi (**uncertain**) | `T.III.8.*` (flagged uncertain) | IB_AI_HL |
| Graph theory light (**uncertain**) | `T.III.8.*` | IB_AI_HL |
| Proof by induction (AA HL) | `T.V.1.*`, `T.IV.13.*` | IB_AA_HL |
| Complex numbers HL depth | `T.IV.8.*` | IB_AA_HL |
| Maclaurin / series HL | `T.VI.9–10.*` | IB_AA_HL, AP_CALC_BC |
| Matrices transforms HL | `T.VII.3.*`, `T.VII.5.*`, `T.V.13.*` | IB_*_HL |
| Exploration mini-write bridge | `T.V.1.*` | IBALL |

### US CCSSM + AP Calc/Stats → Testing skills

| Gap theme | Primary branch / id range | Tracks |
|-----------|---------------------------|--------|
| CCSS MD / Counting & Cardinality density | `T.I.1.*`, `T.I.7.*`, `T.II.10.*` | US_CCSS_K5 |
| CCSS RP domain depth | `T.III.2.*`, `T.III.3.*` | US_CCSS_68 |
| CCSS SP 6–8 | `T.III.9.*` | US_CCSS_68 |
| G-GPE / G-GMD | `T.V.11.*`, `T.V.14.*` | US_CCSS_HS |
| N-VM (+) vectors/matrices bridge | `T.VII.1.*`, `T.VII.3.*` | US_CCSS_HS |
| S-MD expected value decisions | `T.IV.14.*` | US_CCSS_HS, AP_STATS |
| AP Calc FRQ justification | `T.VI.1–6.*`, `T.VI.3.*` practice packs | AP_CALC_AB/BC |
| Euler / logistic / slope fields | `T.VI.7.*` | AP_CALC_AB |
| Series tests battery | `T.VI.9.*` | AP_CALC_BC |
| Taylor error bounds | `T.VI.10.*` | AP_CALC_BC |
| Polar/parametric FRQ | `T.VI.8.*` | AP_CALC_BC |
| AP Stats procedures (z/t/χ²/slope) | `T.VI.11.*` | AP_STATS |
| Study design / bias / simulation inference | `T.VI.11.*`, `T.III.9.*` | AP_STATS |

---

## File

- Machine JSON: [`testing-skills-1000.json`](./testing-skills-1000.json)
- Profile spec: [`exam-mode-profile-spec.md`](./exam-mode-profile-spec.md)
