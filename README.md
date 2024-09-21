# LDA Dimensionality Reduction and Classification Project

This project uses Linear Discriminant Analysis (LDA) for dimensionality reduction on a dataset containing university statistics. Two classifiers are employed for predicting whether a university is private or public:
- Logistic Regression
- LDA itself (used as a classifier)

## Project Structure

The project follows these major steps:
1. **Data Preparation:** 
   - A dataset with 17 features and a target variable (`Private`) indicating whether the university is private (`Yes`) or public (`No`) is used.
   
2. **Standardization:**
   - The input features are standardized using a Standard Scaler (mean-centered and variance-normalized).
   
3. **Dimensionality Reduction:**
   - LDA is applied to reduce the data from 17 dimensions to 1 dimension, while preserving the class separability.

4. **Classification:**
   - Two classifiers are employed:
     - **Logistic Regression (LGD):** After reducing the dimensions, logistic regression is used to classify universities.
     - **LDA Classifier:** LDA itself is also used as a classifier.

5. **Evaluation:**
   - The project evaluates both classifiers using standard metrics such as accuracy, precision, recall, F1 score, confusion matrix, ROC and precision-recall curves.

## Key Files

- **Data:** `College.csv` (Data containing 17 numerical features and the target variable `Private`)
- **LDA and Logistic Regression Code:**
  - LDA is applied for dimensionality reduction, followed by classification using both Logistic Regression and LDA.
  - Code for generating scatter plots, confusion matrices, and classification reports.
- **Predictions and Results:**
  - The project creates a DataFrame containing the original data index, the target variable, the projected value (from LDA), the predicted class, and a correctness indicator.

## How to Run the Project

### Prerequisites

Ensure you have Python installed with the following packages:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

### Installation

To install the necessary dependencies, run:

```bash
pip install -r requirements.txt
