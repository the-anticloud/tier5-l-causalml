# Deploy Guide — L_CAUSALML
**Tier:** TIER_5_WORLD_NEURO_EMBODIED | **Stack:** Python 3.11, causalml 0.x, DoWhy, PAX 27B, AIOSS_FORMAT
**Air-gap capable after initial setup.**

## Prerequisites
Python 3.11+, causalml 0.15+, dowhy 0.11+, PAX 27B. CPU-intensive for causal graph estimation.

## Environment
16GB RAM for large causal graphs. CPU-heavy. GPU for PAX hypothesis generation.

## AIOSS Integration
```bash
aioss init --module L_CAUSALML --output ./l_causalml.aioss
aioss append --chain ./l_causalml.aioss --payload ./output.bin --module L_CAUSALML
aioss verify --chain ./l_causalml.aioss
```

## Air-Gap Setup
```bash
pip download -r requirements.txt -d ./wheels/
pip install --no-index --find-links ./wheels/ -r requirements.txt
```

## PAX 27B Harness Wiring
```python
from anticloud_pax import PAXHarness
harness = PAXHarness(
    model_path="./pax-27b-q4.gguf",
    module="L_CAUSALML",
    aioss_chain="./L_CAUSALML.aioss",
    classification="L5_NARROW_L2_GENERAL"
)
result = harness.process(input_data)
```

## Verification
```bash
aioss verify --chain ./L_CAUSALML.aioss --verbose
python -m L_CAUSALML.tests.smoke
```
