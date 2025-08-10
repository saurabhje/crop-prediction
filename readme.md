# Crop Type Prediction

## Overview
This project builds **multi-class classification models** to predict the type of crop based on soil and environmental features.  
It also identifies the **single most important feature** for predictive performance.

## Dataset
The dataset contains the following features:

- **N**: Nitrogen content in soil  
- **P**: Phosphorous content in soil  
- **K**: Potassium content in soil  
- **ph**: Soil pH value  
- **crop**: Target variable (crop type)

The dataset is included in the folder for ease of use.

## Methodology
1. **Data Preprocessing**:  
   - Checked for missing values  
   - Normalized numerical features  
   - Encoded target labels  

2. **Model Training**:  
   - Trained multiple classification models  
   - Evaluated using F1-score per class  

3. **Feature Importance**:  
   - Measured feature contribution to model performance  
   - Identified the most predictive single feature

## Results
F1-score for each feature when used alone:

| Feature | F1-score |
|---------|----------|
| N       | 0.1008   |
| P       | 0.0940  |
| K       | **0.1356** |
| ph      | 0.0675   |

**Most important feature**: `K` (Potassium content in soil)

## Requirements
To run this project, install the dependencies:

```bash
pip install -r requirements.txt
```

## Usage

Run the Jupyter Notebook:

```bash
jupyter notebook Crop_Prediction.ipynb

