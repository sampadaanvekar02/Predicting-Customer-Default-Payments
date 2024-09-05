# Predicting-Customer-Default-Payments
Project Objective: The primary objective of the study was to evaluate and compare the effectiveness of different data mining methods in predicting the probability of customer default payments. This is particularly significant in the context of risk management where understanding the likelihood of default can help in making informed decisions

1)Problem Identification : Approach of the Project:
1) Data Preparation
2) Finding answer in the data
3) Building supervised Learning models
4) Finally, Predict default payment.

Background of the Project:
!) Focus on Predictive Accuracy:- Rather than simply classifying customers as either credible or not credible, the study emphasizes the importance of predicting the actual probability of default. This approach provides a more nuanced understanding of risk, allowing for better risk management and more precise decision-making.
2)Sorting Smoothing Method:- To overcome the challenge of estimating the real probability of default. Default on CC Bills payment can result in great financial loss. In order to reduce or even prevent loss of this kinds, bank need to determine appropriate given credit for each
specific client based on their informations.

Data Modelling:-
Objective: Predict if the given client will default on their next payments
Notes:-
1) 30000 observations , 22% base rate.
2) For all the models, 5-fold cross validation is applied
3) We tried different parameters associated with each algorithm and picked the one will the best
evaluation performance.

Algorithms used:
1) SVM
2) Random Forest
3)Neural Networks

Evaluation:- Basically,
SVM draws a boundary to separate different classes of data and tries to maximize the margins between the class and boundaries.
1) Neural Networks
- Multi-Layers perceptron , using propagation to Learn.
- 3 hidden layers (5,10,2 units), learning rate, epoch 500
2) Random Forest
- Ensemble of classification trees
- The models builds many classification trees by taking in different orders of features.
- The forest chooses the classification having the most votes.

Exploratory Data Analysis (EDA):
1) Distribution Plots:
Plot histograms and box plots for numerical features (credit amount, age, bill amounts, previous payments) to understand their distribution.

3) Categorical Analysis:
Use bar charts to analyze the distribution of categorical features (gender, education, marital status) and their default rates.

4) Correlation Analysis:
Compute and visualize correlations between numerical features and the target variable. For example,calculate correlations between credit amount and default, or between previous payment amounts and default.

5) Group Comparisons:
Use bar charts or box plots to compare default rates across different categories (e.g.,education levels ormarital status).

6) Preprocessing Steps:
-- Handling Missing Values: Impute or handle missing values in features. Common strategies include mean imputation for numerical values and mode imputation for categorical values.
-- Normalization/Standardization: Scale numerical features such as credit amount, age, bill amounts, and previous payments to ensure that all features contribute equally to the model training..

7) Feature Engineering:
-- Aggregating Payment History Create summary features from the repayment history, such as average delay, maximum delay, or a count of delayed months.
-- Debt-to-Income Ratio, Calculate ratios like the debt-to-income ratio if income data is available or can be inferred.

8) Predictive Modeling:
Data Splitting: Split the dataset into training and testing sets (e.g., 70% training and 30% testing) to evaluate model performance

9) Interactive Visualizations:
--Tools: Use interactive dashboards in tools Power BI to allow users to explore the data, filter by different features, and drill
down into specifics.

10) Conclusion:
Accuracies yield from all the models are no better than simply predicting all client not to default. Instead , we are AUC as evaluating measure, which is more directly and naturally related to cost/benefit analysis Based on AUC, random forest has best performance
