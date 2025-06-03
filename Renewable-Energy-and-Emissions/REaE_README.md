# 🌿 Air Quality, Renewable Energy, and Emissions

**UC Berkeley – Data 102 Final Project**  
_Group 4: Alex Nii, Ethan Antony Serbanescu, Lucas Czajka, Lydia Jung_

---

## Project Overview

This project explores the environmental impact of different energy generation profiles in U.S. regions, with a specific focus on how renewable energy adoption correlates with greenhouse gas emissions. We conducted both exploratory and statistical analyses using EPA eGRID data.

---

## Key Research Questions

1. **Hypothesis Testing**
   - Are CO₂, CH₄, NOₓ, and SO₂ emissions significantly lower in states with more renewable energy?
   - Are fossil-fuel-dominant subregions producing significantly more emissions?

2. **Causal Inference**
   - What is the estimated causal effect of renewable sources (Hydro, Biomass, Solar, Geothermal) on CO₂ emissions?
   - Does fossil fuel reliance predict increased emissions after adjusting for generation capacity?

---

## Methods

- **EDA**: Scatter plots, capacity vs. generation comparisons, regional bar graphs
- **Hypothesis Testing**: Two-sample t-tests with Bonferroni & Benjamini-Hochberg corrections
- **Regression Modeling**: OLS with fuel shares as treatment, controlling for generation & capacity

---

## Files Included

- `REaE_code`: Full Jupyter Notebook with:
  - Data loading and cleaning  
  - Visualization and exploration  
  - Hypothesis testing  
  - OLS regression for causal inference  
  - Summary tables and plots

- `REaE_written_report`: PDF with:
  - Data Overview
  - EDA
  - Research Questions: Hypothesis Testing, CAusal Inference
  - Conclusion

---

## Key Results

- States with ≥30% renewables have ~22% lower CO₂-equivalent emissions
- Methane and NOₓ levels are also lower in high-renewable states
- Hydro is the only renewable energy source with a statistically significant emissions-reducing effect
- Oil is significantly associated with higher emissions

---

## Limitations

- One-year snapshot data limits generalizability  
- Aggregated state/subregion level, no facility or time-series granularity  
- Omitted variable bias possible (e.g., energy policy, demand)

---

## Policy Recommendations

- States should raise Renewable Portfolio Standards to 35%+ by 2030
- Increase investment in hydro where environmentally feasible
- Future work should use high-frequency panel data to confirm causal links

---

## Tools Used

- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Statsmodels, Matplotlib, Seaborn  
- **Environment**: Jupyter Notebook  
- **Data Source**: U.S. EPA eGRID

---
