# datascience
regression problem

This project focuses on solving a regression problem: estimating the coordinates of a particle as it passes through a sensor plane. Several machine learning models were trained and evaluated to predict the particle’s position. The study explores the contribution of dataset features to model performance and compares predictions based on the average Euclidean distance, identifying the model that provides the most accurate position estimation.

# Particle Position Estimation (Regression Project)

#Overview
This project addresses a regression problem: predicting the position of particles passing through a sensor plane using extracted signal features.  
The objective is to train regression models and evaluate them using the **average Euclidean distance** metric.

#Dataset
- **Features per signal:**
  - PMAX (positive peak magnitude, mV)  
  - NegPMAX (negative peak magnitude, mV)  
  - Tmax (positive peak delay, ns)  
  - Area (area under signal)  
  - RMS (root mean square value)  
- Hardware limitations: only **12 out of 18 records** per particle are valid.  
- Total: **19 numerical columns**.

#Methods
- Feature selection using **mean** and **variance** analysis  
- Models tested:
  - 🌲 **Random Forest Regression**  
  - 📐 **Ridge Regression**  
- Hyperparameter tuning via **grid search**

#Results
- **Random Forest Regression** (best model)  
  - Test set: **4.662**
  - Evaluation set: **5.437**  
- **Ridge Regression**  
  - Test set: **17.739**  
- Feature importance analysis revealed redundancy in some attributes.

#How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/shadimahboub/datascience/project

 


