# 2025 CAS/JCR Journal Rank Tables by Letter

This folder contains GPT-friendly split CSV files for journal quality lookup.

## Files

- `A.csv` to `Z.csv`: journals grouped by the first normalized English letter.
- `OTHER.csv`: journals whose normalized name does not start with A-Z.

## Columns

```text
Journal
Journal_Normalized
CAS2025_Quartile
CAS2025_Top
JCR_BestQuartile
```

## Matching rule

1. Confirm the official journal name from DOI/publisher page.
2. Normalize the journal name:
   - uppercase;
   - trim spaces;
   - treat `&` as `AND`;
   - ignore punctuation, hyphens, commas, periods, colons and extra spaces.
3. Open the corresponding first-letter CSV.
4. Match `Journal_Normalized` first; if difficult, match `Journal`.
5. Read `CAS2025_Quartile`, `CAS2025_Top`, and `JCR_BestQuartile`.

## Source

Generated from uploaded `CAS_2025.csv` and `JCR_2025.csv`.

## Record counts

{
  "A": 2442,
  "B": 871,
  "C": 2038,
  "D": 420,
  "E": 1392,
  "F": 578,
  "G": 485,
  "H": 497,
  "I": 2149,
  "J": 3768,
  "K": 142,
  "L": 427,
  "M": 1004,
  "N": 657,
  "O": 331,
  "P": 1350,
  "Q": 98,
  "R": 1157,
  "S": 1277,
  "T": 716,
  "U": 116,
  "V": 212,
  "W": 232,
  "X": 4,
  "Y": 23,
  "Z": 130,
  "OTHER": 11
}


## Note

This version removes the original `Journal` column from all CSV files. Use `Journal_Normalized` as the only journal-name matching key.
