# Bank marketing campaigns analysis
Compare classification models to predict if a prospect will subscribe a deposit from a marketing campaign 

## Dataset
- The CSV dataset can be found here: data/bank-additional-full.csv and orginially comes from the UCI Machine Learning repository.
- Explanations can be found here: data/bank-additional-names.txt
- It contains more than 40,000 entries representing the results of marketing campaigns conducted between 2008 and 2010

## Notebook and Repository
- The data mining and the comparison between classifiers can be found in the "prompt_III.ipynb" notebook. 
- Git Repository is located at https://github.com/olsc78/bank-mkt.git

## Summary of findings

### Data
The data exploration analysis revealed that the dataset was clean with only a few duplicates and the need to deal with 'unknown' values for some features.
The main specificity of the dataset is its imbalance towards the negative class resulting in a misleading high accuracy of most models.

### Models
Several models have been tested (Logistic regressions, K Nearest Neighbors, Decision Trees and Support Vector Machines) with a grid search of various hyperparameters.

### Findings
- Dataset is imbalanced and needed some strategies to circumvent
- Metrics to focus on were ROC AUC and recall in order to find more true positives with the risk of increasing false positives
- KNN and SVM perform better, with KNN being faster and SVM being able to explain the importance of certain features with respect to a conversion, such as the duration of the call or the month of the call 
