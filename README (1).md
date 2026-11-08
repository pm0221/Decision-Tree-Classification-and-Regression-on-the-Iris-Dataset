# Decision Tree Classification and Regression on the Iris Dataset

## Project Overview

This Data Analytics (DA) project demonstrates two supervised machine learning tasks using the **Iris dataset** from `scikit-learn`:

1. **Classification:** A Decision Tree Classifier using the CART approach with the Gini impurity criterion predicts the Iris flower species.
2. **Regression:** A Decision Tree Regressor predicts petal length using the other three flower measurements.

The work is implemented in the Jupyter Notebook `exp7_DA.ipynb`.

## Dataset

The project uses the built-in Iris dataset provided by `sklearn.datasets.load_iris()`.

The dataset contains measurements for three Iris species:

- Setosa
- Versicolor
- Virginica

The four input features are:

- Sepal length
- Sepal width
- Petal length
- Petal width

No separate dataset download is required.

## Project Workflow

### 1. Classification

- Load the Iris dataset.
- Use all four measurements as input features and the species labels as the target.
- Split the data into training and testing sets using a 70:30 ratio (`test_size=0.3`) and `random_state=42`.
- Train a `DecisionTreeClassifier` with:
  - Criterion: `gini`
  - Maximum depth: `3`
  - Random state: `40`
- Predict the species for the test data.
- Evaluate the model using:
  - Accuracy score
  - Confusion matrix
  - Classification report (precision, recall, and F1-score)
- Plot the trained decision tree.

### 2. Regression

- Load the Iris dataset.
- Use sepal length, sepal width, and petal width as input features.
- Use petal length as the target variable.
- Split the data into training and testing sets using a 70:30 ratio (`test_size=0.3`) and `random_state=42`.
- Train a `DecisionTreeRegressor` with:
  - Maximum depth: `3`
  - Random state: `40`
- Predict petal length for the test data.
- Evaluate the model using:
  - Mean Squared Error (MSE)
  - R-squared (R²) score

## Technologies and Libraries

- Python
- Jupyter Notebook
- scikit-learn
- Matplotlib

The notebook imports the following scikit-learn modules and metrics:

- `load_iris`
- `train_test_split`
- `DecisionTreeClassifier`
- `DecisionTreeRegressor`
- `accuracy_score`
- `confusion_matrix`
- `classification_report`
- `mean_squared_error`
- `r2_score`

## Getting Started

### Prerequisites

Install Python 3 and Jupyter Notebook, or use JupyterLab / VS Code with notebook support.

### Installation

Install the required libraries:

```bash
pip install scikit-learn matplotlib notebook
```

### Run the Project

1. Download or clone this project.
2. Open `exp7_DA.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
3. Run the notebook cells from top to bottom.

## Expected Outputs

When the notebook is executed, it displays:

- The first five Iris feature rows and target labels.
- Classification accuracy.
- Classification confusion matrix.
- Classification precision, recall, and F1-score report.
- A visual plot of the trained Decision Tree Classifier.
- Regression Mean Squared Error.
- Regression R-squared score.

Exact metric values are not listed here because they are produced when the notebook is run.

## Project Structure

```text
.
├── exp7_DA.ipynb
└── README.md
```

## Learning Outcomes

- Understand the difference between classification and regression.
- Apply Decision Tree models to a real dataset.
- Split data into training and testing sets.
- Evaluate a classification model using standard metrics.
- Evaluate a regression model using MSE and R².
- Visualize a trained decision tree.

## Author

Add your name and academic details here if required for submission.
