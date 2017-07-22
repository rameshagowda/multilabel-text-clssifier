High leverl summary for multi label, multi class classifier
-----------------------------------------------------------

1 - Data preprocessing and Data wrangling:
 - Use pivoting to convert multi-class, multi-label data into multi-label, binary class data. this can be done using MultiLabelBinarizer(it is also a One-hot encoder).

2 - Data split - Use train-split / k-fold crsoss validation / stratified(balanced) shuffle split:
 - Have single training/testing dataset.

3 - Use OneVsRestClassifier to solve multi-label data by wrapping these algorithms like LinearSVM or Naive Bayes.
- Tf-Idf vectorizer to convert the string in to numeric value - have appropriate parameters set.
- english stop_words from english Corpus
- Parameter tunning through GridSearchCV

4 - Model Evaluation
- Use precision, recall and f1 score to evaluate the model.
- Accuracy is not suited measure in multilabel scenario
