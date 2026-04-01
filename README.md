# GHG Accounting Model for Regenerative Agriculture Supply Chains

> In this modeled example, regenerative farming systems reduce emissions intensity by ~50–70% compared to conventional systems, primarily driven by lower fertilizer use and soil carbon improvements.

## Overview

This project implements a Python-based greenhouse gas (GHG) accounting model for agricultural operations and supply chains. It estimates emissions across facilities, fleet fuel use, electricity consumption, and farm-level inputs, and compares conventional and regenerative farming systems.

The model is designed as a simplified ESG analytics workflow to support emissions estimation, scenario analysis, and emissions intensity benchmarking.

---

## Why this matters

Agriculture is a significant contributor to global greenhouse gas emissions, driven by:

- Fuel combustion (Scope 1)
- Purchased electricity (Scope 2)
- Fertilizer production and soil emissions
- Livestock and manure management
- Land-use change

Understanding how operational and farming decisions affect emissions is critical for sustainability teams, ESG analysts, and supply-chain decision-makers.

---

## Key Features

- Scope 1 emissions (stationary + fleet fuel)
- Scope 2 emissions (purchased electricity)
- Farm-level emissions modeling (inputs + soil N₂O)
- Emissions intensity (kgCO₂e per tonne of crop)
- Scenario analysis:
  - Fertilizer reduction
  - Regenerative system adjustments
  - Renewable diesel adoption
- Structured outputs and visualizations

---

## Key Findings (Example Results)

- Regenerative systems show lower modeled emissions intensity than conventional systems
- Fertilizer use is a major driver of farm emissions
- Scenario analysis demonstrates meaningful reductions in emissions intensity under regenerative practices

| Metric | Example Result |
|---|---:|
| Scope 1 emissions | ~400–500 tCO2e |
| Scope 2 emissions | ~1200–1500 tCO2e |
| Conventional intensity | ~200–300 kgCO2e/tonne |
| Regenerative intensity | ~70–120 kgCO2e/tonne |

---

## Visualization

### Farm Emissions Intensity
![Farm Intensity](outputs/figures/farm_intensity.png)

### Operational Emissions Breakdown
![Operational Emissions](outputs/figures/operational_emissions_breakdown.png)

---

## Project Structure
