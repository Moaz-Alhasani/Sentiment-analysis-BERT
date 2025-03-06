#Sentiment Analysis using BERT

This project implements sentiment analysis using a pre-trained BERT model from Hugging Face's transformers library. The model predicts sentiment on a scale from 0 (very negative) to 4 (very positive).

#Features

Uses nlptown/bert-base-multilingual-uncased-sentiment, a multilingual BERT model for sentiment analysis.

Tokenizes input text using BertTokenizer.

Performs inference using BertForSequenceClassification.

Outputs sentiment scores and labels.

#Installation

To run this project, install the required dependencies:

pip install torch transformers

#How It Works

Loading the Model & Tokenizer: The script loads a pre-trained BERT model and its corresponding tokenizer to process text inputs.

Tokenization: The input text is tokenized using BertTokenizer, ensuring it is properly formatted for the model.

Inference: The tokenized text is passed to the BertForSequenceClassification model to generate sentiment predictions.

Softmax Application: The output logits from the model are converted into probability scores using the softmax function.

Sentiment Classification: The highest probability score determines the sentiment class, which is mapped to one of five categories: very negative, negative, neutral, positive, or very positive.

Result Display: The script prints the sentiment score, label, and probability distribution for better interpretation.
