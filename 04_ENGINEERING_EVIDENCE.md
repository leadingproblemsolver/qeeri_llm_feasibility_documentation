# Technical implementation evidence — separate components, explicit limits

Main code: [leadingproblemsolver/qeeri-agricultural](https://github.com/leadingproblemsolver/qeeri-agricultural).

## Existing artifacts
**Draft PR #4**: a greenhouse demonstration with `demo/greenhouse/` containing `cases.yaml`, `check_cases.py`, `overview.md`, `qeeri_evidence.yaml`, `run_demo.py`. It exposes ten example checks and evidence/scope warnings. **10/10** demo checks were reported in the local 13 Nov verification. Demonstration checks are internal data-contract consistency checks, not peer-reviewed agricultural validation.

**Draft PR #2**: Python/SQLite FTS5 local RAG with allowlists, provenance, source hashes, bounded output controls, receipts, evaluator scaffolding, tests. A Windows PowerShell/Python environment reported **75 tests, 73 passing and two errors** linked to SQLite/temporary-directory paths. Calling both errors *proven environment-only* would overreach; root-cause fix and rerun remain pending. Repository historical CI reports a distinct earlier passing run. The actual model A/B/C evaluation is **NOT_EXECUTED**.

**Standalone integration contract ZIP**: a separate `integration.py` program with **9/9 locally reported tests**, hash checks, an illustrative 26.1 °C case and a fail-closed invalid psychrometric input. Verifications reported: archive SHA-256 `c8c1643f35e58abadeb26d8d8d4283f9b314cfe3bb8717119c99685055b5b21f`; `integration.py` SHA-256 `bae81fc153978b65f63f762237ee29645848fa34e1a851b271895910193722c7`; deterministic decision hash `372522249f4b5451487b1cc6c64a23bdae10a465ef6732596c53837f5d3736f8`. These were reported from a local verification transcript and have not been independently re-run from GitHub in this documentation repository.

## Known unclosed issues
- PR #2, PR #4 and standalone `integration.py` **not connected** end to end; no final production UI/deployment.
- Source-verification states differ between demo and retrieval corpus; **never promote** a 'verified' label from one register into human scientific sign-off.
- FAO-exclusion inconsistency appears in RAG allowlist: reconcile before scientific use.
- Citation-resolution checks do not establish semantic entailment.
- No verified site data; no calibrated crop prediction or construction readiness.
- No controlled model-versus-fixed-packet-versus-RAG improvement result.

## Exact developer reproduction entry
```bash
git clone https://github.com/leadingproblemsolver/qeeri-agricultural.git
cd qeeri-agricultural
git fetch origin pull/4/head:greenhouse-demo
git switch greenhouse-demo
python -m pip install pyyaml
python demo/greenhouse/run_demo.py
```

For the separate RAG branch:
```bash
git fetch origin pull/2/head:rag-prototype
git switch rag-prototype
cd research/qeeri_rag_v0
python -m unittest discover -s tests -v
python evidence/demo.py
```
**Record new observed results; do not assume previously observed counts will match.**

An earlier integration plan mistakenly copied only two of five demonstration files. The full `demo/greenhouse/` directory is the dependency-correct unit. This is a documented **plan defect**, not proof of an integration defect.