# Sentiment Analysis on Movie Reviews
Sentiment classifier using the rotten tomatoes movie review dataset

The dataset was downloaded from this source:
http://www.cs.cornell.edu/People/pabo/movie-review-data/

The performance metric - *Area under the curve (AUC)*. This metric calculates the overall performance of a classification model based on area under the ROC curve

*Receiver operating characteristic (ROC) curve*: plots the true positive rate (TPR) versus the false positive rate (FPR) as a function of the model’s threshold for classifying a positive

*Accuracy* - (TP + TN)/(TP+TN+FP+FN)

####  Tokenization - Count Vectorizer

| Techniques        | Accuracy           | AUC  |
| ------------- |:-------------:| -----:|
| Logistic Regression     | 0.8 | 0.81 |
| SGD classifier      | 0.805      |   0.806 |
| SVM | 0.795     |    0.796 |
| SVM | 0.795     |    0.796 |

#### Tokenization - TF-IDF

| Techniques        | Accuracy           | AUC  |
| ------------- |:-------------:| -----:|
| SVM | 0.795     |    0.796 |

#### Vowpal Wabbit

| Accuracy           | AUC  |
| ------------- |:-------------:|
| 0.785     |    0.896 |

#### Deep Learning

| Techniques        | Epochs          | Batch size          | Accuracy           | AUC  |
| ------------- |:-----:|:-----:|:-------------:|-----:|
| LSTM     | 5 | 64 | 0.738 | 0.819 |
| LSTM+Dropout      | 5 | 128 |0.652      |   0.687 |
| LSTM+CNN | 5     | 64 | 0.715 |    0.801 |

TO-DO:
1. Improve preprocessing using [stemming, lemmatization](https://nlp.stanford.edu/IR-book/html/htmledition/stemming-and-lemmatization-1.html) and stop-words
2. Lean more about Deep learning NLP application and make more robust architecture
