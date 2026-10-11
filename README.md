# ML-model-comparisons
This is solely to revamp my old project from UG.

This project compared four classification algorithms (Logistic Regression, KNN, Decision Tree and Random Forest) on the Breast Cancer dataset from Kaggle to predict patient survival status. After hyperparameter tuning with GridSearchCV and 5-fold cross-validation, Logistic Regression and Random Forest performed best, reaching test accuracies of 87.5% and 87.6%.

However, the dataset is imbalanced (about 87% “Alive”), so a model that always predicts “Alive” would score a similar accuracy. Accuracy therefore overstates performance: recall for the “Dead” class was only 15% for Logistic Regression and 11% for Random Forest, so most deaths were missed.
