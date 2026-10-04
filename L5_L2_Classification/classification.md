# L5 Narrow / L2 General Classification — L_CAUSALML
**Platform:** Anticloud | **Tier:** TIER_5_WORLD_NEURO_EMBODIED | **PAX:** 27B
**IP:** USPTO pending 2026, Anticloud FZ LLE, 0-1.gg | **License:** Apache-2.0

## L5 Narrow
L_CAUSALML applies causal inference methods (do-calculus, propensity scoring, counterfactual analysis) to Anticloud AI decisions. Narrow scope: causal analysis of AIOSS-chained outputs — why did PAX 27B produce this response given this context?

## L2 General
L2 General: L_CAUSALML's causal explanations improve auditability across all tiers. Clinical AI decisions and security alert classifications both benefit from causal explanations.

## PAX 27B Integration
PAX 27B is used to generate causal hypotheses that L_CAUSALML then tests with formal causal inference methods. The combination produces human-readable causal explanations that are formally valid.

## AIOSS Audit Chain
Every causal analysis (treatment variable hash + outcome hash + causal graph hash + ATE estimate + confidence intervals) is chained: H_n = SHA3-256(H_{n-1} || entry_hash_n || timestamp_n).
Offline-verifiable, tamper-evident, zero cloud dependency.

## Regulatory / Compliance
NIST AI RMF 1.0 (explainable AI decisions). EU AI Act Art. 13 (transparency).
