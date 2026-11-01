# Artificial Intelligence Capacity and Environmental Sustainability in OECD Countries

This repository contains the harmonized dataset, derived indicators, analysis workbook, figures, and conference manuscript materials used in the study:

**Artificial Intelligence Capacity and Environmental Sustainability in OECD Countries: A Cross-Country Assessment**

The study was prepared for the **3rd International Congress on Data Science and Information Technologies (INFTEC 2026), Nicosia / TRNC, 22–24 October 2026**.

## Authors

- Özge Taş
- Rabia Yumuşak

## Study scope

The study evaluates the relationship between artificial intelligence capacity and environmental sustainability across **38 OECD member countries**. The analytical framework combines indicators of AI adoption, scientific output, technological innovation, electricity-sector carbon intensity, renewable electricity share, and energy intensity.

The longitudinal component covers **2021–2025** where comparable endpoint data are available. Cross-sectional indicators use the most recent broadly comparable year available for each source.

## Repository structure

```text
.
├── README.md
├── data_dictionary.md
├── methodology.md
├── sources.md
├── CITATION.cff
├── LICENSE.md
├── data/
│   ├── OECD_AI_Sustainability_Panel_v2.xlsx
│   └── OECD_AI_Sustainability_Analysis_v4_with_Figures.xlsx
├── figures/
│   ├── Figure1_AI_vs_Environmental_Sustainability.png
│   ├── Figure3_Environmental_by_AI_Group.png
│   ├── Figure4_AI_Decarbonization_Gap.png
│   └── Figure_Manifest.csv
├── paper/
│   └── INFTEC_2026_full_text.docx
└── archive/
    ├── OECD_AI_Sustainability_Panel_v1.xlsx
    └── OECD_AI_Sustainability_Analysis_v3.xlsx
```

## Main derived indicators

### AI Capacity Index

The AI Capacity Index is calculated from standardized values of:

1. AI adoption rate,
2. `ln(1 + AI conference publications)`, and
3. `ln(1 + AI patent grants)`.

The index is computed as the arithmetic mean of the available standardized components and requires at least two of the three components.

### Environmental Sustainability Index

The Environmental Sustainability Index is calculated as the mean of:

1. standardized renewable electricity share,
2. standardized inverse carbon intensity, and
3. standardized inverse energy intensity.

Higher values therefore correspond to relatively stronger environmental and energy sustainability performance.

### AI–Decarbonization Gap

The AI–Decarbonization Gap compares the relative pace of AI adoption growth and power-sector decarbonization:

`AI–Decarbonization Gap = z(AI adoption CAGR) − z(decarbonization rate)`

A positive value indicates that AI adoption grew faster relative to OECD peers than power-sector decarbonization. A negative value indicates relatively stronger decarbonization performance. The indicator is comparative and should not be interpreted as an absolute environmental success/failure measure or as evidence of causality.

## Data availability and reuse

The repository contains a harmonized research dataset assembled from publicly available third-party sources. Original source data remain subject to the terms, licenses, and conditions of their respective providers. The authors do not claim ownership of the underlying third-party source data.

Derived indicators, documentation, and analytical organization created by the authors may be reused subject to the terms described in `LICENSE.md`, while users should consult the original providers before redistributing source-derived data.

## Citation

If you use this dataset or its derived indicators, please cite the study and this repository. See `CITATION.cff` for machine-readable citation metadata.

## Notes on reproducibility

- Missing observations were retained as missing and were not coded as zero.
- No interpolation, mean substitution, or model-based missing-value completion was applied.
- Private AI investment was retained as a complementary descriptive indicator but excluded from the AI Capacity Index because country coverage was limited.
- Energy intensity uses the latest broadly comparable year available in the assembled dataset (2022), while the main AI/electricity cross-section uses 2024 values.
- Analyses are comparative and observational; causal claims are not made.
