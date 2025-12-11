
## Logistic Regression — Effect of L2 Regularisation on Decision Geometry

## Overview

This repository contains the implementation and experimental materials for a university-level Machine Learning coursework project examining how L2 regularisation influences the decision geometry of logistic regression models. The study focuses on the inverse regularisation parameter C and analyses its effect on weight magnitude, margin width, decision boundary smoothness, and predictive calibration.

The repository accompanies a written tutorial submitted as a PDF or webpage and is designed to be fully reproducible.

## Project Objective

The objective of this project is to provide a focused and interpretable analysis of the role of L2 regularisation in logistic regression. Rather than comparing multiple models, the study isolates a single internal mechanism and investigates how regularisation strength shapes the geometric and probabilistic behaviour of the classifier.

Specifically, the project examines:

Decision boundary geometry under varying regularisation strengths

The relationship between weight norm and margin width

Effects on probability calibration measured via log loss

Locations and causes of classification failures

## Repository Structure

notebooks/
24092678.ipynb
Contains the Jupyter notebook used to generate all experimental results and figures.

figures/
Stores the plots produced by the experiments, including decision boundaries, performance trends, and error visualisations.

report/
Contains the final written tutorial in PDF or web page format, including figures and references.

data/
No external data files are required. All datasets are generated programmatically using scikit-learn.

## Dataset

The experiments use a synthetic two-dimensional binary classification dataset generated with scikit-learn. The dataset includes overlapping classes and label noise, enabling direct visual analysis of decision geometry and regularisation effects. Stratified training, validation, and test splits are applied to ensure balanced evaluation.

## Experimental Design

Logistic regression models are trained using an L2 penalty with varying values of the inverse regularisation parameter C. All other hyperparameters are held constant. Evaluation metrics include accuracy, macro-averaged F1 score, log loss, and weight vector norm. Decision boundaries and misclassification patterns are visualised to support geometric interpretation.

## Reproducibility

All experiments are fully reproducible. Running the notebook from start to finish regenerates all reported figures and metrics. Random seeds are fixed, and no manual preprocessing steps are required.

## Requirements

The implementation relies on standard Python scientific computing libraries, including NumPy, Matplotlib, and scikit-learn. No external datasets or specialised hardware are required.

## Usage

Read the written report in the report/ directory to understand the theoretical motivation and findings.

Run the Jupyter notebook in the notebooks/ directory to reproduce all experiments and figures.

Review the figures in the figures/ directory alongside the reported analysis.

## License

This project is released under an open-source license for educational and non-commercial use. See the LICENSE file for details.
