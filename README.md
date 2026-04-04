# Additionality Constraints & Investment in Carbon Sequestration

This repository contains the core materials and results for a research project studying how **additionality constraints** affect investment incentives in **soil organic carbon (SOC) sequestration**. We analyze four scenarios using an optimal control framework, evaluate results across **Texas**, and present numerical outputs on SOC sequestration both under the additionality constraint and under a fully monetizable carbon asset class.

---

## 📁 Repository Contents

### 1. `AdditionalityConstraint_Code_3.ipynb`

This Python Jupyter Notebook implements and solves the optimal control problem numerically for four scenarios:

- **Scenario 1**: Uses baseline parameter values from Table 1.
- **Scenario 2**: Normalizes the parameters (\hat{C}, \bar{C}, \theta) by (\sigma C_0).
- **Scenario 3**: Normalizes (\hat{C}, \bar{C}, \theta) by (\sigma C_0) and considers a smaller (\bar{C}).
- **Scenario 4**: Normalizes (\hat{C}, \bar{C}, \theta) by (\sigma C_0) and considers a larger (\bar{C}).

We use a **direct approach** to numerically solve the model by discretizing the problem and transcribing the optimal control formulation into a numerical optimization problem.

The notebook includes:
- Visualizations of key policy-relevant results
- Robustness checks using different normalization schemes and upper bounds on SOC

---

### 2. `Sensitivity analyses.xlsx`

This Excel file summarizes the results from the optimal control problem for **Scenarios 2–4**, including:
- Total SOC sequestered (for a representative oilseed and grain farmer and for a representative vegetable and melon farmer) by 2050 under the additionality constraint and under a fully monetizable carbon asset class.
- A terminal time horizon sensitivity analysis focusing on 15 years (2040) and 30 years (2055) for a representative oilseed and grain farmer.

---

### 3. `2022 Census Calculations.xlsx`

This Excel file provides some of the data used to calculate the net income per hectare for a oilseed and grain farmer (NAICS 1111) and a vegetable and melon farmer (NAICS 1112) in Texas.

---

### 4. `Texas.aprx` (ArcGIS Project File)

This ArcGIS Pro project contains spatial data for Texas, including:
- **World Soils 250m Organic Carbon Stocks (2020)**
- **Land Cover Data (2021)**
- **USDA Crop Sales by County (2022)**
- **SOC stocks (Mg/ha) at 250m resolution**
- **Cropland area (2021)**

All layers are ready for:
- Visual analysis
- Map exports


---

## 🧠 Research Motivation

Carbon offset markets often use **additionality constraints** to ensure that credited sequestration wouldn’t have occurred without payments. However, these constraints may limit investment in carbon farming and lead to suboptimal climate outcomes.

This project investigates how relaxing the additionality constraint and fully monetizing historically accumulated SOC can incentivize greater sequestration and reshape investment dynamics.

---

## 🔧 How to Use

### Python Model
1. Clone the repository.
2. Open `AdditionalityConstraint_Code_3.ipynb` in Jupyter Notebook or JupyterLab.
3. Ensure the following Python packages are installed:
   ```bash
   pyomo.environ
   pyomo.dae
   matplotlib
   numpy
