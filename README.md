# 1000+ Predictor

Standalone Oracle v5.0 football-odds pattern predictor.

- 1,200 deterministic reference profiles expanded from the supplied archive patterns
- market-implied probability and bookmaker-margin calculation
- nearest-neighbour pattern comparison
- consensus, trap, fatigue and injury checks
- optional double-chance selection and capped 2% staking suggestion
- additive secondary-results predictor trained on 48 completed probability/score rows
- automatic transfer of the mother predictor's Home/Draw/Away percentages into the secondary engine

The mother predictor logic remains unchanged. The third cross-check receives the secondary engine's **output** Home/Draw/Away percentages, rather than its mother-percentage inputs. It uses 23 usable percentage/actual-score records (one red-card match excluded). A result can be named when at least three close examples agree by 75%, or when an exact pattern and at least one other close outcome agree. An exact match is displayed with its recorded score as evidence, not a promised score. If the third result differs from the secondary result, the page flags disagreement and SKIP. The bars always show distance-weighted Home/Draw/Away shares of seven nearest records, not calibrated forecast probabilities. The 1,200 reference profiles are synthetic variations, not 1,200 distinct completed games.

Predictions are estimates and are not guaranteed.
