Water Quality Prediction – EY 2026
Overview

This project predicts river water quality in South Africa using historical measurements and environmental data.
It was built as part of the EY AI & Data Challenge 2026 – Optimizing Clean Water Supply.

The goal is to predict three water quality values for new river locations:

Total alkalinity

Electrical conductance

Dissolved reactive phosphorus

Problem Statement

Given:

River location (latitude, longitude)

Date of measurement

Past water quality readings

Build a model that can:

Learn patterns from historical data

Predict water quality for new regions

Highlight which factors influence water quality the most

Data

The dataset contains:

River samples collected between 2011–2015

~200 river locations across South Africa

Geographic coordinates and dates

Three water quality measurements

Additional environmental data (e.g. climate or satellite data) may be used to improve predictions.

Approach

High-level steps followed in this project:

Load and clean the data

Create simple time-based features (month, season)

Train separate models for each water quality parameter

Test performance on unseen regions

Generate a submission file in the required format

Analyze which inputs affect predictions the most

Evaluation

Model performance is measured using R² score.

The final score is the average R² across all three water quality parameters.

Repository Structure
├── data/          # Raw and processed datasets
├── notebooks/     # Data exploration and model training
├── models/        # Saved models (if any)
├── submissions/   # Final prediction files
├── requirements.txt
└── README.md

How to Run

Clone the repository

Install dependencies from requirements.txt

Open and run the notebooks in order

Generate the final prediction CSV

Notes

This project focuses on practical modeling, not complex theory

The benchmark model provided by EY is used as a starting point

Improvements are made through better features and tuning

Disclaimer

This repository is for learning and competition purposes only.
Predictions should not be used for real-world water management decisions.
