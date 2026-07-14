# Data contract

The original field dataset is not included in this public repository.

To run the Notebook, place an authorized Excel workbook at:

```text
data/raw/Data_all_forblindtest.xlsx
```

Expected columns:

```text
well_ind, DEPTH, DT, ZDEN, GR, CNCF, M2RX, POR, PERM, SW, PROD
```

- `well_ind`: well identifier used for grouped/blind-well analysis
- `PROD`: depth-segment production target in m3/d
- Remaining columns: depth, logging, petrophysical, and saturation predictors

Remove or anonymize field identifiers and verify data-sharing permissions before adding any dataset to a public release.
