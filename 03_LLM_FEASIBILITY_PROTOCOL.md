# Research proposal: do LLMs improve evidence-bound technical assessment?

**Research status: PROPOSED; NOT an executed controlled study.**

## Load-bearing question
Compared with a no-document LLM and a fixed evidence packet, does retrieval or a deterministic source gate improve *correctness, exact provenance, scope differentiation, and calibrated abstention* enough to justify its additional complexity?

## Existing preliminary observation
RC01 is a *small illustrative pad-calculation/protocol exercise*. One zero-shot correct answer **does not establish an RAG improvement or failure**; archived intervention branches may be marked skipped or not executed. The formal PR #2 RAG README explicitly reports **model A/B/C comparisons NOT_EXECUTED**; deterministic retrieval checks are not model-accuracy experiments.

## Proposed pilot — requires mentor approval
- **Case classes:** calculation, exact citation, source-class classification, underdetermination/refusal, conflicting sources and domain safety.
- **Arms:** A = no evidence packet; B = same model + frozen approved packet; C = same model + retrieval-selected approved passages; optional D = deterministic evidence/rules + constrained explanation.
- **Control:** freeze case inputs, version, prompts, tool state, generation settings, source hashes and recorded full outputs. Run comparable independent sessions.
- **Reference:** subject expert verifies the source passages/answer keys *before* model scoring.
- **Scoring:** numeric/semantic correctness; attribution; source-class/scope accuracy; refusal when information is absent; safety; practical usefulness. Rubric and veto failures to be fixed in advance.
- **Analysis:** paired per-question differences, error taxonomy and uncertainty; report small-sample limits and negative/null outcomes.
- **Reviewer:** blinded domain assessment where available; inter-rater method and acceptable thresholds must be decided by mentors.
- **Budget and schedule:** *not verified*. Do not quote previous speculative dollar estimates or IRB exemptions as facts.

## Falsification
RAG is **not justified** if it fails to outperform a fixed packet on the actual restricted tasks after accounting for costs, complexity and attribution errors. Deterministic gating is **not proven superior** without the same fair outcome-based comparison. A correct formula with absent site variables must result in an explicitly narrow answer, not a greenhouse recommendation.

## Go/no-go
Execute only a pre-registered bounded pilot when the case, source permissions, expert review and acceptance conditions are agreed. **Model training is not a current deliverable.**