# Public Codebook and Data-Schema Template

## Important limitation

This is a public, non-identifying schema for the analysis template—not the final confidential study codebook. Variable names, item membership, scale direction, response ranges, reverse coding, missing-value codes, and exclusion rules must be verified against the original research documentation before real-data analysis.

## Study-level information

| Component | Confirmed count | Public availability |
|---|---:|---|
| Quantitative survey | N = 119 | Participant-level data not public |
| Qualitative interviews | n = 19 | Transcripts and coding materials not public |

## Demonstration variables

| Variable | Type | Example range/levels | Role in template | Status |
|---|---|---|---|---|
| `participant_id` | Character | `SIM001`–`SIM119` | Synthetic row identifier | Demonstration only; never publish real IDs |
| `age` | Numeric | 18–55 | Example covariate | Definition/range to verify |
| `attachment_group` | Factor | `lower`, `higher` | Example ANOVA grouping variable | Derivation/cut point to replace |
| `attachment_anxiety_1`–`attachment_anxiety_4` | Numeric items | 1–7 | Example reliability/EFA inputs | Names, item count, keys, and range to verify |
| `rumination_1`–`rumination_3` | Numeric items | 1–5 | Example reliability/EFA inputs | Names, item count, keys, and range to verify |
| `attachment_anxiety` | Numeric score | Mean of example items | Example composite predictor | Scoring rule to replace |
| `rumination` | Numeric score | Mean of example items | Example composite outcome/predictor | Scoring rule to replace |
| `adjustment_score` | Numeric | Unspecified | Example regression outcome | Construct and scoring to replace |

## Confirmed statistical facts

| Analysis | Confirmed value/conclusion | Details still needed before reporting |
|---|---|---|
| KMO | .812 | Exact item set, correlation choice, per-item MSA |
| Reliability | Cronbach's alpha = .891 | Scale name, item set, standardized/raw alpha |
| ANOVA | Attachment anxiety and rumination showed a significant relationship | Model specification, F, df, p, effect size, assumptions, group definition |

## Qualitative component

The project included 19 interviews. The public repository intentionally contains no transcripts, quotations, participant attributes, code-level excerpts, or themes that have not been confirmed for public reporting.

## Final-data verification checklist

- Confirm instrument and subscale names.
- Confirm every item-to-scale mapping and reverse-keyed item.
- Confirm valid response ranges and missing-value codes.
- Confirm inclusion/exclusion and duplicate-handling rules.
- Confirm how attachment anxiety enters the ANOVA (continuous score, categories, or another specification).
- Reproduce KMO = .812 and alpha = .891 from the authorized analysis file.
- Add exact ANOVA statistics only after checking the original output.
- Document regression outcomes only if supported by verified results.
- Remove direct and indirect identifiers from every exported artifact.
