# 📊 Tech Talent & Developer Market Analysis

A comprehensive data analysis project examining global software developer survey data to uncover insights on demographics, technology stack adoption, salary distributions, and platform preferences.

---

## 📌 Project Overview

This repository contains an end-to-end Data Analysis workflow designed to process, clean, transform, and analyze developer survey responses. The goal of this project is to provide actionable market intelligence regarding high-demand skills, compensation trends, and technological adoption patterns.

---

## 📁 Repository Structure

```text
.
├── assets/
│   ├── .gitkeep
│   ├── dashboard_preview.png             # Dashboard overview screenshot
│   └── demographics_preview.png          # Demographics analysis screenshot
├── dashboard/
│   └── IBM_Cognos_Dashboard_Report...    # Exported IBM Cognos report file
├── data/
│   ├── processed/
│   │   ├── survey_data_updated 5.zip     # Cleaned and transformed primary dataset
│   │   └── splits/                       # Normalized (1:N) datasets for Cognos BI filtering
│   │       ├── DatabaseHaveWorkedWith_split.csv
│   │       ├── DatabaseWantToWorkWith_split.csv
│   │       ├── LanguageHaveWorkedWith_split.csv
│   │       ├── LanguageWantToWorkWith_split.csv
│   │       ├── PlatformHaveWorkedWith_split.csv
│   │       ├── PlatformWantToWorkWith_split.csv
│   │       ├── WebframeHaveWorkedWith_split.csv
│   │       └── WebframeWantToWorkWith_split.csv
│   └── raw/
│       └── dataset_link.txt                 # Source reference and link to original raw data

## 🛠️ Data Pipeline & BI Data Modeling
Exploratory Data Analysis (EDA) & Data Cleaning:

Processed raw survey responses, handled missing values, corrected data types, and normalized numerical metrics.

Exported the consolidated clean dataset (survey_data_updated 5.zip).

Data Normalization for Business Intelligence (IBM Cognos):

Multi-select survey fields (e.g., Languages, Databases, Web Frameworks, Platforms) contained semicolon-separated values within single cells.

To enable accurate filtering, aggregation, and relational modeling in IBM Cognos, these columns were split and exploded into 1-to-N relational tables (data/processed/splits/).

This structure allows precise dynamic drill-downs on developer preferences without double-counting biases.

## 📈 Key Insights & Findings
Top Remunerated Technologies: Languages like Swift and Python show high compensation medians relative to global averages.

Skill Demand vs. Desire: High correlation between current language usage and future adoption interest in modern web frameworks and cloud platforms.

Demographic Distribution: Detailed breakdown of experience levels, primary roles, and regional participation.

## 🚀 How to Run the Project
Clone the Repository:

git clone [https://github.com/badfaceaxel/Tech-Talent-Developer-Market-Analysis.git](https://github.com/badfaceaxel/Tech-Talent-Developer-Market-Analysis.git)
cd Tech-Talent-Developer-Market-Analysis

Run the Notebook:

Open notebooks/notebook.ipynb using Jupyter Notebook, JupyterLab, or Google Colab.

Execute the cells sequentially to reproduce the data processing and preliminary visualizations.

Explore the Dashboard:

Import the report file in dashboard/ into IBM Cognos Analytics to interact with the visual dashboard.

## 🧰 Technologies & Tools Used
Language: Python

Data Processing: Pandas, NumPy

Data Visualization & BI: IBM Cognos Analytics, Matplotlib / Seaborn

Environment: Jupyter Notebook, Git/GitHub
├── notebooks/
│   └── notebook.ipynb                       # Complete Jupyter Notebook (ETL & EDA)
└── README.md                                # Project documentation
