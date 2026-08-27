# IMDB Sentiment Analysis - RNN vs LSTM vs GRU

## Project Overview

This project implements a Deep Learning-based Sentiment Analysis system
using the IMDB movie reviews dataset.

The project compares three different Recurrent Neural Network architectures:

- Simple RNN
- LSTM
- GRU

The goal is to classify movie reviews as either Positive or Negative.

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Scikit-learn
- BeautifulSoup
- Matplotlib
- Google Colab

## Dataset

The project uses an IMDB movie reviews dataset containing movie reviews
and their corresponding sentiment labels.

The dataset is cleaned before training by:

- Removing missing values
- Removing duplicate reviews
- Converting sentiment labels to numerical values
- Cleaning HTML tags
- Converting text to lowercase
- Removing extra whitespace

## Data Preprocessing

The text preprocessing pipeline includes:

1. Text cleaning
2. Tokenization
3. Converting text into sequences
4. Padding sequences to a fixed length

The tokenizer keeps the top 25,000 words and the maximum review length
is set to 300 words.

## Models

Three Deep Learning models were implemented:

### 1. Simple RNN

The RNN model consists of:

- Embedding Layer
- SpatialDropout1D
- SimpleRNN
- Dense Layer
- Dropout
- Sigmoid Output Layer

### 2. LSTM

The LSTM model consists of:

- Embedding Layer
- SpatialDropout1D
- LSTM
- Dense Layer
- Dropout
- Sigmoid Output Layer

### 3. GRU

The GRU model consists of:

- Embedding Layer
- SpatialDropout1D
- GRU
- Dense Layer
- Dropout
- Sigmoid Output Layer

## Training

The models are trained using:

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Epochs: 10
- Batch Size: 64
- Early Stopping
- ReduceLROnPlateau
- Model Checkpointing

## Evaluation

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

The project also compares the performance of RNN, LSTM, and GRU using
visualizations for Accuracy and F1-Score.

## Results

The best-performing model is selected automatically based on test accuracy.

The project also generates:

- Classification Reports
- Confusion Matrices
- Accuracy Comparison
- F1-Score Comparison
- Training vs Validation Accuracy
- Training vs Validation Loss

## Prediction

After training, the best model can be used to predict the sentiment
of new movie reviews.

The system returns:

- Predicted Sentiment
- Prediction Confidence

## Saved Files

The project saves:

- Best trained sentiment model
- Tokenizer
- Model configuration
- Model comparison results

## How to Run

1. Open the notebook in Google Colab.
2. Upload the required IMDB dataset.
3. Run the notebook cells sequentially.
4. Train the RNN, LSTM, and GRU models.
5. Compare the model performance.
6. Use the best model for sentiment prediction.

## Project Structure

```text
IMDB-Sentiment-Analysis-RNN-LSTM-GRU/
│
├── IMDB_Sentiment_Analysis.ipynb
├── README.md
└── model_results.csv# IMDB-Sentiment-Analysis-RNN-LSTM-GRU
