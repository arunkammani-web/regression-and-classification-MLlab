# Retail Response Modeling with Regression and Support Vector Machines

A compact machine learning project that explores how different supervised learning methods capture different data structures.

This repository demonstrates three complementary modelling scenarios:

- **Linear trend modelling** with Ordinary Least Squares regression
- **Curvilinear trend modelling** with polynomial regression
- **Binary classification in 3D feature space** with a linear Support Vector Machine

The project is designed as a clean showcase of model selection: when the data are approximately linear, a simple regression model is appropriate; when the relationship bends, polynomial features improve fit; and when the goal changes from prediction of a continuous outcome to separation of two classes, a max-margin classifier becomes the right tool.

## Project overview

This project brings together three supervised learning workflows:

1. **Linear response modelling**  
   A straight-line relationship is fitted between an input variable and a continuous response using Ordinary Least Squares.

2. **Non-linear trend analysis**  
   A U-shaped response pattern is modelled using polynomial regression, showing why a linear specification can be structurally inadequate.

3. **Margin-based classification**  
   A synthetic three-dimensional dataset is classified using a linear Support Vector Machine, with evaluation through a confusion matrix and geometric visualisation of the decision plane.

## Repository structure

```text
.
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
├── src/
│   ├── linear_trend.py
│   ├── nonlinear_trend.py
│   └── svm_boundary.py
├── figures/
├── docs/
└── notebooks/
```

## Installation

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

On Windows:

```bash
.venv\\Scripts\\activate
```

## Usage

```bash
python src/linear_trend.py
python src/nonlinear_trend.py
python src/svm_boundary.py
```

## Outputs

The scripts generate model outputs and visualisations such as:

- fitted regression lines
- polynomial response curves
- confusion matrix plots
- 3D SVM decision boundary visualisations

Store screenshots or exported plots in the `figures/` directory to make the repository easier to browse.

## Methods used

- Ordinary Least Squares regression
- Polynomial feature expansion with linear regression
- Linear Support Vector Machine classification
- Confusion matrix, precision, recall, and F1-score evaluation

## Tech stack

- Python
- NumPy
- Matplotlib
- scikit-learn

## License

This project is released under the MIT License.
