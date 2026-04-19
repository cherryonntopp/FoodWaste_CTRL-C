# Beyond the Bin
### CTRL+C - UCSD DataHacks 2026
**Track:** Analytics | **Theme:** Environment & Climate  
**Team:** Justin Sipraseuth, Justin Santiago, Shana Ibatuan

---

## The Question
Is waste generation in the majority of the United States improving or getting worse?

---

## What We Found
The average American generates around 1,600 lbs of waste per year, which is 
the weight of a vintage car. And while waste per capita has stayed 
roughly flat, the total amount going to landfills keeps climbing 
because of population growth.

More importantly, the composition of waste hasn't changed. The same 
percentage goes to landfills today as it did in 2007. Recycling is flat. 
Composting is flat. Environmental efforts over the past decade have not 
meaningfully shifted where waste ends up.

Our recommendation: stop looking at national averages and dig into 
state-level outliers. States that successfully reduced landfill waste 
or improved recycling rates hold the blueprint for what policies and 
infrastructure actually work.

---

## Files

| File | Description |
|---|---|
| `power2_impexp.csv` | Core waste dataset — tracks waste by state, county, year, and type (disposal, recycling, composting, etc.) from 1991–2021 across 36 US states |
| `population.csv` | County-level US population data from 1991–2019 used to calculate per capita metrics |
| `DataHacks 2026 FINAL ANALYSIS - Type and p...` | Main analysis notebook — full code for data cleaning, merging, per capita calculation, and composition analysis |
| `Charts/` | Folder containing all generated charts used in the presentation |
| `README.md` | This file |

---

## Methodology
1. Filtered waste data for disposal, recycling, and composting types
2. Aggregated county-level data up to state level where needed
3. Reshaped population data from wide to long format and aggregated to state level
4. Merged both datasets on state + year
5. Calculated core metric: `(tons / population) * 2000 = lbs per person per year`
6. Analyzed composition of waste over time across 27 states with complete records (2007–2018)

---
