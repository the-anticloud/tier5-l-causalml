# HF_Leaderboard_Lab_Results

**Project:** `L_CAUSALML`  
**Tier:** `TIER_5_WORLD_NEURO_EMBODIED`  
**Slug:** `uber/causalml`  
**Commit:** `9a2327811406`  
**Run:** `2026-09-30T15:07:07.146295+00:00`  

## Isolation Environment

| Field | Value |
| ----- | ----- |
| Platform | `win32` |
| Python | `3.12.10` |
| HF model | `distilbert-base-uncased` |
| HF load time | `4.42s` |
| Inference device | `cpu` |

## Results

**Framework:** [HuggingFace Open LLM Leaderboard (proxy via distilbert-base-uncased)](https://huggingface.co/docs/leaderboards/en/open_llm_leaderboard/archive)

**Model used:** `distilbert-base-uncased`

### Inference Latency (Classification)

| Metric | Value |
| ------ | ----- |
| Avg latency | **43.06 ms** |
| Min latency | 38.53 ms |
| Max latency | 46.25 ms |
| Samples | 5 |

### Real Tokenization Results

| Field | Value |
| ----- | ----- |
| Token count | **36** |
| Tokenization latency | 1.0 ms |
| Classification label | `LABEL_0` |
| Classification score | 0.5859 |
| Classification latency | 116.96 ms |
| Status | **PASS** |

**Input text tokenized:**
```
L_CAUSALML (uber/causalml) — 250 files, 41771 source lines, licence Apache-2.0, primary language ['Python']
```

**First 20 tokens:**
```
['[CLS]', 'l', '_', 'causal', '##ml', '(', 'uber', '/', 'causal', '##ml', ')', '—', '250', 'files', ',', '417', '##7', '##1', 'source', 'lines']
```

> Full MMLU/HellaSwag/TruthfulQA/ARC/Winogrande/GSM8K require dedicated GPU.
> These results are CPU inference proxy metrics using distilbert-base-uncased.

---
_Anticloud Benchmark Suite — isolation log — 2026-09-30T15:07:07.146295+00:00_