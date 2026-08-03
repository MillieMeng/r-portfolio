# 📈 R Portfolio — Behavioral Data Analysis

[![R](https://img.shields.io/badge/R-tidyverse%20%7C%20ggplot2-276DC3?style=flat-square&logo=r&logoColor=white)](https://github.com/MillieMeng/r-portfolio)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen?style=flat-square)](https://github.com/MillieMeng/r-portfolio)

Three R analysis projects spanning behavioral data pipelines, predictive modeling, and psychometric research. All projects are documented in RMarkdown with reproducible workflows.

---

## 01 · Cognitive Control — Flanker Task Pipeline

### Overview
End-to-end data pipeline processing 8,000+ trial-level observations from a Flanker cognitive control experiment. Automates per-participant visualization and response-time modeling across congruent and incongruent conditions.

### Business Question
> How do cognitive load conditions affect response-time performance, and which participants show the strongest interference effects?

### Method
- Cleaned and restructured raw trial-level data using `dplyr`
- Built reusable `ggplot2` functions for automated per-participant visualization
- Modeled response-time and error-rate trends using LOESS regression
- Documented end-to-end in RMarkdown for reproducibility

### Results
- Identified consistent response-time elevation under incongruent (high-interference) conditions across participants
- Automated pipeline eliminates manual per-participant processing — scales to any sample size
- LOESS smoothing revealed individual variation in interference magnitude not captured by group-level averages

### Skills
`tidyverse` · `dplyr` · `ggplot2` · `LOESS regression` · `RMarkdown` · data wrangling · automated visualization

---

## 02 · Predictive Modeling — Attachment & Mental Health

### Overview
Multiple regression model predicting mental health outcomes from attachment-related variables using archival survey data (N = 473). Full assumption testing reported in APA format.

### Business Question
> Which attachment-related variables predict psychological wellbeing, and how much variance can a linear model explain?

### Method
- Multiple regression on N = 473 archival survey responses
- Full assumption testing: normality (Shapiro-Wilk), homoscedasticity (Breusch-Pagan), multicollinearity (VIF), outlier detection (Cook's D)
- Two-way ANOVA and independent samples t-test for group comparisons
- Effect sizes (Cohen's d, η²) reported throughout

### Results
- Final model: R² = .31 — attachment variables explain 31% of variance in psychological adjustment
- All key assumptions met; model diagnostics documented and interpreted
- Effect sizes indicate medium-to-large practical significance for primary predictors

### Skills
`multiple regression` · `ANOVA` · `assumption testing` · `effectsize` · `RMarkdown` · APA reporting

---

## 03 · Social Cognition — Relationship Dissolution & Ghosting

### Overview
Mixed-methods psychometric study on psychological responses to ghosting (N = 119 survey + n = 19 interviews). See the [full repository](https://github.com/MillieMeng/relationship-dissolution-analysis) for complete documentation.

### Business Question
> What psychological mechanisms drive post-dissolution adjustment, and can they be reliably measured?

### Method
- Psychometric survey across four dimensions: rumination, self-worth doubt, trust erosion, confusion
- EFA to assess factorial validity; Cronbach's α and KMO/Bartlett for reliability
- Qualitative interviews coded into three thematic stages
- Privacy-conscious design: analysis defaults to reproducible simulated data

### Results
- High-reliability scale: α = .891, KMO = .812
- 62.9% scored ≥ 4 on rumination; psychological impact showed no significant correlation with ghosting duration
- Findings delivered as structured report to faculty stakeholder

### Skills
`EFA` · `psychometrics` · `psych` · `ggplot2` · `mixed-methods` · `RMarkdown` · privacy-conscious data handling

---

## Technical Stack

| Tool | Usage |
|---|---|
| `tidyverse` / `dplyr` | Data wrangling and transformation |
| `ggplot2` | Visualization and automated plotting |
| `psych` | Reliability analysis, EFA, psychometrics |
| `effectsize` | Cohen's d, η², standardized effect sizes |
| `RMarkdown` | Reproducible documentation throughout |
| `LOESS` | Non-parametric trend modeling |
