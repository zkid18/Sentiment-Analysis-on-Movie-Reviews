# Sentiment Analysis on Movie Reviews
Sentiment classifier using the rotten tomatoes movie review dataset

The dataset was downloaded from this source:
http://www.cs.cornell.edu/People/pabo/movie-review-data/

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

| Techniques        | Accuracy           | AUC  |
| ------------- |:-------------:| -----:|
| LSTM     | 0.8 | 0.81 |
| LSTM+Dropout      | 0.805      |   0.806 |
| LSTM+CNN | 0.795     |    0.796 |
