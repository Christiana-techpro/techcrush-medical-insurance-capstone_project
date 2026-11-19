# techcrush-medical-insurance-capstone_project
Predicting annual medical insurance charges and uncovering key cost drivers using EDA and Regression models (TechCrush Cohort 9 Data Science Capstone).

# Medical Insurance Cost Prediction — TechCrush Cohort 9 Capstone

## 1. Problem Statement
Medical insurance costs vary widely across individuals depending on age, lifestyle, body mass index (BMI), family size, and region. An insurance provider needs a reliable way to estimate a customer's annual medical charges and understand which factors drive higher costs so it can set fair pricing and design targeted wellness incentives.

**Who uses this solution:** Insurance pricing analysts, underwriting teams, and business decision-makers looking for clear, data-backed guidance on risk and customer pricing.

## 2. Dataset
* **Source:** [Medical Cost Personal Datasets (Kaggle)](https://www.kaggle.com/datasets/mirichoi0218/insurance)
* **Size:** 1,338 records and 7 columns (`age`, `sex`, `bmi`, `children`, `smoker`, `region`, `charges`)
* **Target Variable:** `charges` (annual individual medical costs billed by health insurance, in USD)

## 3. Team Members & Pair Responsibilities
Each teammate owns a separate file to keep our workflow organized and prevent merge conflicts.

| Pair | Shared Role | Partner A (Name & GitHub) | Partner B (Name & GitHub) | Assigned Files |
| :--- | :--- | :--- | :--- | :--- |
| **Pair 1** | **Project Leaders & Final Checkers** | Mongou Loic (`@mongou4`) | *[Add Name & @username]* | `notebooks/00_master_capstone.ipynb`, `README.md`, `requirements.txt` |
| **Pair 2** | **Data Cleaners & Organizers** | *[Add Name & @username]* | *[Add Name & @username]* | `notebooks/01_data_cleaning.ipynb`, `notebooks/02_data_grouping.ipynb` |
| **Pair 3** | **Chart Makers (EDA Visuals)** | *[Add Name & @username]* | *[Add Name & @username]* | `notebooks/03_charts_smoking.ipynb`, `notebooks/04_charts_demographics.ipynb`, `figures/` |
| **Pair 4** | **Prediction Model Builders** | *[Add Name & @username]* | *[Add Name & @username]* | `notebooks/05_model_linear.ipynb`, `notebooks/06_model_forest.ipynb` |
| **Pair 5** | **Medium Writer & Slide Designer** | *[Add Name & @username]* | *[Add Name & @username]* | Medium Report & Presentation Slides |

## 4. Repository Structure

    techcrush-cohort9-medical-insurance-capstone/
    ├── data/
    │   ├── insurance.csv               # Raw Kaggle dataset
    │   ├── insurance_clean.csv         # Cleaned dataset (duplicates/issues checked)
    │   └── insurance_featured.csv      # Dataset with grouped age/BMI labels
    ├── figures/                        # Exported PNG charts for Medium and Slides
    ├── notebooks/
    │   ├── 00_master_capstone.ipynb    # Final combined capstone notebook
    │   ├── 01_data_cleaning.ipynb      # Pair 2A: Data audit & duplicate removal
    │   ├── 02_data_grouping.ipynb      # Pair 2B: Feature grouping (BMI & age tiers)
    │   ├── 03_charts_smoking.ipynb     # Pair 3A: Charges & smoking EDA charts
    │   ├── 04_charts_demographics.ipynb# Pair 3B: Age, BMI, region & family charts
    │   ├── 05_model_linear.ipynb       # Pair 4A: Train/test split & Linear Regression
    │   └── 06_model_forest.ipynb       # Pair 4B: Random Forest & top factors chart
    ├── README.md
    └── requirements.txt

## 5. How to Run This Project
1. Clone this repository to your computer:

       git clone https://github.com/mongou4/techcrush-cohort9-medical-insurance-capstone.git
       cd techcrush-cohort9-medical-insurance-capstone

2. Install the required Python libraries:

       pip install -r requirements.txt

3. Open `notebooks/00_master_capstone.ipynb` in Jupyter Notebook or VS Code and run all cells from top to bottom.

## 6. Project Deliverables
* **GitHub Repository:** This repository
* **Medium Report:** *[Link to be added by Pair 5A]*
* **Presentation Slides:** *[Link to be added by Pair 5B]*
