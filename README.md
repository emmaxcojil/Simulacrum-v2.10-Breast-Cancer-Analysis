# Simulacrum-v2.10-Breast-Cancer-Analysis
Breast Cancer Exploratory Data Analysis Project using the Simulacrum v2.1.0 tumour diagnoses, SACT, radiotherapy and gene testing data

Project Overview
The Simulacrum is a synthetic dataset that mirrors real patient data for breast cancer, allowing researchers to explore patterns and correlations without compromising patient confidentiality. This project aims to:

Merge and preprocess data from multiple tables.
Filter the data to include only breast cancer patients.
Perform exploratory data analysis (EDA) on patient demographics, tumor characteristics, and treatment patterns.
Visualize key findings through graphs and charts.
Conduct survival analysis using Kaplan-Meier curves.
Develop a web application to predict patient survival.
Discuss limitations of the data.

Dataset Description
The dataset includes the following tables:

The following datasets were used in this analysis:

sim_av_gene: Gene data for patients.
sim_av_patient: Demographic and patient-level data.
sim_av_tumour: Tumour characteristics and diagnoses.
sim_rtds_combined: Combined radiotherapy records.
sim_rtds_episode: Radiotherapy treatment episodes.
sim_rtds_exposure: Radiotherapy exposure details.
sim_rtds_prescription: Radiotherapy prescriptions.
sim_sact_cycle: Chemotherapy cycle details.
sim_sact_drug_detail: Chemotherapy drug details.
sim_sact_outcome: Chemotherapy outcomes.
sim_sact_regimen: Chemotherapy regimen data.
Each table contains specific information related to patients, tumors, treatments, and outcomes. The data covers various aspects such as:

Patient Demographics: Age at diagnosis, gender, vital status.
Tumor Characteristics: Site, morphology, behavior, grade.
Treatment Data: Radiotherapy episodes, prescriptions, exposures, chemotherapy regimens, cycles, drug details.
Genetic Information: Gene mutations associated with breast cancer.
Outcomes: Survival data, treatment modifications.

A. Steps
1. Filtering Breast Cancer Patients
The initial step involved filtering the dataset to extract only breast cancer patients based on specific ICD codes. The sim_av_tumour dataset was filtered using the following ICD-10 codes:

2-11. Filtering Other Datasets for Breast Cancer Patients Only
The same set of breast cancer patients identified in Step 1 was used to filter other datasets:

sim_av_gene: Gene data filtered for breast cancer patients.
sim_av_patient: Patient demographic data filtered.
sim_rtds_episode, sim_rtds_combined, sim_rtds_exposure, sim_rtds_prescription: Radiotherapy data filtered for breast cancer.
sim_sact_regimen, sim_sact_cycle, sim_sact_drug_detail, sim_sact_outcome: Chemotherapy data filtered for breast cancer.

B. Visualizations and Key Insights:
Several visualizations to display the various insights gotten from the data analysis

1. Demographics & Vital Status Distribution
Visualizations were created to show the distribution of demographics and vital status:

Age, sex and ethnicity distribution of breast cancer patients.
Vital status (alive vs. deceased) across the patient population.

2. Tumour Analysis
This section focused on breast cancer tumour characteristics:

Distribution of tumour sites, morphology codes, behaviour types, and grade types.
Kaplan-Meier survival curves based on tumour grades, showing survival probabilities over time.

3. Treatment Pathways
Analysis of treatment regimens and outcomes:

Most commonly used chemotherapy regimens for breast cancer treatment.
Comparison of regimen types vs. survival rates.
Survival curves comparing the top five most frequently used regimens.
Most frequently administered drugs based on dosage and frequency.
Routes of drug administration and frequency of treatment modification.

4. Treatment Modalities & Intents
In-depth analysis of radiotherapy treatments:

Distribution of radiotherapy modalities and treatment intents.
Comparisons between prescribed fractions and actual fractions delivered.
Analysis of prescribed doses vs. actual doses received.

5. Survival Prediction 
A web-based application was developed to predict patient survival rates based on the breast cancer data and analysis.
The Application also has several sections showing the visuals of all results/insights gotten from the analysis

7. Limitations of the Data
Visualizations were created to highlight limitations of the dataset, including missing data, inconsistencies, and potential biases in the simulated dataset.
