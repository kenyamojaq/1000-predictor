# Clean master archive audit

The recoverable source contained 177 rows.

- 3 exact duplicate rows were removed.
- 5 red-card-annotated results were quarantined because those matches are not ordinary full-match comparisons.
- 1 suspicious row (`2.80, 3.25, 8.20, 1-1`) was quarantined rather than silently corrected.
- 168 clean, unique, ordinary completed matches remain in the score-complete master source.

The site also contained two older odds-bearing sources that were separate from that file:

- 48 earlier JPG rows, of which 47 add a new exact odds/score record after deduplication.
- 100 original mother seed rows, of which 86 add a new odds/result combination after excluding combinations already represented in the score-bearing data.

The resulting expanded real-odds archive contains **301 deduplicated completed outcomes**. Of these, 215 include an exact score and 86 retain only the known Home/Draw/Away result. The published export is `expanded-real-archive.csv`.

## Odds-band test

The original global archive test selected 91 of 301 matches, with 46 correct (50.5%) and a flat-stake result of -7.16 units. A simple pre-defined three-band model selected 90 matches, with 47 correct (52.2%) and -2.89 units. The bands are based on no-margin favourite probability: below 42%, 42–55%, and 55% or above. This is an improvement, but it is still negative, so the validation safety lock remains active.

Percentage-only third- and fourth-predictor rows are intentionally excluded from this odds archive. The source messages also contained repeated or malformed rows; they are not claimed as published unless they appear in `expanded-real-archive.csv`.

The mother predictor formula remains unchanged. The master archive is an independent decision gate and returns `AVOID MATCH` when nearby historical evidence is insufficient or inconsistent.
