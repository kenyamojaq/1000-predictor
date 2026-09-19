# Clean master archive audit

The recoverable source contained 177 rows.

- 3 exact duplicate rows were removed.
- 5 red-card-annotated results were quarantined because those matches are not ordinary full-match comparisons.
- 1 suspicious row (`2.80, 3.25, 8.20, 1-1`) was quarantined rather than silently corrected.
- 168 clean, unique, ordinary completed matches remain in the published master archive.

The source messages contained additional pasted blocks, many of which repeated earlier rows or included malformed values. Those rows are not claimed as published unless they are present in `clean-master-archive.csv`.

The mother predictor formula remains unchanged. The master archive is an independent decision gate and returns `AVOID MATCH` when nearby historical evidence is insufficient or inconsistent.
