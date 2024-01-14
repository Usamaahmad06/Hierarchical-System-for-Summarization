# Hierarchical-System-for-Summarization
Natural Language Processing Assignment 2
## Overview
This assignment presents an implementation of a Hierarchical System for Text Summarization using Natural Language Processing (NLP) techniques. This system utilizes tokenization, stemming, and cosine similarity to generate concise summaries from input documents. The goal is to provide an efficient and effective approach for extracting key information from large textual datasets.

## Code Structure
### Dependencies
Before running the code,we have to ensure that required dependencies installed:

import nltk
nltk.download('punkt')
nltk.download('stopwords')
### Modules
preprocess_text: This module tokenizes and preprocesses input text by removing stopwords and applying stemming.

sentence_similarity: Computes cosine similarity between two preprocessed sentences.

generate_summary: Generates a summary for a set of sentences based on sentence similarity scores.

hierarchical_summarization: Implements a hierarchical summarization approach, iteratively generating summaries for multiple steps.

## Usage Example
summary_size = 5
num_steps = 10

#### Provide your input documents to the 'documents' variable
final_summaries = hierarchical_summarization(documents, summary_size, num_steps)

#### Display summaries
for i, summary in enumerate(final_summaries):
    print(f"Summary for document {i + 1}:\n{summary}\n")
## How to Use
Ensure dependencies are installed.
Input your documents into the documents variable.
Adjust summary_size and num_steps parameters as needed.
Run the script to obtain hierarchical summaries.
## Important Considerations
The effectiveness of the summarization heavily relies on the quality and nature of the input documents. It is recommended to fine-tune parameters and preprocess the input data accordingly.
## Acknowledgments
The implementation incorporates various NLP techniques and libraries, including NLTK
