# Machine Learning Model Implementation for Solubility Prediction

This project demonstrates a simple machine learning workflow for predicting solubility based on a set of molecular descriptors using two models: **Linear Regression** and **Random Forest**. The goal is to predict the solubility (`logS`) based on molecular features extracted from the dataset.

## Dataset

The dataset used in this project is the **Delaney Solubility with Descriptors** dataset. It contains molecular descriptors (features) and the solubility values (`logS`). The dataset is available on GitHub.

- **Dataset URL**: [Delaney Solubility with Descriptors](https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv)

## Results Interpretation
The scatter plot and model evaluation metrics help us assess the accuracy of the predictions made by both the Linear Regression and Random Forest models. A higher R² value and lower MSE indicate better model performance.

## Conclusion
In this implementation, you compared two regression models, Linear Regression and Random Forest, for predicting the solubility of compounds. Based on the evaluation metrics, you can determine which model performs better on this particular dataset.

## Steps Involved

### 1. **Load Data**
The dataset is loaded using `pandas` from a URL, which is stored in a DataFrame for further processing.

```python
import pandas as pd
df = pd.read_csv('https://raw.githubusercontent.com/dataprofessor/data/refs/heads/master/delaney_solubility_with_descriptors.csv')
df
