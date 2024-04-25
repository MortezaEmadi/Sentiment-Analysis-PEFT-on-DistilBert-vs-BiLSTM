# Sentiment Analysis and Text Generation for Enhanced Customer Service on Social Media

## Overview

This project leverages advanced NLM techniques to analyze and generate text based on social media data. It targets specifically Twitter interactions with customers, where understanding and responding to user sentiments efficiently can greatly enhance customer engagement and brand perception. This is particularly valuable in sectors like airlines, where public opinion can significantly influence business success. Also, the primary focus of this phase was to explore methods for conveniently enhancing accuracy.

## Features

- **Sentiment Analysis:** Utilizes a fine-tuned DistilBERT model enhanced with Low-Rank Adaptation (LoRA) to accurately interpret sentiments from tweets. This component is crucial for tailoring responses in customer service scenarios.
- **Text Generation:** Implements a combined RNN-GRU and N-gram model suited for generating short, context-rich responses typical in social media interactions.
- **Adaptability:** Designed to be versatile across different platforms and regional requirements, by enhancing this AI module it can play a great role as an effective CRM tool

## Model Access

The tuned LoRA model, which shows significant improvements in precision, is available for public use and further development on my [Hugging Face profile](https://huggingface.co/your_username/your_model).

## Project Details

- **Dataset:** Uses the Sentiment140 dataset containing 1.6 million tweets, though due to time constraints, only 15,000 tweets were used for training. This dataset includes annotations for sentiments which are crucial for our analysis.
- **Challenges:** The project addresses complex sentiment interpretations in tweets, involving nuanced language and emoticons. 

## Technical Approach

1. **Sentiment Analysis:** Fine-tuning of the DistilBERT model using PEFT with a LoRA approach, increasing model precision from 0.47 to 0.78 in just eight epochs. (Due to time and computational limits for the project, <br>I used only 10% of the dataset volume and incorporated a data augmentation.</br> Despite minimal training, the model's accuracy improved by 59.5% in comparison with non-fine tuned DistilBert LLM!)
2. **Text Generation:** Development of a text generation module using RNN-GRU architecture along with N-gram modeling, balancing complexity and performance effectively.

## Evaluation and Enhancement

- **Accuracy Metrics:** Model validation through accuracy, precision, recall, and F1 scores.
- **Future Enhancements:** Potential applications of semi-supervised learning and generative models for data augmentation are discussed, which could further improve the efficiency and applicability of the sentiment analysis. (refer to the report for more discussion on these aspects)
