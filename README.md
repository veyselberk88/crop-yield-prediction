# Crop Yield Prediction Using Machine Learning

![Project Banner](Images/agriculture.jpg)


This project uses real-world data to build a machine learning model that predicts crop yield based on environmental and agricultural inputs. The goal is to help stakeholders make better decisions around crop selection, input use, and agricultural planning.

## BLUF (Bottom Line Up Front)

This project uses environmental and agricultural data to build a predictive model for crop yield. The final model (XGBoost) achieves R² = 0.999 and highlights rainfall and crop type as key drivers.

## Business Problem

The global population is rising, but farmland is limited. To feed more people without expanding land, we need to increase yield from existing land. This project aims to:

* Predict expected yield using features like rainfall, temperature, and pesticide use
* Identify what factors drive yield the most
* Help growers, advisors, and policymakers plan more effectively

## Stakeholders

* Farmers and growers
* Agricultural advisors
* Government agriculture departments
* International organizations (e.g., FAO)
* Ag-tech companies
* Researchers and NGOs

## Why Machine Learning

Traditional methods often miss complex relationships. ML models can:

* Capture non-linear interactions (e.g., between rainfall and crop type)
* Generalize across countries, crops, and years
* Provide scalable insights to support planning

## Project Workflow
[Data Cleaning] → [Feature Engineering] → [Model Training] → [Model Tuning] → [Evaluation]

## Dataset

* Source: [Crop Yield Prediction Dataset – Kaggle (Omdena project)](https://www.kaggle.com/datasets/oluwatobiajiboye/crop-yield-prediction-dataset)

* File: `yield_df.csv`
* Rows: ~28,000
* Key features: Country (Area), Crop (Item), Year, Yield, Rainfall, Pesticide Use, Avg Temp

## Success Metrics

**Technical**:

* High R² score
* Low MAE and RMSE

**Business**:

* Predictions within 10–15% of actual yield
* Clear identification of top yield drivers

## Methodology

1. **Data Understanding**: Initial inspection, missing values, outliers, trends
2. **Data Preparation**: Feature engineering, log transforms, encoding, pipeline creation
3. **Modeling**: Baseline (Linear Regression), Advanced (Random Forest, XGBoost)
4. **Model Tuning**: GridSearchCV with cross-validation
5. **Evaluation**: Final model testing, feature importance analysis

## Final Model

* Model: XGBoost pipeline
* R² on test set: 0.999
* Top features: Log rainfall, rainfall per ton, crop type

## Files

* `crop_yield_prediction.ipynb`: Main notebook
* `Data/yield_df.csv`: Cleaned dataset
* `xgboost_yield_pipeline.pkl`: Serialized model
* `crop_yield_prediction_pitch.rtf`: Original pitch document
* `Images/agriculture.jpg`: Project banner

## Author

Prepared by: Veysel Berk

Project Duration: October 13–25, 2025
