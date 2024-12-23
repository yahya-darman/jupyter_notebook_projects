# Cardio Risk Predictor

## Overview

The **Cardio Risk Predictor** is a machine learning project that evaluates an individual's risk of heart attack based on clinical data. It uses multiple classification models to determine the most accurate predictor for heart attack risk and provides predictions on new input data.

---

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/cardio-risk-predictor.git
   cd cardio-risk-predictor
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the dataset using `kagglehub`:
   ```python
   import kagglehub
   path = kagglehub.dataset_download("nareshbhat/health-care-data-set-on-heart-attack-possibility")
   ```

---

## Usage

1. **Run the script**:
   ```bash
   python main.py
   ```

2. **Load the dataset**:
   The dataset is automatically downloaded using `kagglehub` and loaded into a pandas DataFrame.

3. **Train and Evaluate Models**:
   - Models are trained, and the best one is selected based on accuracy.

4. **Make Predictions**:
   - Use the best model to predict heart attack risks for new data.

---

## Results

The system evaluates several models and outputs their performance metrics. For example:

| Model               | Accuracy |
|---------------------|----------|
| **Gradient Boosting**     | 78.69%    |
| **Bagging**               | 80.33%    |
| **AdaBoost**              | 80.33%    |
| **Decision Tree**         | 81.97%    |
| **MLP**                   | 83.61%    |
| **KNN**                   | 85.25%    |
| **SVM**                   | 85.25%    |
| **Logistic Regression**   | 85.25%    |
| **Random Forest**         | 86.89%    |
| **Extra Trees**           | 86.89%    |
| **Gaussian Naive Bayes**  | **92.60%** |

The best-performing model is saved and used for predictions.

---

## Technologies Used

- **Python**: Core language for implementation.
- **scikit-learn**: For machine learning models and preprocessing.
- **pandas**: For data manipulation.
- **kagglehub**: To download datasets directly from Kaggle.

---

## Acknowledgements

- **Dataset**: [Kaggle Dataset](https://www.kaggle.com/nareshbhat/health-care-data-set-on-heart-attack-possibility).
- **Libraries**: pandas, numpy, scikit-learn, kagglehub, logging

---

## Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

---

## Contact

If you have any questions or suggestions, please feel free to contact:
- Name: Yahya Darman
- LinkedIn: [My LinkedIn Profile](https://linkedin.com/in/yahya-darman)
