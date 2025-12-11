# COE 379L – Project 03  
### Predicting Income Using Classical ML Models, XGBoost, and a Neural Network  
**Author:** Nakul Mody and Jesse Oh  

---

## Project Overview
This project explores an open-ended ML task using the **UCI Adult Income dataset** (http://archive.ics.uci.edu/dataset/2/adult), where the goal is to predict whether an individual's income exceeds $50,000 per year.  
The project compares multiple machine learning approaches:

- Baseline Random Forest using scikit-learn  
- Tuned Random Forest using GridSearchCV  
- XGBoost (if available in the environment)  
- Feed-forward Neural Network (Keras/TensorFlow)

The notebook includes:

- Data cleaning and preprocessing using `ColumnTransformer`
- One-hot encoding for categorical variables
- Training multiple models
- Evaluating each using accuracy, precision, recall, and F1-score
- Feature importance analysis for RF and XGBoost
- Final comparison table of all model performances

---

## Repository Contents

| File | Description |
|------|-------------|
| `Project03.ipynb` | Main Jupyter Notebook containing the full implementation and model comparison |
| `COE_379L_InitialProposal.docx` | Initial project proposal submitted on Dec 1 |
| `Use_of_AI.md` | Documentation of how AI tools were used for coding assistance |
| `README.md` | This file; summary of the project and structure |

---

## Methods & Technologies Used
- **Python**, **scikit-learn**, **pandas**, **numpy**
- **RandomForestClassifier**, **GridSearchCV**
- **XGBoost** (if installed)
- **TensorFlow / Keras** for the neural network
- **ColumnTransformer** + **OneHotEncoder**
- **StandardScaler** for NN preprocessing

---

## How to Run the Notebook
If using the TACC-hosted Jupyter server:

1. Start the Docker Jupyter container  
2. Connect via your TACC credential token  
3. Upload or copy the notebook into your workspace  
4. Run all
   
The notebook expects the following file structure:
data/
adult.csv
Project03.ipynb


`adult.csv` is automatically generated from the provided `.data` and `.test` files in the notebook.

---

## Results Summary
The project compares performance across models.  
Typical outcomes (varies slightly with random seed):

- RF Baseline: ~0.85 accuracy  
- RF Tuned: ~0.855 accuracy  
- XGBoost Baseline: ~0.86 accuracy (if available)  
- Neural Network: ~0.84–0.85 accuracy

Final model rankings are shown in the notebook's results table.

---

## Reproducibility
- All random seeds set via `random_state`  
- Preprocessing handled consistently inside scikit-learn `Pipeline`  
- Data splits fixed using `train_test_split(test_size=0.2, random_state=...)`

---


