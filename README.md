# Automated_Essay_Scorer

#REQUIREMENTS :
1. Pandas
2. Numpy
3. Natural language toolkit(nltk)
4. Gensim for Word2vec
5. Scikit-learn
6. Keras

MODELS USED IN TRAINING :

1. Linear Regressor
2. Gradient Boosting Regressor
3. Support Vector Regressor
4. Long Short Term Memory(LSTM)

EVALUATION METRIC :

1. Mean squared error
2. Variance
3. Cohen Kappa score

APPROACH: 

Here, Word2vec model is used to generate word embeddings on which the whole model relies to predict the scores. Before generating word vectors, essays given in the essay sets are cleaned(removing stopwords, punctuations, special symbols etc.) and then word vectors are created so as to feed it to the word2vec model for generating word embeddings.After that, model is trained on various regression algorithms and each is avaluated on the basis of certain evaluation metric.


STEPS TO TRAIN THE MODELS AND GENERATE SCORES AND EVALUATING THEM AGAINST METRICS :

1. Install all the packages which are mentioned above.
2. Run the essay_scorer.ipynb file in jupyter notebook.
3. Have a cup of coffee and wait for the models to generate their respective mean squared error values, variances, cohen kappa scores.

CONCLUSION : 

Out of all the models that were trained and tested, LSTMs outperforms all other models and hence the same is used to generate scores for the final dataset.
