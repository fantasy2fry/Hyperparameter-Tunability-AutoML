# Hyperparameter-Tunability-AutoML

## Project Overview
The goal of this project is to analyze the tunability of hyperparameters of three selected machine learning algorithms (e.g., XGBoost, Random Forest, Elastic Net) on at least four datasets. The project involves applying a minimum of two different techniques for hyperparameter tuning and evaluating their effectiveness.

## Objectives
- **Analyze the tunability of three machine learning algorithms** using different hyperparameter tuning techniques.
- **Compare the performance of tuning methods** using uniform sampling techniques (e.g., Grid Search, Random Search) and Bayesian optimization.
- **Assess the stability** of the optimization process by evaluating the number of iterations required to reach stable results.
- **Determine the tunability** of specific algorithms and individual hyperparameters based on the collected tuning data.

## Datasets
The analysis will be conducted on at least four different datasets. Specific datasets will be chosen to represent a variety of data types and structures. Details about each dataset will be documented in the `data/` directory.
- [Raisin](https://www.kaggle.com/datasets/nimapourmoradi/raisin-binary-classification?resource=download)
- [Credit Score](https://www.kaggle.com/datasets/conorsully1/credit-score) 

## Hyperparameter Tuning Methods
The project involves the following hyperparameter tuning techniques:
1. **Uniform Sampling Techniques:**
   - Uniform Grid Search
   - Random Search
2. **Bayesian Optimization Techniques:**
   - Using packages like SMAC3 or Scikit-Optimize (with `BayesSearchCV`).

## Methodology
1. **Setup Hyperparameter Grid:** Use a consistent hyperparameter grid for each algorithm across all datasets.
2. **Tuning Techniques:** Implement the selected uniform and Bayesian techniques for each algorithm.
3. **Evaluation:** Analyze the history of the tuning process to determine tunability according to the definitions provided in the reference article: *"Tunability: Importance of Hyperparameters of Machine Learning Algorithms"*.

## Analysis Points
The analysis will focus on the following key aspects:
- Number of iterations required to achieve stable optimization results.
- Definition of hyperparameter ranges for each model, motivated by the literature.
- Comparison of algorithm tunability.
- Analysis of the impact of sampling techniques on the conclusions related to tunability (algorithm and hyperparameter levels).

## Potential Extensions
- Use of statistical tests to compare differences in tuning results between hyperparameter sampling techniques.
- Visualization of results using Critical Difference Diagrams if more sampling techniques are used.
- Additional visualizations and analyses beyond those used in the reference article.

## Project Structure



## Dependencies
- Python 3.x
- Libraries: 
  - `xgboost`
  - `scikit-learn`
  - `scikit-optimize`
  - `SMAC3`
  - `matplotlib`, `seaborn` (for visualization)
  - `numpy`, `pandas` (for data manipulation)

Install the dependencies using:
```bash
pip install -r requirements.txt
```
