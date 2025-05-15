# Pharmacovigilance-EDA-Analyzing-Adverse-Drug-Reactions-from-the-OpenFDA-Dataset

# 📊 Adverse Drug Reaction Analysis using OpenFDA Data

This project analyzes publicly available drug adverse event reports from the [OpenFDA](https://open.fda.gov/) dataset. The goal is to perform Exploratory Data Analysis (EDA) to uncover insights into drug safety, adverse reactions, and demographic impact trends.

---

## 📁 Dataset

- **Source:** Kaggle / OpenFDA Drug Event Dataset
- **Size:** ~10,000 records
- **Structure:** JSON data containing nested fields for patient, reaction, and drug details

---
## 🛠️ Tech Stack

- **Python (Pandas, NumPy, Matplotlib, Seaborn)**
- **Jupyter Notebook** for stepwise analysis
- **Data Normalization & JSON Parsing**
-  Pure EDA with real-world pharma data
---

## 🧹 Data Preparation

The raw data required extensive **cleaning, categorization from Numerical Codes, DataType conversions and Normalization**:
- Extracted and structured nested fields (`Reactions`, `Drug Details`)
- Created 3 normalized DataFrames:
  - `df_primary` – Core information (e.g., Report ID, Age, Gender, Seriousness, Country, Dates)
  - `df_reactions` – One row per adverse reaction per report
  - `df_drugs` – One row per drug per report, with administration route and indication

---

## 📊 Exploratory Data Analysis (EDA)

### 1. **Demographic Insights**
- Distribution by **Patient Gender** and **Age Groups**
- High missing values in Age handled via binning and ‘Missing’ category

### 2. **Seriousness Analysis**
- Split between **Serious** and **Non-Serious** cases
- Reports that resulted in **Death**
- Country-wise distribution of adverse reports

### 3. **Time Trend Analysis**
- Year-wise and Month-wise trend in reporting
- Seasonal peaks (e.g., August and September)

### 4. **Drug Analysis**
- Top 10 most reported drugs
- Most common drug indications (e.g., Myelofibrosis, Multiple Sclerosis)
- Routes of administration associated with serious events
- Drugs most linked with death or serious outcomes

### 5. **Reaction Analysis**
- Most frequent reactions (e.g., Dyspnoea, Drug Ineffective)
- Reactions most marked as serious (e.g., Type 2 Diabetes Mellitus, Hyperthermia Malignant)
- Gender-wise reaction distribution

---

## 📈 Visualizations

- Count plots for Age, Gender, Seriousness, Reactions, Drugs
- Timeline plots for event counts
- Heatmaps for drug-reaction associations
- Pie charts and bar graphs for categorical breakdowns

---

## ✅ Key Insights

- **Females** reported higher adverse events than males.
- Most reports came from the **United States**.
- **Older patients (61–75)** had the highest report count.
- **Lipitor** is most frequently associated with serious or death-related cases.
- There is **seasonal reporting behavior**, peaking in **August**.

---

## 📌 Future Scope

- Build a dashboard
- Add ML models for risk prediction or classification
---
## Regards,
Shikha Yadav
