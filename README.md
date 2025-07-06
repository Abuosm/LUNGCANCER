🫁 LUNGCANCER
Handling Missing Biomarker Data in Lung Cancer Patients with Diabetes Using KNN Imputation

📘 Overview
This project addresses a critical issue in clinical informatics: managing missing biomarker data in lung cancer patients, especially those with diabetes. By applying K-Nearest Neighbors (KNN) imputation, we enhance data integrity and improve downstream analyses on key biomarkers:

CA19‑9

LYVE1

CYFRA 21‑1

Creatinine

📊 Data Description
The dataset comprises several CSV files containing clinical and biomarker data:

File Name	Description
patient_data.csv	General patient info and clinical attributes
Original_Data.csv	Unprocessed original dataset
diabetes_patients.csv	Subset of patients diagnosed with diabetes
blood_data_set.csv	Biomarker-specific measurements
imputed_patient_data.csv	Final dataset with imputed values
🛠️ Imputation Methodology
Exploratory Data Analysis (EDA) Conducted via data_info.ipynb to visualize and understand missing data patterns.

KNN Imputation

Identifies patient similarity using clinical features

Imputes missing biomarker values via Knn_algorithm.ipynb

Validation Strategy

Mask known values to simulate missingness

Evaluate imputation performance using RMSE and MAE metrics

🗂️ Repository Structure
LUNGCANCER/
├── data_info.ipynb           # Missing data exploration
├── Knn_algorithm.ipynb       # KNN imputation demo
├── main.ipynb                # End-to-end workflow
├── *.csv                     # Raw and processed datasets
└── imputed_patient_data.csv  # Output: complete dataset
⚙️ Installation & Usage
Clone the Repository
bash
git clone https://github.com/Abuosm/LUNGCANCER.git
cd LUNGCANCER
Install Dependencies
bash
pip install -r requirements.txt
Run the Notebooks
data_info.ipynb: Visualize missingness

Knn_algorithm.ipynb: Perform imputation

main.ipynb: Execute the full imputation pipeline

💡 Examples & Outputs
📉 Missingness Report: Heatmaps and summaries of incomplete data

🔁 Before vs After: Visualize the impact of imputation

📈 Performance Metrics: RMSE and MAE plots for validation sets

📈 Results & Findings
Imputation filled missing biomarker values across ~X% of the dataset

Achieved RMSE = Y, MAE = Z for the validation cohort

Significantly improved data completeness for robust clinical analysis

🚀 Future Work
Compare KNN with advanced imputation techniques (e.g., MICE, regression, deep learning)

Integrate imputed data into lung cancer risk or progression prediction models

Package the imputation pipeline into a reusable Python or R module

📜 License
This repository is licensed under the MIT License. Feel free to use and adapt!

🤝 Contributions
Contributions, improvements, and bug fixes are welcome!

Open an Issue or submit a Pull Request

Improve documentation, add more data sources, or optimize the algorithm

Let’s make clinical data cleaner together! 🧪

🙌 Acknowledgements
Gratitude to the original data providers and all contributors. Inspired by best practices in biomedical data science and imputation strategies.
