# Data Dictionary

| Variable | Definition | Unit | Source | Role in analysis |
|---|---|---|---|---|
| `Country` | Country name | Text | Harmonized | Country identifier |
| `ISO3` | ISO-3 country code | Code | Harmonized | Cross-source matching key |
| `Year` | Observation year | Year | Source datasets | Panel time identifier |
| `AI_Adoption_pct` | Enterprises using artificial intelligence; enterprises with 10+ employees | % of enterprises | OECD ICT Access and Usage by Businesses | AI Capacity Index component and temporal growth measure |
| `AI_Conference_Publications` | AI-related conference publications attributed to a country | Papers | CSET / Stanford HAI Global AI Vibrancy | AI Capacity Index component |
| `AI_Patent_Grants` | AI-related patents granted to applicants from a country | Patents | CSET / Stanford HAI Global AI Vibrancy | AI Capacity Index component |
| `AI_Private_Investment_USD_Bn` | Private investment received by AI companies | USD billions | Stanford AI Index 2025 / Quid | Complementary descriptive indicator; excluded from AI Capacity Index |
| `Carbon_Intensity_gCO2_kWh` | Direct power-sector CO2 emissions per unit of electricity generation | gCO2/kWh | Ember Yearly Electricity Data | Environmental Sustainability Index component; decarbonization measure |
| `Renewable_Electricity_pct` | Electricity generation from renewable sources, including hydro | % of generation | Ember Yearly Electricity Data | Environmental Sustainability Index component |
| `Energy_Intensity_MJ_per_2021PPP_USD` | Primary-energy supply per unit of PPP-adjusted GDP | MJ per 2021 international-$ PPP GDP | IEA/IRENA/UN/WHO/World Bank via Our World in Data | Environmental Sustainability Index component |
| `AI_Capacity_Index` | Mean standardized score of AI adoption, log-transformed publications, and log-transformed patents | z-score | Derived | Cross-country AI capacity measure |
| `Environmental_Sustainability_Index` | Mean standardized score of renewable share, inverse carbon intensity, and inverse energy intensity | z-score | Derived | Cross-country sustainability measure |
| `AI_ENV_Profile` | Four-group classification based on median splits of the two composite indices | Category | Derived | Country profiling |
| `AI_CAGR_pct` | Compound annual growth rate of AI adoption from 2021 to 2025 | % per year | Derived | Temporal AI growth measure |
| `Decarbonization_pct` | Relative reduction in electricity carbon intensity from 2021 to 2025 | % | Derived | Temporal decarbonization measure |
| `AI_Decarb_Gap_Z` | Difference between standardized AI CAGR and standardized decarbonization rate | Standard deviations | Derived | Comparative AI–decarbonization alignment indicator |

## Missing data rule

Missing values are preserved as missing. They must not be interpreted as zeros. No interpolation, mean replacement, or model-based missing-value completion was applied in the study dataset.
