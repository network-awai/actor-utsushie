# utsushie 写し絵 — Maturity

**Stage: R0** (design scaffold) — created 2026-06-16 per ADR-2606161536 §D2.

| Dimension | State |
|---|---|
| Lexicon | ✅ `lex/video.edn` — `com.etzhayyim.utsushie.video` with U1–U6 structural gates |
| Methods | ✅ `src/utsushie/methods/render_plan.cljk` — offline, pure, deterministic plan builder + R0-gated `render()` |
| Tests | ✅ Clojure/EDN suite via `kbb -M -e '(load-file "run_tests.cljk")'` |
| Cells | ✅ dry-run social-post membrane; live publication remains R1-gated |
| Manifest | ✅ canonical `manifest.edn`; legacy JSON-LD is external wire only |
| Render | ⛔ R0-gated (G8 + Murakumo-only, U5 = G6) — `render()` raises by design |
| Publish | ⛔ R1 — i18n scripts (D3) + feed-post membrane (D4), member-signed (U6 = G7) |

## R0 → R1 gate

R1 lift requires: Council Lv6+ + operator (G8), Murakumo-fleet render capacity decided
(ADR-2606161536 C1), and the kawaraban `:article` derivation (D1) landed upstream.
