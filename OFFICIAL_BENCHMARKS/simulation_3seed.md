# 3-Seed Simulation — L_CAUSALML

**Seeds:** `9795` · `41132` · `75331`

**Seed method:** `sha256("L_CAUSALML")[:8]` as hex→int, offsets +0 / +31337 / +65536

> These seeds are deterministic and documented. Any researcher can reproduce this simulation exactly by running `write_three_seed_simulation.py` with project name `L_CAUSALML`.

## Confidence Intervals (mean ± σ across 3 seeds)

| Metric | Mean | σ | 95% CI |
|--------|------|---|--------|
| trl_score | 7.0637 | 0.0151 | ±0.0296 |
| throughput_tokens_per_sec | 889.8667 | 25.7858 | ±50.5402 |
| p50_latency_ms | 47.01 | 4.6103 | ±9.0362 |
| p99_latency_ms | 109.2167 | 1.5085 | ±2.9567 |
| ttft_ms | 27.66 | 1.4142 | ±2.7718 |
| mmlu_proxy | 0.7626 | 0.0 | ±0.0 |
| hellaswag_proxy | 0.7606 | 0.0303 | ±0.0594 |
| truthfulqa_proxy | 0.5425 | 0.0146 | ±0.0286 |
| arc_proxy | 0.7158 | 0.0159 | ±0.0312 |
| complexity_cyclomatic | 4.7733 | 0.0377 | ±0.0739 |
| maintainability_index | 74.2633 | 4.1342 | ±8.103 |
| security_issues_high | 0.6667 | 0.9428 | ±1.8479 |
| dependency_freshness_pct | 73.4 | 2.5456 | ±4.9894 |
| test_coverage_pct | 60.7333 | 0.2357 | ±0.462 |
| doc_coverage_pct | 64.5333 | 2.3099 | ±4.5274 |
| memory_mb | 410.0667 | 13.9064 | ±27.2565 |
| gpu_util_pct | 64.3667 | 6.7411 | ±13.2126 |
| openssf_score | 6.78 | 0.3394 | ±0.6652 |
| eu_ai_act_compliance_pct | 84.7667 | 0.5185 | ±1.0163 |
| slsa_level | 2.0 | 0.0 | ±0.0 |

## Per-Seed Raw Results

| Metric | Seed 9795 | Seed 41132 | Seed 75331 |
|--------|------------|------------|------------|
| trl_score | 7.053 | 7.085 | 7.053 |
| throughput_tokens_per_sec | 908.1 | 853.4 | 908.1 |
| p50_latency_ms | 50.27 | 40.49 | 50.27 |
| p99_latency_ms | 108.15 | 111.35 | 108.15 |
| ttft_ms | 26.66 | 29.66 | 26.66 |
| mmlu_proxy | 0.7626 | 0.7626 | 0.7626 |
| hellaswag_proxy | 0.7392 | 0.8035 | 0.7392 |
| truthfulqa_proxy | 0.5528 | 0.5219 | 0.5528 |
| arc_proxy | 0.7271 | 0.6933 | 0.7271 |
| complexity_cyclomatic | 4.8 | 4.72 | 4.8 |
| maintainability_index | 71.34 | 80.11 | 71.34 |
| security_issues_high | 0 | 2 | 0 |
| dependency_freshness_pct | 71.6 | 77.0 | 71.6 |
| test_coverage_pct | 60.9 | 60.4 | 60.9 |
| doc_coverage_pct | 62.9 | 67.8 | 62.9 |
| memory_mb | 419.9 | 390.4 | 419.9 |
| gpu_util_pct | 59.6 | 73.9 | 59.6 |
| openssf_score | 7.02 | 6.3 | 7.02 |
| eu_ai_act_compliance_pct | 84.4 | 85.5 | 84.4 |
| slsa_level | 2 | 2 | 2 |

---
_Anticloud 3-Seed Simulation — 2026-09-30T16:01:40.704491+00:00_
_Citation: Lois-Kleinner. (2026). The Anticloud. DOI: pending._