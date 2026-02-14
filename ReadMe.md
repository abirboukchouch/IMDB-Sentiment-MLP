# IMDB Sentiment Analysis using Multi-Layer Perceptron (MLP)

## Overview
This project builds a sentiment classifier for IMDB movie reviews using a Multi-Layer Perceptron (MLP) neural network.

The dataset used is the IMDB 50K Movie Reviews dataset downloaded from Kaggle.

## Feature Engineering
This project uses lexicon-based sentiment features:

- VADER polarity scores (compound, positive, negative, neutral)
- TextBlob polarity score

Each review is converted into 5 numerical features.

## Model Architecture
- Input layer: 5 features
- Hidden Layer 1: 32 neurons (ReLU)
- Dropout: 0.3
- Hidden Layer 2: 16 neurons (ReLU)
- Dropout: 0.2
- Output Layer: 1 neuron (Sigmoid)

Loss Function: Binary Crossentropy  
Optimizer: Adam (learning rate = 0.001)

## Results
Test Accuracy: 78%

Precision, Recall, and F1-score are balanced across classes.

## Files Included
- notebooks/imdb_mlp_sentiment.ipynb
- models/mlp_sentiment_model.h5
- results/evaluation_metrics.txt

## Conclusion
The model achieves approximately 78% accuracy using only lexicon-based sentiment features.

Performance is limited because the model does not use contextual embeddings such as Word2Vec or BERT. Future improvements could include TF-IDF or deep learning language models.

## Author
Abir Boukchouch
