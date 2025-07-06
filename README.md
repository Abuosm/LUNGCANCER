🫁 LUNGCANCER
Handling Missing Biomarker Data in Lung Cancer Patients with Diabetes via KNN Imputation

📌 Table of Contents
Overview

Data Description

Imputation Methodology

Repository Structure

Installation & Usage

Examples

Results & Findings

Future Work

Licensing & Contributions

Overview
This project tackles the challenge of missing clinical data in lung cancer patients, particularly those diagnosed with diabetes. We analyze key biomarkers—CA19‑9, LYVE1, CYFRA 21‑1, and Creatinine—and employ K-Nearest Neighbors (KNN) to impute missing values, enhancing downstream analyses.

Data Description
patient_data.csv, Original_Data.csv, diabetes_patients.csv, etc.: Raw clinical measurements and patient attributes

blood_data_set.csv: Focused on biomarker measurements (CA19‑9, LYVE1, CYFRA, Creatinine)

imputed_patient_data.csv: Contains datasets post-imputation ready for analysis

Imputation Methodology
Exploratory Analysis: Identify patterns and distribution of missing values via data_info.ipynb.

KNN Imputation:

Fill missing values using KNN based on closest patient profiles

Verified via Knn_algorithm.ipynb

Validation: Compare imputed vs. original values in masked validation to assess accuracy.

Repository Structure
arduino
Copy
Edit
/
├── data_info.ipynb           # data exploration & missingness visualization
├── Knn_algorithm.ipynb       # imputation pipeline demo
├── main.ipynb                # combined workflow notebook
├── *.csv                     # raw & cleaned data files
└── imputed_patient_data.csv  # final imputed dataset
Installation & Usage
Clone the repository

bash
Copy
Edit
git clone https://github.com/Abuosm/LUNGCANCER.git
cd LUNGCANCER
Set up environment

bash
Copy
Edit
pip install -r requirements.txt
Run the notebooks

data_info.ipynb: Explore missing patterns

Knn_algorithm.ipynb: Execute imputation on sample sets

main.ipynb: Full workflow with data pre- and post-imputation

Examples
Missingness Report: Clear visuals and statistics for absent biomarker data

Before/After Comparison: Visualize how KNN fills in values

Performance Metrics: Imputation error rates via RMSE and MAE

Results & Findings
Successfully imputed missing biomarker values across ~X% of the dataset

Achieved RMSE of Y and MAE of Z for validation cohort

Enhanced dataset completeness enables more reliable statistical analysis downstream

Future Work
Compare KNN with other imputation strategies (e.g., MICE, regression)

Integrate imputed data into predictive lung cancer models

Automate imputation using a modular Python or R package

Licensing & Contributions
This project is released under the MIT License

Contributions are welcome!

Fix bugs, add features, improve documentation

Please open a Pull Request or Issue 🎉

✅ Acknowledgements
Thanks to the original data contributors and authors

Inspiration from best practices in clinical data imputation workflows
