# Developer Cookbook — L_CAUSALML
**Stack:** Python 3.11, causalml 0.x, DoWhy, PAX 27B, AIOSS_FORMAT
**Domain:** CausalML: causal inference and counterfactual reasoning for Anticloud AI

## Causal analysis of AI decision
```python
from l_causalml import CausalAnalyzer

analyzer = CausalAnalyzer(
    pax_model="./pax-27b-q4.gguf",
    aioss_chain="./causalml.aioss"
)

# Why did PAX flag this biosignal as anomalous?
result = analyzer.explain(
    decision_chain_entry="./audit.aioss",
    entry_index=142,
    treatment="high_theta_power",
    outcome="seizure_flag"
)
print(f"ATE: {result.ate:.3f} (p={result.p_value:.4f})")
print(f"Causal explanation: {result.natural_language_explanation}")
```

## Counterfactual
```python
cf = analyzer.counterfactual(
    entry_index=142,
    counterfactual_intervention={"high_theta_power": False}
)
print(f"Without high theta: seizure_flag would be {cf.counterfactual_outcome}")
```

## AIOSS Chain Append
```python
import hashlib, time

def aioss_append(chain_path, payload: bytes, module_id: str):
    entry_hash = hashlib.sha3_256(payload).digest()
    ts = int(time.time_ns()).to_bytes(8, 'big')
    with open(chain_path, 'rb') as f:
        f.seek(-32, 2); prev_hash = f.read(32)
    new_hash = hashlib.sha3_256(prev_hash + entry_hash + ts).digest()
    with open(chain_path, 'ab') as f:
        f.write(ts + entry_hash + new_hash)
    return new_hash.hex()
```
