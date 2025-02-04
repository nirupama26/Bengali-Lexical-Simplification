Bengali Lexical Simplification using BERT

Overview

This project focuses on Bengali Lexical Simplification using BERT-based models, particularly XLM-RoBERTa. The system identifies complex words in Bengali text and suggests simpler alternatives using semantic similarity, word frequency, Named Entity Recognition (NER), Part-of-Speech (POS) tagging, and contextual probability.

By leveraging pre-trained transformer models and additional helper functions, the system improves text accessibility, aiding language learners, individuals with cognitive difficulties, and general users who seek a more readable version of Bengali text.

Features

Complex Word Identification: Detects difficult words based on word frequency, syllable count, and length.

BERT-Based Simplification: Uses XLM-RoBERTa to predict simpler alternatives.

Helper Functions: Enhances predictions by integrating semantic similarity checks, word embeddings, NER, POS tagging, and contextual constraints.

Multi-Domain Evaluation: Tested on datasets from news articles, general Bengali text, and scientific literature.

Performance Metrics: Evaluates accuracy using precision, recall, F1-score, and qualitative analysis.

Technologies Used

Python

Hugging Face Transformers (XLM-RoBERTa, BERT)

NLTK & SpaCy for NLP Processing

Pandas & NumPy for Data Handling

Word Embeddings & Frequency Dictionaries

Installation

Clone the repository:

git clone https://github.com/your-repo/bengali-lexical-simplification.git
cd bengali-lexical-simplification

Install dependencies:

pip install -r requirements.txt

Download necessary NLP models:

import nltk
nltk.download('punkt')
nltk.download('averaged_perceptron_tagger')

Usage

Run the main script:

python simplify_text.py --input sample_text.txt --output simplified_text.txt

Specify constraints:

python simplify_text.py --use_ner --use_pos --use_embeddings

Evaluation & Results

Comparisons between BERT models (Sagor-Sarker Bangla BERT vs. XLM-RoBERTa)

Performance with and without helper functions

Qualitative assessment based on human evaluation

Future Enhancements

Fine-tuning BERT on Bengali-specific lexical simplification datasets

Improving handling of idiomatic expressions and multi-word phrases

Expanding evaluation metrics to include SARI and BLEU scores

Contributors

Nirupama Patra (Lead Developer)

Open to contributions from the community!

License

This project is open-source and available under the MIT License.

Contact

For queries or collaborations, reach out via email or open an issue on GitHub.
