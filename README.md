# Additionality-Constraints-Investment-in-Carbon-Sequestration
Additionality Constraints Investment in Carbon Sequestration

This repository contains the core materials and results for a research project studying how additionality constraints affect investment incentives in soil organic carbon (SOC) sequestration. We analyze four scenarios using an optimal control framework, evaluate results across Texas, and present numerical outputs on SOC sequestration under the additionality constraint and under a fully monetizable carbon asset class.

1. Jupyter Notebook (AdditionalityConstraint_Code.ipynb)
This Python notebook implements the optimal control problem and solves it numerically for four scenarios:

Scenario 1: using the parameter values from Table 1
Scenario 2: normalizing the parameters \hat{C}, \bar{C}, and \theta by \sigma C_0
Scenario 3: normalizing the parameters \hat{C}, \bar{C}, and \theta by \sigma C_0 and consider a smaller \bar{C}
Scenario 4: normalizing the parameters \hat{C}, \bar{C}, and \theta by \sigma C_0 and consider a larger \bar{C}

We use a direct approach to solve the model using a discretization of the problem followed by a transcription of the optimal control problem

The code includes:

Visualization of key policy-relevant results
Robustness check using normalization and varying upper bound values

2. Excel Results File (Robustness test 2.xlsx)
A summary of results from Scenarios 2–4, including:
Total SOC sequestered by 2050 under the additionality constraint and under a fully monetizable carbon asset class based on the results from the calibrations

3. ArcGIS Project File (Texas.aprx)
Contains spatial data for Texas, including:
World Soils 250m Organic Carbon Stocks from 2020
Land Cover data from 2021
USDA Crop sales from 2022
SOC stocks (Mg/ha) from 2020 in 250m resolution
Cropland area from 2021

Ready-to-use layers for map exports and visual analysis
