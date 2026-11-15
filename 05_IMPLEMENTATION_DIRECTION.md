# Implementation decision — beyond an LLM-first feasibility advisor

## Current position, not a published superiority claim
**Prefer to investigate a deterministic, source-register-gated decision workflow with optional LLM explanation.** The scientific reference remains the authority; the model cannot approve itself, certify sources, estimate unavailable site conditions, or invent component sizing.

This is superior *as a risk-bounded engineering proposal* to leaving calculations, evidence status and consequential approval solely to free-form generation. **Empirical superiority is NOT established**, and mentor approval is pending.

## Smallest implementation path
1. **Structured intake:** crop, region, greenhouse configuration, user-provided climate/water/energy parameters and source identifiers; record units, evidence class and timestamp.
2. **Source register and storage:** approved passages, exact locators, verification state, exclusions, provenance SHA-256, persistent SQLite records.
3. **Deterministic calculations:** cooling-pad equation with physical validation and explicit scope; missing-critical-input behavior `BLOCK` or `REVIEW`.
4. **Decision guard:** check jurisdiction, evidence sufficiency, contradictions, unsafe sizing and reviewer approval. No automated construction or investment acceptance.
5. **Optional LLM:** explain only already-supported observations with traceable citations. Test against no-LLM and fixed-packet alternatives before integration.
6. **Receipt:** capture case input, version, source hashes, executed checks, decision, blocked/unknown fields and reviewer status.
7. **Human review:** mentor assesses one frozen scientific case and acceptance criteria before expanding to greenhouse equipment, water budgeting or costs.

## Falsifiable next experiment
Run the **same frozen cases** with (A) LLM alone, (B) LLM with fixed sources, (C) RAG and (D) deterministic gates with optional explanation; compare independently scored correctness, attribution, refusal/safety and implementation burden. A preselected conclusion would invalidate the purpose.

## Out of scope now
Model training, unrestricted agents, live sensor integration, clinical/safety certification, field greenhouse sizing, financial return forecasts, production business deployments. The current work is **engineering research and an unfinished integration**.