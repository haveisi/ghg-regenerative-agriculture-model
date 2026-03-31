# GHG Accounting Model for Regenerative Agriculture Supply Chains

## Overview
This project implements a simplified greenhouse gas (GHG) accounting model for an agricultural supply chain using Python.

It demonstrates how to estimate:
- Scope 1 emissions from facilities (stationary combustion)
- Scope 1 emissions from fleet fuel use
- Farm-level emissions from agricultural inputs and operations
- Emissions intensity per tonne of crop
- Differences between conventional and regenerative farming systems

The model is designed to reflect the structure of real-world ESG and GHG reporting workflows, while remaining transparent and easy to follow.

---

## Why this matters
Agricultural supply chains are a major source of emissions, driven by:
- Fuel use (diesel, gasoline)
- Fertilizer production and application
- Soil emissions (especially N₂O)
- Land management practices

There is increasing interest in **regenerative agriculture** as a way to reduce emissions intensity and improve soil carbon outcomes.

This project explores how different farming systems may impact:
- Gross emissions
- Emissions intensity (kgCO2e per tonne)
- Soil carbon (reported separately as a memo item)

---

## Model structure

### 1. Operational Scope 1
- Stationary fuel use (e.g., natural gas, diesel)
- Fleet fuel consumption (mobile combustion)

### 2. Farm-level emissions
Includes:
- Diesel use
- Nitrogen fertilizer (production + soil N₂O)
- Herbicides and inputs
- Lime application
- Transport of inputs

### 3. Regenerative vs Conventional comparison
The model aggregates results by system type:
- Total emissions (tCO2e)
- Emissions intensity (kgCO2e per tonne)
- Soil carbon change (memo only)

---

## Key results (example output)

### Operational Scope 1
- Stationary: **341.8 tCO2e**
- Fleet: **81.6 tCO2e**
- Total: **423.4 tCO2e**

### Farm comparison

| System        | Gross tCO2e | kgCO2e / tonne |
|--------------|------------|----------------|
| Conventional | 137.2      | 258.9          |
| Regenerative | 43.2       | 92.2           |

The model suggests significantly lower emissions intensity in the regenerative system. However, this result is highly sensitive to assumptions and emission factors.

---

## Important assumptions and limitations

This is a **simplified model for demonstration purposes**:

- Emission factors are illustrative and not fully validated
- Soil carbon is treated as a **memo item** and is NOT netted against gross emissions
- Not all emission sources are included (e.g., livestock, upstream supply chain)
- Results are sensitive to fertilizer assumptions and yield differences

This reflects real-world challenges in agricultural GHG accounting.

---

## How to run

Install dependencies:

```bash
pip install -r requirements.txt
