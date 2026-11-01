# Methodology

## 1. Study scope

The analysis covers 38 OECD member countries.

## 2. Data collection

AI and environmental indicators were compiled from OECD, Stanford HAI/CSET, Ember, Stanford AI Index, and international energy data sources.

## 3. Data harmonization

Country names were standardized using ISO-3 codes and merged into a common country-level structure. Missing observations were preserved as missing.

## 4. Variable transformation

Indicators measured in different units were standardized using z-scores. AI conference publication and patent counts were strongly right-skewed and were transformed using `ln(1+x)` before standardization.

## 5. AI Capacity Index

The index is based on:

- z(AI adoption rate)
- z(ln(1 + AI conference publications))
- z(ln(1 + AI patent grants))

For country *i*:

`AI Capacity Index_i = mean(available standardized AI components)`

The index was calculated only for countries with at least two of the three components.

Private AI investment was not included because coverage was restricted to a limited set of leading countries.

## 6. Environmental Sustainability Index

The index is defined as:

`Environmental Sustainability Index_i = mean[z(Renewable Share), z(-Carbon Intensity), z(-Energy Intensity)]`

The signs of carbon intensity and energy intensity were reversed so that higher index scores consistently represent more favorable sustainability performance.

## 7. Country profiles

Countries were classified into four groups using the median values of the AI Capacity Index and Environmental Sustainability Index:

- High AI / High Sustainability
- High AI / Low Sustainability
- Low AI / High Sustainability
- Low AI / Low Sustainability

## 8. Statistical analyses

- Descriptive statistics
- Spearman rank correlation
- Benjamini–Hochberg false discovery rate correction for multiple comparisons
- Mann–Whitney U test for high- versus low-AI-capacity groups
- Rank-biserial correlation as an effect-size measure

Statistical significance was evaluated at `p < 0.05`.

## 9. Temporal analysis, 2021–2025

AI adoption growth was calculated using the compound annual growth rate:

`AI CAGR = (AI_2025 / AI_2021)^(1/4) - 1`

Power-sector decarbonization was calculated as:

`Decarbonization Rate = (CarbonIntensity_2021 - CarbonIntensity_2025) / CarbonIntensity_2021`

The strict temporal sample includes countries with both 2021 and 2025 AI-adoption and carbon-intensity observations.

## 10. AI–Decarbonization Gap

The comparative indicator was defined as:

`AI–Decarbonization Gap = z(AI CAGR) - z(Decarbonization Rate)`

Positive values indicate that AI adoption grew relatively faster than decarbonization compared with OECD peers; negative values indicate relatively stronger decarbonization performance. The indicator is not a causal lag measure and should not be interpreted as an absolute environmental ranking.
