# Radon_Complexity_Lab_Results
**Project:** `L_CAUSALML` | **Status:** `PASS` | **Run:** `2026-09-30T17:14:20.030944+00:00`

**Framework:** [Radon — Cyclomatic Complexity & Maintainability Index](https://radon.readthedocs.io/)

## Key Metrics

- **files_analyzed:** `10`
- **average_complexity:** `{'grade': 'A', 'score': 2.9464285714285716}`
- **complexity_grade:** `A`
- **complexity_score:** `2.9464285714285716`
- **mi_output:** `E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_CAUSALML\UPSTREAM\setup.py - A (76.74)
E:\fenta\Downloads`

## Raw Output (first 50 lines)
```
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_CAUSALML\UPSTREAM\causalml\exceptions.py
    F 1:0 handle_xgboost_error - A (2)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_CAUSALML\UPSTREAM\causalml\features.py
    F 237:0 load_data - C (12)
    M 193:4 OneHotEncoder.transform - A (5)
    C 136:0 OneHotEncoder - A (3)
    C 13:0 LabelEncoder - A (2)
    M 36:4 LabelEncoder._get_label_encoder_and_max - A (2)
    M 79:4 LabelEncoder.fit - A (2)
    M 91:4 LabelEncoder.transform - A (2)
    M 106:4 LabelEncoder.fit_transform - A (2)
    M 160:4 OneHotEncoder._transform_col - A (2)
    M 24:4 LabelEncoder.__init__ - A (1)
    M 33:4 LabelEncoder.__repr__ - A (1)
    M 67:4 LabelEncoder._transform_col - A (1)
    M 147:4 OneHotEncoder.__init__ - A (1)
    M 157:4 OneHotEncoder.__repr__ - A (1)
    M 188:4 OneHotEncoder.fit - A (1)
    M 222:4 OneHotEncoder.fit_transform - A (1)
E:\fenta\Downloads\The Anticloud\TIER_5_WORLD_NEURO_EMBODIED\L_CAUSALML\UPSTREAM\causalml\match.py
    M 146:4 NearestNeighborMatch.match - C (13)
    M 377:4 MatchOptimizer.check_table_one - C (12)
    M 447:4 MatchOptimizer.search_best_match - C (11)
    C 84:0 NearestNeighborMatch - B (6)
    C 294:0 MatchOptimizer - B (6)
    F 34:0 create_table_one - A (3)
    M 432:4 MatchOptimizer.match_and_check - A (2)
    F 14:0 smd - A (1)
    M 115:4 NearestNeighborMatch.__init__ - A (1)
    M 271:4 NearestNeighborMatch.match_by_group - A (1)
    M 295:4 MatchOptimizer.__init__ 
```

---
_Anticloud Independent Benchmark — 2026-09-30T17:14:20.030944+00:00_