# Projet_SpamDetection
SMS Spam Detection with Dimensionality Reduction
This project aims to design a high-performance classifier to distinguish between legitimate SMS messages (ham) and unwanted messages (spam). The project explores various Natural Language Processing (NLP) techniques, ranging from traditional vectorization to the use of Deep Learning models and pre-trained language models.

🎯 Project Objectives
Cleaning and Preprocessing: Normalization of raw textual data.

Vectorization: Transformation of text into numerical vectors via TF-IDF.

Dimensionality Reduction: Using an Autoencoder to compress the feature space.

Model Comparison: Evaluation of performance with and without feature selection.

Robust Evaluation: Implementation of Cross-Validation for reliable results.

Advanced NLP: Implementation of a pre-trained BERT model for embedding extraction.

📊 Dataset
The project uses the SMSSpamCollection dataset containing 5,572 messages:

Ham: 4,825 messages (86.6%)

Spam: 747 messages (13.4%)

🛠️ Methodology
1. Text Preprocessing
Each message undergoes the following steps to reduce noise:

Conversion to lowercase.

Removal of non-alphabetic characters (punctuation, numbers).

Removal of English stop words.

Stemming using the Porter Stemmer algorithm.

2. Feature Extraction
TF-IDF: Creation of a matrix with 5,000 features including unigrams and bigrams.

Autoencoder: A neural network compressing the 5,000 input dimensions into a 128-dimension latent space.

3. Classification Models
Logistic Regression: Used as the base classifier on both TF-IDF vectors and BERT embeddings.

BERT (Bidirectional Encoder Representations from Transformers): Extraction of embeddings from the [CLS] token to capture the semantic context of the SMS.
