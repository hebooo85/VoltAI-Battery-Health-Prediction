# VoltAI – Battery Health Prediction

## 1. Problem Statement
Lithium-ion battery degradation significantly impacts electric vehicle reliability, safety, and maintenance costs.  
This project predicts:
- State of Health (SOH)
- Remaining Useful Life (RUL)

## 2. Business Impact
- Enables predictive maintenance strategies  
- Reduces unexpected battery failures  
- Improves EV fleet optimization  
- Supports data-driven maintenance planning  

## 3. Dataset
NASA Battery Aging Dataset  
Cycle-level structured data with group-aware validation to prevent data leakage.

## 4. Methodology
- Data preprocessing and cleaning  
- Feature engineering (cycle-level + lag features)  
- Standardization for scale-sensitive models  
- GroupKFold cross-validation  
- Hyperparameter tuning  

### Models Implemented
- Linear Regression  
- Random Forest  
- Support Vector Regression (SVR)  
- XGBoost  

## 5. Model Evaluation

Evaluation Metrics:
- RMSE (Root Mean Squared Error)  
- MAE (Mean Absolute Error)  
- R² Score  

**Best Performing Model:** XGBoost  
**Cross-Validation Strategy:** GroupKFold  

## 6. Explainability
- SHAP analysis used to interpret feature importance  
- Identifies key degradation drivers such as voltage, temperature, and capacity  

## 7. Tools & Technologies
- Python  
- Scikit-learn  
- XGBoost  
- Pandas / NumPy  
- SHAP  
- Jira (Agile project management)  

## 8. Project Structure
- `VoltAI_Sprint1.ipynb`  
- `battery_cycle_level_dataset_CLEAN_FINAL.csv`  
- `Project Backlog.png`  
- `Sprint1 Backlog.png`  

## 9. Future Improvements
- LSTM-based temporal modeling  
- Deployment using Streamlit  
- Model monitoring framework  

