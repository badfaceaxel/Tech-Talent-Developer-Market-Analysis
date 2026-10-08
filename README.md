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

