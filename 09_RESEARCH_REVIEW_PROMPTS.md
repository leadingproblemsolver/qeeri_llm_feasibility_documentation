# Research review prompt pack — public-safe condensed version

These prompts are documentation aids, **not proof** that an LLM or a project is scientifically valid.

## 1. Ground-truth audit
> Given named project files, commands and output records, separate (a) artifacts that were opened/run, (b) claims not evidenced by those artifacts, and (c) the single highest-consequence missing test. Quote exact paths and refuse to infer unseen results.

## 2. Adversarial domain check
> Check physical boundary conditions, units, contradictions, circular assumptions, transferability, and original-source passage support. Score software reproducibility separately from scientific correctness. Do not prescribe fixes until observed defects are listed.

## 3. First-principles reduction
> State the single load-bearing claim; the minimum independent evidence required; the explicit falsification condition; and everything else that is optional packaging.

## 4. Dual review
> Produce separate (a) domain-expert and (b) external methods-auditor objections. Identify the single disagreement that should be sent to a real reviewer.

## 5. Presentation receipts
> For each slide record: on-screen claim and units, precise citation/source class, 15–25 spoken words, and observed executable/demo receipt or PENDING. Do not render unavailable data as measured charts.

## 6. Publication gate
> In four one-line answers: what exists, what it establishes, what would falsify it, and what is still unverified. Do not turn proposed tests into experimental results.

**Common failure:** a correctly cited equation or passing unit test does not prove its application to a particular greenhouse or demonstrate LLM performance.