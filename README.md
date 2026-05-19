# SIDE-yang-mills-formation v0.1

Kernel encoding of Yang-Mills as a formation-determined system. The Clay Millennium mass-gap problem reread as a domain Ostrowski for the n₃ output stage.

## Status

| | |
|---|---|
| Toolchain | `leanprover/lean4:v4.29.0-rc8` |
| Mathlib | not required |
| sorry | 0 |
| axioms | 0 |

Companion: `SIDE-formation-procedure v0.2`, `SIDE-structural-error-correction`, `ARITHMETIC_ORIGIN_STEANE_CODE_v3.md`, `MATTER_AS_ARITHMETIC_v1_0_CONSOLIDATED.md`.

## The structure

**Formation tuple (3, 3, 2, 0) = 8:**
- n₁ = 3: gauge symmetry, Lorentz symmetry, quantization
- n₂ = 3: Ostrowski places of ℚ
- n₃ = 2: mass gap + asymptotic freedom
- n₄ = 0: gauge invariance dark for color content

**Derived parameters:**
- S = 3 non-dark stages
- d_eff = 2S − 1 = 5 (Tightness Theorem for k = 1)
- Formation code: [[8, 1, 5]] on AG(3, 𝔽₂)

**Geometric realization:** AG(3, 𝔽₂), the full eight elements of (ℤ/2)³. ξ(s) lives on PG(2, 𝔽₂) — the seven non-zero elements. The extra point is the origin = trivial character = quantization.

**TECHNE TYPE II:** specified, closed, but mass-gap classification missing means partially enumerable. Impossibility sub-type II-D (specific dark interface at the output stage).

**Promotion path:** Yang-Mills becomes TYPE I when two domain Ostrowskis are supplied — classification of independent algebraic primitives in SU(N), and the mass-gap classification theorem. Solving the Clay Millennium mass-gap problem IS supplying the second domain Ostrowski.

## What's verified

### §1–§2 — Formation tuple and non-dark count
- `yang_mills_total_eight`: total = 8
- `S_equals_three`, `S_counts_non_dark`

### §3 — Formation distance
- `d_eff_equals_five`: d_eff = 2S − 1 = 5
- `tightness_applies_yang_mills`: k = 1 ⇒ tightness

### §4 — Steane-style formation code
- `yang_mills_code_consistent`: [[8, 1, 5]]

### §5 — Geometric realization
- `cubit_eight`, `trivium_seven`, `yang_mills_eight_geom`
- `yang_mills_extra_point`: AG(3, 𝔽₂) = PG(2, 𝔽₂) ∪ {origin}
- `extra_point_matches_extra_dimension`

### §6 — TECHNE TYPE II classification
- `yang_mills_TYPE_II`
- `yang_mills_specified`, `yang_mills_closed`, `yang_mills_not_enumerable`

### §7 — Impossibility sub-type
- `yang_mills_subtype_II_D`: II-D (specific dark interface)

### §8 — Mass gap as silence boundary
- `silence_boundary_at_output_stage`: stage 3

### §9 — Comparison with ξ(s)
- `yang_mills_vs_xi`: same n₂, n₃, n₄; n₁ differs by 1
- `yang_mills_total_eq_xi_plus_one`: 8 = 7 + 1
- `quantization_is_one`: the extra dimension is quantization

### §10 — Substrate class (gauge)
- Gauge class encoded with formation tuple, exclusion 18.6σ, not selected
- Arithmetic class encoded with exclusion 0.13σ, selected
- `yang_mills_matches_gauge_class`

### §11 — Universal Darkness Verification
- `yang_mills_universal_darkness`: n₄ = 0

### §12 — Promotion path
- `promoted_becomes_TYPE_I`
- `promotion_preserves_tuple`: tuple, d_eff, code unchanged

### §13 — Mass gap as domain Ostrowski
- `mass_gap_equals_n3_certification`: the Clay problem IS the n₃ domain Ostrowski

### §14 — Falsification routes
- Four routes catalogued

## Build

```bash
lake build
```

Self-contained — no Mathlib.

## Federation context

| Kernel | Role |
|---|---|
| **SIDE-yang-mills-formation** | **Yang-Mills as TECHNE TYPE II with promotion path** |
| SIDE-kernel | The reference TYPE I system (ξ(s)) — same n₂, n₃, n₄, lower n₁ |
| SIDE-formation-procedure v0.2 | The TECHNE classification machinery |
| SIDE-structural-error-correction | The d_eff = 2S − 1 tightness theorem |
| SIDE-silence-principle | The n₄ = 0 dark interface foundation |
| SIDE-steane-arithmetic | The Steane code arithmetic; Yang-Mills [[8, 1, 5]] adjacent to Steane [[7, 1, 3]] |

## License

CC-BY 4.0.

> Seale, J. Y. (2026). *SIDE-yang-mills-formation v0.1: Yang-Mills as a Formation-Determined System.* A PLACE TO STAND Research Programme.

---

`:: → · ← ::`

*The mass gap is the silence boundary. The Clay problem is the domain Ostrowski for n₃.*
