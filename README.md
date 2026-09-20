# 1000+ Predictor

Standalone Oracle v5.0 football-odds pattern predictor.

- 301 deduplicated real odds/outcome records in the expanded decision archive
- 1,200 deterministic mother-reference profiles expanded from 100 supplied seed patterns
- market-implied probability and bookmaker-margin calculation
- nearest-neighbour pattern comparison
- consensus, trap, fatigue and injury checks
- optional double-chance selection and capped 2% staking suggestion
- additive secondary-results predictor trained on 48 completed probability/score rows
- automatic transfer of the mother predictor's Home/Draw/Away percentages into the secondary engine

The mother predictor logic remains unchanged. The third cross-check receives the secondary engine's **output** Home/Draw/Away percentages, rather than its mother-percentage inputs. It uses 23 usable percentage/actual-score records (one red-card match excluded). A result can be named when at least three close examples agree by 75%, or when an exact pattern and at least one other close outcome agree. An exact match is displayed with its recorded score as evidence, not a promised score. If the third result differs from the secondary result, the page flags disagreement and SKIP. The bars always show distance-weighted Home/Draw/Away shares of seven nearest records, not calibrated forecast probabilities. The 1,200 reference profiles are synthetic variations, not 1,200 distinct completed games.

Predictions are estimates and are not guaranteed.

## Unified safety and validation layer

The site now includes a validation-locked unified decision. It combines the no-margin bookmaker baseline with an expanded 301-match real-odds archive; the dependent secondary, third and fourth checks can contribute no more than 10% and receive no weight when they conflict.

The expanded archive recovers every valid odds-bearing source that was already embedded in the site: 168 clean score rows, 47 additional earlier-JPG score rows and 86 original seed outcomes not already represented by the same odds and result. Percentage-only third/fourth rows are not mixed into this archive because they do not contain bookmaker odds. The original mother predictor formula and its 1,200 generated reference profiles remain unchanged.

The expanded archive now uses three pre-defined odds bands based on the favourite's no-margin probability: Balanced below 42%, Moderate from 42% to below 55%, and Strong at 55% or above. A match is compared only with outcomes in the same band; the engine falls back to the global archive if a band has fewer than 30 records. The final formula remains 50% market baseline + 40% banded archive + 10% unanimous chain confirmation.

A leave-one-out diagnostic tests every clean archived match without using its own result. The current diagnostic does not demonstrate a positive flat-stake return, so the unified layer remains locked in `AVOID · RESEARCH MODE`. This is intentional: the interface must not present an unvalidated historical pattern as a wagering edge. The Real Results Tracker now also records the unified output so genuinely new matches can provide forward evidence.

The fourth predictor automatically reads the third predictor's output percentages and compares them with 56 distinct completed rows transcribed from two additional JPGs. One red-carded game and exact repeated rows are excluded. A candidate needs at least four outcomes within a 12-point Euclidean distance, a nearest row within 6 points, at least 75% of nearby outcomes for the side, at most 20% draws, and the two closest results on that side. Otherwise the output is AVOID MATCH. It never predicts a draw or an exact score. It shows distance-weighted Home, Draw risk, and Away percentages from seven nearest completed results even when the verdict is AVOID MATCH; these descriptive percentages are not calibrated forecasts. A small leave-one-out check did not establish reliable accuracy; a HOME/AWAY result is a pattern signal, not an assured outcome or a calibrated probability.
