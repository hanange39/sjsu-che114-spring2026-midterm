# Data-Driven Prediction of Lithium-ion Battery Degradation from Partial Cycling Data Using Machine Learning

Study the degradation of an 18650 lithium-ion battery (NMC811/graphite-silicon) over 400 cycles and compare two machine learning models to determine which best predicts maximum discharge capacity.

## Course Context
* **Course:** CHE114: Data Science in Chemical and Materials Engineering
* **Institution:** San Jose State University
* **Instructor:** Prof. Naoki Matsumura
* **Term:** Spring 2026

## Team Members
* **Thi Le**
* **Henry Maala**
* **Angela Han**

## Dataset
* **Source:** [UCL Lithium-ion Battery INR18650 MJ1 Data: 400 Electrochemical Cycles](https://rdr.ucl.ac.uk/articles/dataset/Lithium-ion_Battery_INR18650_MJ1_Data_400_Electrochemical_Cycles_EIL-015_/12159462/1?file=23140433)
* **Description:** Cycling data for a single 3.5 Ah LG Chem NCA INR18650 MJ1 cell. The cell was cycled according to the manufacturer's recommendations in a fixed ambient temperature (24 °C) for 400 cycles. The dataset provides in-cycle measurements of temperature, voltage, and capacity, and per-cycle measurements of charge/discharge capacity in `.csv` format.

## Models Evaluated
* **Non-Tree-Based Model:** Linear Regression
* **Tree-Based Model:** Extra Trees Regressor (via FLAML AutoML)
* **Result:** The Extra Trees Regressor outperformed Linear Regression, capturing non-linear capacity fade with a lower MAE.

## Quick Start

### Prerequisites
* **Python 3.x**
* **Jupyter Notebook** or **JupyterLab**
*(Alternatively, this file can be opened directly in **VS Code** with the Jupyter extension installed, or uploaded to **Google Colab**).*

### Running the Project
1. Clone this repository:
   ```bash
   git clone https://github.com/hanange39/sjsu-che114-spring2026-midterm.git
   ```
2. Navigate to the folder:
   ```bash
   cd sjsu-che114-spring2026-midterm
   ```
3. Install any required libraries:
   ```bash
   pip install "flaml[automl]" pandas numpy matplotlib scikit-learn scipy
   ```
4. Launch the Jupyter Notebook environment:
   ```bash
   jupyter notebook
   ```
5. The browser will open. Click on the notebook file and run the cells sequentially.

## Built With
* **Python 3**
* **Jupyter Notebook**
* **FLAML** (Automated Machine Learning)
* **Data & Science Libraries:** `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `scipy`
