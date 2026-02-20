# Workflow

This folder uses the **reduction method** to examine and mitigate potential bias in a machine learning model for hiring prediction. The overall workflow is structured as follows:

1. **Exploratory Data Analysis (EDA)**
   We begin by examining the dataset to understand feature distributions, class balance, correlations, and potential disparities across sensitive groups. This step helps identify initial patterns and informs modeling decisions.

2. **Baseline Model (Unconstrained)**
   We train a standard machine learning model without any fairness constraints. All available features, including sensitive attributes, are included. The model is evaluated using both performance metrics (e.g., accuracy) and fairness metrics (e.g., demographic parity, equal opportunity).

3. **Fairness-Constrained Model (Reduction Method)**
   We apply a reduction-based fairness approach that incorporates fairness constraints during training. Sensitive attributes are used to enforce fairness criteria (rather than simply removed), and the resulting model is evaluated using the same performance and fairness metrics.

4. **Comparison and Analysis**
   We compare the baseline and fairness-constrained models to analyze trade-offs between predictive performance and fairness. Additionally, we compare the reduction method with selected pre-processing and post-processing strategies to understand their relative effectiveness.

