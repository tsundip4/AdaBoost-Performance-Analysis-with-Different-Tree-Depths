This is an implementation of ADAboost for boosting our general Decision Tree classifier. The code tests how decision tree depth affects AdaBoost classifier performance on breast cancer data using cross-validation.


--Datasets--
Wisconsin Breast Cancer Dataset (30 features, binary classification)
569 samples (malignant/benign tumors)
Preloaded from scikit-learn

--The Experiment--
We test AdaBoost with 20 decision trees at different depths:
Depths tested: 1, 2, 3, 4, 5
Each configuration evaluated with 10-fold cross-validation
Performance measured by accuracy

---What You'll See--
A line plot showing:
X-axis: Decision tree depth (1-5)
Y-axis: Cross-validation accuracy
Key insight: Which tree depth gives the best performance

---why this matters--
You'll see a clean plot showing accuracy scores for each tree depth. Typically, shallow trees (depth 1-2) are too simple and underperform, while depth 3-4 often hits the sweet spot of capturing patterns without overfitting. Depth 5 might show similar or slightly worse performance as trees become too specialized.

--Conclusion--
The beauty of AdaBoost is how it combines multiple weak learners (our decision trees) to create a strong classifier. Even simple "decision stumps" (depth=1 trees) can form an effective ensemble when properly weighted and combined.

*** Run in Google Colab***


