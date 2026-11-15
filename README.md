# QEERI internship — evidence-led agricultural feasibility and LLM evaluation

**Status:** preliminary research and engineering documentation; scientific results and final direction pending mentor review. **Reviewed through:** 15 November 2026.

This repository is a **public, selected documentation record**, not the complete QEERI internship archive, official lab notebook, approved greenhouse design, finished benchmark, or validated commercial product. It deliberately excludes private mentor correspondence, restricted publications, unpublished institutional data, original full-text PDFs, and raw archives.

## What is actually established
- A Qatar-focused literature review with a proposed Al-Shahaniya tomato greenhouse reference case. The case is **not** an instrumented or approved site.
- Study comparisons from Shannak et al. 2026 (Tables 14–15), cooling principles from UF/IFAS AE069, and transfer limits for the Al Khor greenhouse paper.
- A reproducible **illustrative** pad-outlet calculation: dry bulb 38 °C, wet bulb 24 °C, effectiveness 0.85 → 26.1 °C at the pad outlet, **not** at crop height.
- Distinct prototype components: source-linked greenhouse demonstration; local SQLite/FTS5 retrieval and provenance; standalone case-validation/decision contract. **Not verified as a single integrated system.**
- Experimental method proposals and a two-week activity record; no verified on-site hours, mentor-approved final research verdict, or completed controlled multi-model comparison.

## Navigate
| Path | Purpose |
|---|---|
| [01_SCOPE_AND_HISTORY.md](01_SCOPE_AND_HISTORY.md) | Original mandate, 5 Nov scope evolution, research truth states |
| [02_SCIENTIFIC_EVIDENCE.md](02_SCIENTIFIC_EVIDENCE.md) | Narrow findings, source classes, numbers, missing data |
| [03_LLM_FEASIBILITY_PROTOCOL.md](03_LLM_FEASIBILITY_PROTOCOL.md) | Falsifiable comparison design, not fabricated results |
| [04_ENGINEERING_EVIDENCE.md](04_ENGINEERING_EVIDENCE.md) | Existing code/PRs, test observations and reproducibility boundaries |
| [05_IMPLEMENTATION_DIRECTION.md](05_IMPLEMENTATION_DIRECTION.md) | Proposed beyond-LLM architecture, decision gates and milestones |
| [06_PRESENTATIONS_AND_DELIVERABLES.md](06_PRESENTATIONS_AND_DELIVERABLES.md) | What the completed slide decks and reports mean |
| [07_TWO_WEEK_ACTIVITY_LOG.md](07_TWO_WEEK_ACTIVITY_LOG.md) | Nov 1–14 work grouped by week, **not attendance hours** |
| [08_REVIEW_DECISIONS.md](08_REVIEW_DECISIONS.md) | Exact decisions requested of mentors |
| [09_RESEARCH_REVIEW_PROMPTS.md](09_RESEARCH_REVIEW_PROMPTS.md) | Compact reusable evidence-audit prompts |

## Actual code — separate repository
[qeeri-agricultural](https://github.com/leadingproblemsolver/qeeri-agricultural)
- [PR #2: local RAG prototype](https://github.com/leadingproblemsolver/qeeri-agricultural/pull/2) — draft, not merged.
- [PR #4: 10-case greenhouse demonstration](https://github.com/leadingproblemsolver/qeeri-agricultural/pull/4) — draft, not merged.

## Non-claims
No confirmed field dataset, greenhouse investment return, crop-zone temperature, independent agronomic validation, AI/RAG gain, trained model, complete 50 × 4 model result set, or functioning integrated deployment.

The central position is **test whether deterministic checks plus a governed source register provide a safer and simpler decision boundary**; use LLMs only where a measured benefit justifies them. This is a proposed engineering direction, **not** an experimental superiority verdict.

**Access and reuse:** This public summary does not grant reuse rights to external papers, mentor materials, institutional research data, or source code beyond its own repository license (if any).