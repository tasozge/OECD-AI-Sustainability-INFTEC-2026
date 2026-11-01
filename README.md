# Artificial Intelligence Capacity and Environmental Sustainability in OECD Countries

This repository documents the dataset, derived indicators, methods, and analysis outputs used in the study:

**Artificial Intelligence Capacity and Environmental Sustainability in OECD Countries: A Cross-Country Assessment**

Prepared for the **3rd International Congress on Data Science and Information Technologies (INFTEC 2026), Nicosia / TRNC, 22–24 October 2026**.

## Authors

- Özge Taş
- Rabia Yumuşak

## Study scope

The study evaluates the relationship between artificial intelligence capacity and environmental sustainability across **38 OECD member countries**. The analytical framework combines AI adoption, scientific output, technological innovation, electricity-sector carbon intensity, renewable electricity share, and energy intensity.

The longitudinal component covers **2021–2025** where comparable endpoint data are available.

## Repository contents

- `data/Country_Summary.csv` — country-level 2021–2025 summary and derived temporal indicators
- `data/Analysis_Results.csv` — descriptive statistics, correlations, group comparisons, and RQ4 results
- `data_dictionary.md` — variable definitions, units, sources, and analytical roles
- `methodology.md` — transformations, composite indices, statistical analyses, and AI–Decarbonization Gap
- `sources.md` — original data sources and URLs
- `figures/Figure_Manifest.csv` — figure descriptions
- `CITATION.cff` — machine-readable citation metadata
- `LICENSE.md` — reuse terms and third-party data notice

## Main derived indicators

### AI Capacity Index

The AI Capacity Index is calculated from standardized values of:
1. AI adoption rate,
2. `ln(1 + AI conference publications)`, and
3. `ln(1 + AI patent grants)`.

The index is the arithmetic mean of available standardized components and requires at least two of the three components.

### Environmental Sustainability Index

The Environmental Sustainability Index is the mean of:
1. standardized renewable electricity share,
2. standardized inverse carbon intensity, and
3. standardized inverse energy intensity.

Higher scores represent relatively stronger environmental and energy sustainability performance.

### AI–Decarbonization Gap

`AI–Decarbonization Gap = z(AI adoption CAGR) − z(decarbonization rate)`

Positive values indicate that AI adoption grew relatively faster than decarbonization compared with OECD peers; negative values indicate relatively stronger decarbonization performance. The indicator is comparative and is not a causal lag measure.

## Data availability and reuse

The repository contains harmonized and derived research materials assembled from publicly available third-party sources. Original source data remain subject to the licenses, terms, and conditions of their respective providers. The authors do not claim ownership of the underlying third-party source data.

Missing observations were retained as missing and were not coded as zero. No interpolation, mean substitution, or model-based missing-value completion was applied.

Private AI investment was retained as a complementary descriptive indicator but excluded from the AI Capacity Index because country coverage was limited.

## Binary research files

The original Excel workbooks, publication figures, and INFTEC 2026 Word manuscript are maintained as companion research files. The current ChatGPT GitHub connector supports direct creation of text-based repository files but did not expose a direct local binary-file upload action in this session. The CSV exports and full documentation needed to inspect the main analysis are included here.

## Citation

If you use this dataset or its derived indicators, please cite the associated INFTEC 2026 study and this repository. See `CITATION.cff`.
