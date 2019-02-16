# Automated_Essay_Scorer

# Pre-requisites :
* Pandas
* Numpy
* Natural language toolkit(nltk)
* Gensim for Word2vec
* Scikit-learn
* Keras

# Models used in training:

* Linear Regressor
* Gradient Boosting Regressor
* Support Vector Regressor
* Long Short Term Memory(LSTM)

# Evaluation metric

* Mean squared error
* Variance
* Cohen Kappa score

# Approach: 

Here, Word2vec model is used to generate word embeddings on which the whole model relies to predict the scores. Before generating word vectors, essays given in the essay sets are cleaned(removing stopwords, punctuations, special symbols etc.) and then word vectors are created so as to feed it to the word2vec model for generating word embeddings.After that, model is trained on various regression algorithms and each is avaluated on the basis of certain evaluation metric.


# Installation :

1. Install all the packages which are mentioned above using the following command:

'''
pip install keras
pip install numpy
pip install pandas
pip install sklearn
pip install gensim
pip install nltk
'''

2. Run the essay_scorer.py file in jupyter notebook.
3. Have a cup of coffee and wait for the models to generate their respective mean squared error values, variances, cohen kappa scores.

# Conclusion : 

Out of all the models that were trained and tested, LSTMs outperform all other models and hence the same is used to generate scores for the final dataset.
