#  Data Mining 
## Table of Contents
- [Project Overview]( #Project-Overview)
- [Data Sources](#Data-Sources)
- [Tools ](Tools)
- [Data Cleaning and Pre-processing](#Data-Cleaning-and-Pre-processing)
- [Analysis ](Analysis)
- [Results/Findings ](Results/Findings)
- [Recommendation ](Recommendation)
- [Limitations ](Limitations)
- [REFERENCES](REFERENCES)

### Project Overview
This document describes the analysis of a dataset aimed at predicting epitopes for Trypanosoma cruzi (T. cruzi), a parasite causing Chagas’ disease.
This document presents the analysis of a dataset for predicting epitopes of Trypanosoma cruzi, the cause of Chagas' disease. The dataset includes 49,606 entries and 1,291 features.
 <img width="986" alt="Variable Imbalance" src="https://github.com/user-attachments/assets/fcc468b4-aa59-4c4b-a335-d8ee0bd56d04">
### Data Sources

The primary dataset used for this analysis is the 'prediction_data.csv' file, which includes detailed information about each sample's epitopes associated with the parasite Trypanosoma cruzi.
The primary dataset used for this analysis is the 'df.csv' file, which includes detailed information about each sample's epitopes associated with the parasite Trypanosoma cruzi.

### Tools 
Python - Data Cleaning, Analysis and Prediction
### Data Cleaning and Pre-processing
1. Data Loading and Overview
2. Checking/Handling Missing values 
3. Data cleaning and formatting
4. Feature Reduction
6. Normalisation and Upscaling
###  Analysis
code/features worked with
```python
# Create full pipeline
pipeline_lr = Pipeline([
    ('preprocessing', preprocessing_pipeline),
    ('classifier', classifier1)
```
### Results/Findings
Using the pipeline I developed, predictions on the unseen dataset  revealed that 98.82% of the distribution were predicted as -1, indicating the absence of Linear B-cell epitopes. In contrast, only 1.18% were predicted as 1, indicating the presence of Linear B-cell epitopes. This result highlights how rLinear B-cell epitopes are relatively rare in this dataset.
### Limitations
The use of Principal Component Analysis (PCA) for feature reduction may have led to the loss of important information, potentially impacting the accuracy of predictions
### REFERENCES
1.[Epitope Mapping](https://doi.org/10.1155/2016/6760830)
2.Predictive Data Mining Models by David and Desheng.

