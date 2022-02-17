# Fake-New-LSTM
## Table of Content
  * [Overview](#overview)
  * [Technical Aspect](#technical-aspect)
  * [Technologies Used](#technologies-used)

## Overview
This is a Fake News Classifier which uses Word Embedding & [LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/).  

## Technical Aspect
Dataset Link: https://www.kaggle.com/c/fake-news/data?select=train.csv  
Given below are the steps taken to build the model:  
For the NLP implementation code –  
  - Imported the following **Python libraries** 
      - Pandas
      - import tensorflow
      - from tensorflow.keras.layers import [Embedding](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Embedding)
      - from tensorflow.keras.preprocessing.sequence import [pad_sequences](https://www.tensorflow.org/api_docs/python/tf/keras/preprocessing/sequence/pad_sequences)
      - from tensorflow.keras.models import [Sequential](https://www.tensorflow.org/api_docs/python/tf/keras/Sequential)
      - from tensorflow.keras.preprocessing.text import [one_hot](https://www.tensorflow.org/api_docs/python/tf/one_hot?hl=en)
      - from tensorflow.keras.layers import [LSTM](https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTM)
      - from tensorflow.keras.layers import [Dense](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Dense)
      - nltk
      - re
      - from nltk.corpus import stopwords
      - from nltk.stem.porter import PorterStemmer
      - numpy
      - from sklearn.model_selection import train_test_split
      - from sklearn.metrics import confusion_matrix, accuracy_score
  -	Imported the Dataset, dropped rows containing missing data, reset the index.
  -	In **Data cleaning** & **Text pre-processing** Section, we removed all unnecessary symbols & numbers. We lower cased all sentences & split sentences into words.
  -	Performed **removal of stopwords** and **Stemming**.
  -	Performed **One Hot Representation** of each Sentence.
  -	Created the **Embedding Representation** of each Sentence.
  -	Created our NN model.
  -	Performed a **train_test_split** on labels & messages.
  -	Trained & tested the model.
  -	**Accuracy = 91%**
      
## Technologies Used
- Jupyter Notebook
-	ML model: LSTM Model
-	Libraries: pandas, numpy, re, nltk, tensorflow, sk-learn.
