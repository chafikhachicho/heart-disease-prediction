# Heart Disease Prediction

A machine learning project in Python that predicts whether a patient has heart disease from medical test results.

## Dataset
Cleveland Heart Disease dataset (UCI), about 300 patients with 13 features such as age, cholesterol, chest pain type and maximum heart rate. The target column is `condition` (heart disease present or not).

## Method
- Stratified 80/20 train/test split (`random_state=42`), giving 60 test patients
- Preprocessing with `StandardScaler` in a scikit-learn `Pipeline`
- Four models compared: KNN, Decision Tree, Random Forest and Logistic Regression
- For KNN, I tested K from 1 to 49 (default K=5 used in the model comparison)

## Results

| Model | Accuracy |
|---|---|
| Logistic Regression | 91.67% |
| KNN | 90.00% |
| Random Forest | 86.67% |
| Decision Tree | 78.33% |

## Limitations
The test set is small (60 patients), and results come from a single split without cross-validation. Random Forest and Decision Tree scores can vary between runs. This is a learning project and is not for medical use.

## Files
- `heart_cleveland_upload.ipynb`: the notebook with all the code
- `heart_cleveland_upload.csv`: the dataset

## Tools
Python, pandas, scikit-learn, matplotlib
