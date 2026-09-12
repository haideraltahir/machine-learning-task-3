```markdown
# House Price Prediction: Model Validation & Hyperparameter Tuning

## Overview
This repository contains the implementation of a professional machine learning workflow focused on model reliability, validation, and optimization[cite: 1]. Using the California Housing Dataset, the project demonstrates how to detect overfitting in base models, establish trustworthy performance metrics using Cross-Validation, and optimize model parameters using `GridSearchCV`[cite: 1].

## Key Learning Outcomes & Implementation
* **Overfitting Detection:** Analyzed the performance gap between training and testing data using an unconstrained Decision Tree Regressor[cite: 1].
* **Cross-Validation:** Replaced single train-test splits with 5-Fold Cross-Validation (`cv=5`) to derive stable and realistic performance estimates[cite: 1, 2].
* **Hyperparameter Tuning:** Automated the search for optimal tree constraints (`max_depth` and `min_samples_split`) utilizing `GridSearchCV`[cite: 1, 2].
* **Model Evaluation:** Benchmarked the optimized model against baseline linear models using Root Mean Squared Error (RMSE) and R² Score metrics[cite: 1].

## Tech Stack & Libraries
* **Language:** Python[cite: 1]
* **Environment:** Jupyter Notebook[cite: 1]
* **Data Manipulation:** `pandas`, `numpy`[cite: 1]
* **Machine Learning:** `scikit-learn`[cite: 1]
* **Visualization:** `matplotlib`[cite: 1]

## Repository Structure
* `AI_ML_Task3_Model_Validation_Tuning.ipynb`: The core Jupyter Notebook containing the end-to-end data processing, model training, cross-validation, and tuning workflow[cite: 1, 2].

## Final Model Comparison
The systematic tuning process successfully mitigated overfitting and produced a model that significantly outperforms standard linear algorithms[cite: 1]. Below is the final performance comparison on the test dataset[cite: 2]:

| Model | RMSE | R² Score |
| :--- | :--- | :--- |
| Linear Regression | 0.745581 | 0.575788 |
| Ridge Regression | 0.745554 | 0.575819 |
| **Tuned Decision Tree** | **0.645430** | **0.682099** |

*Note: The Tuned Decision Tree achieved its optimal performance with `max_depth` set to 10 and `min_samples_split` set to 10*[cite: 2].

## How to Run the Project
1. **Clone the repository:**
   ```bash
   git clone <your-repository-url>
   cd <repository-folder>

```

2. **Activate your virtual environment (recommended):**
* Windows: `venv\Scripts\activate`
* Linux/Mac: `source venv/bin/activate`


3. **Install required dependencies:**
```bash
pip install pandas numpy matplotlib scikit-learn jupyter

```


4. **Launch Jupyter Notebook:**
```bash
jupyter notebook

```


5. Open `AI_ML_Task3_Model_Validation_Tuning.ipynb` and run the cells sequentially to reproduce the validation and tuning results.



```

```
