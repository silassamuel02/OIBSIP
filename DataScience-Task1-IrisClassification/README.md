# Iris Flower Classification 🌸

## Project Overview
This project uses machine learning to classify Iris flowers into three species: Setosa, Versicolor, and Virginica, based on their sepal and petal measurements.

## Dataset
- **Source:** Scikit-learn Iris dataset
- **Samples:** 150
- **Features:** 4 numerical measurements
- **Target classes:** Setosa, Versicolor, Virginica
- **Missing values:** None

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

## Models Compared

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 93.33% |
| K-Nearest Neighbors (KNN) | 93.33% |
| Support Vector Machine (SVM) | 96.67% |

## Results
The Support Vector Machine achieved the highest test accuracy of **96.67%**, correctly classifying 29 out of 30 test samples.

Exploratory data analysis also showed that petal length and petal width were useful for distinguishing between the species.

## How to Run
1. Clone or download this repository.
2. Activate the project's Python virtual environment.
3. Install the required libraries if they are not already installed.
4. Open `iris_classification.ipynb` in VS Code or Jupyter Notebook.
5. Run all cells from top to bottom.

## Conclusion
SVM performed best among the three tested models on the selected train-test split. Cross-validation could provide a more reliable estimate of performance on unseen data.
