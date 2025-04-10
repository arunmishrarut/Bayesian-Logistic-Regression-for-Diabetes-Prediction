# Bayesian-Logistic-Regression-for-Diabetes-Prediction
This project explores the application of Bayesian Logistic Regression for binary classification, using a real-world dataset to predict diabetes outcomes. Developed as part of a statistical modeling course, the project delves into the theory, implementation, and performance evaluation of Bayesian approaches using MCMC sampling.

📊 Project Overview
Bayesian logistic regression allows incorporation of prior beliefs into the modeling process using Bayes’ theorem. In this project, we:

Implement Bayesian logistic regression using stan_glm from the rstanarm package in R.

Compare model performance across various prior distributions (Normal, Uniform, Cauchy, Student-t).

Apply data preprocessing, normalization, and variable selection.

Use diagnostic tools like Posterior Predictive Checks, Cross-Validation, and Posterior Distributions.

📁 Dataset
The dataset originates from the Pima Indians Diabetes Database, containing diagnostic measurements to determine diabetes status. After cleaning, 392 records remained with the following predictors:

Pregnancies

Glucose

Blood Pressure

Skin Thickness

Insulin

BMI

Diabetes Pedigree Function

Age

🧪 Methods
Model Training
Four Bayesian models were trained with different priors:

Normal

Uniform

Cauchy

Student-t

Additionally, a baseline model (intercept only) and a subset model (selected predictors only) were created for comparison.

Evaluation
Model evaluation techniques included:

Posterior Predictive Checks (pp_check)

Posterior Distributions and Credible Intervals

Leave-One-Out Cross-Validation (loo)

Confusion Matrix and Classification Accuracy

✅ Results
All Bayesian models achieved an accuracy of ~78%, with the subset model reaching 80% accuracy and 75% balanced accuracy.

Predictors with the most influence: Glucose, BMI, DiabetesPedigreeFunction, and Age.

Model performance did not vary significantly across different prior choices.

🔧 Tools & Libraries
R (with rstanarm, bayesplot, loo)

MCMC sampling with Hamiltonian Monte Carlo

Data Cleaning and Normalization

📈 Conclusion
Bayesian logistic regression is a robust approach for binary classification tasks, with flexible model construction and interpretability. While priors did not drastically affect outcomes in this case, future work could explore more complex datasets and hyperparameter tuning.

👥 Team
Anitej Biradar

Arun Mishra

Fangru Linghu

📚 References
Literature Cited
1. Vehtari, A., Gelman, A., & Gabry, J. (2017). Bayesian logistic regression with rstanarm. Kaggle.
   Retrieved from https://www.kaggle.com/code/avehtari/bayesian-logistic-regression-with-rstanarm/notebook
2. Zhang, L. (n.d.). Statistical Learning with R. Kaggle.
   Retrieved from https://www.kaggle.com/code/laozhang/statistical-learning-with-r?scriptVersionId=445129
3. UCI Machine Learning Repository. (n.d.). Pima Indians Diabetes Database.
   Retrieved from https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database
4. RStanArm Development Team. (2021). rstanarm: Bayesian Applied Regression Modeling via Stan.
   Retrieved from https://mc-stan.org/rstanarm/
6. Goodrich, B., Gabry, J., Ali, I., & Brilleman, S. (2021). rstanarm: Bayesian applied regression modeling via Stan (Version 2.26.1) [Computer software manual].
   Retrieved from https://cran.r-project.org/web/packages/rstanarm/vignettes/rstanarm.html
8. Gabry, J., & Mahr, T. (2021). Bayesplot: Plotting for Bayesian models (Version 1.8.1) [Computer software manual].
   Retrieved from https://mc-stan.org/bayesplot/
10. Vehtari, A., Gelman, A., & Gabry, J. (2021). Glossary of Terms in the Bayesian Workflow. LOO: Leave-One-Out Cross-Validation and Related Estimators.
    Retrieved from https://mc-stan.org/loo/reference/loo-glossary.html
11. Stan Development Team. (2021). pp_check.stanreg: Posterior predictive checks for Bayesian regression models.
    Retrieved from https://mc-stan.org/rstanarm/reference/pp_check.stanreg.html
12. [Pima Indians Diabetes Dataset on Kaggle
    Retrieved from https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database
