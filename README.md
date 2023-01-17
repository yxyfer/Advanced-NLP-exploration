# Advanced Natural Language Processing (NLP) -- Hands-on experiments.

This repository contains advanced practicals, complete with papers to explain the jupyter-notebooks and includes more detailed explanations.

Divided into two distinct parts:

  - Keyword Extraction, Word & Sentence Vectors
  - Language detection, semantic spaces, and attention exploration

## Keyword Extraction, Word & Sentence Vectors
This part contains exploration and experiments on keyword extraction and word & sentence vectors. Divided into four sections: 

  - Keywords Extraction
  - Word Vectors
  - Prediction-based Word Vectors
  - Prediction-based Sentence Vectors

The first section comprises advanced data pre-processing followed by multiple keyword extraction models (including a top-N implementation, [tf-idf](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html) and [KeyBERT](https://github.com/MaartenGr/KeyBERT))  benchmarked against one another. 

The following section studies word vectors in an in-depth manner. It includes a distinct words algorithm implementation, a co-occurrence algorithm and a reduction in K dimensions algorithm, which enables plotting the embeddings.

The third section explores Prediction-based word vectors. It studies the Global Vectors for Word Representation ([GloVe](https://github.com/stanfordnlp/GloVe)) model and compares the results with section two. It focuses on studying particular problems and goes in-depth into studying analogies.

The final section studies the [SentenceBERT](https://www.sbert.net) (SBERT) model and benchmarks its clustering abilities using different methods.

An analysis of Bias is conducted throughout this report.

## Language detection, semantic spaces, and attention exploration

This second part contains an implementation of language detection followed by a study of semantic spaces studied with French and English spaces and finishes with a mathematical exploration of attention.

This first section on language detection explores two language detection models on a perfectly distributed dataset. As usual, the first step is to pre-process the data, before using it. The main focus of this section is to train and compare two language detection models a [MultinomialNB](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html) (Multinomial Naive Bayes) trained on the above data and a [FastText](https://fasttext.cc) model trained on the [Tatoeba](https://tatoeba.org/en/) dataset. The accuracy tests for both models use the same data.

The second section focuses on rotating semantic spaces. This section uses Wikipedia datasets (en, fr) as semantic spaces. And the [Muse](https://github.com/facebookresearch/MUSE.git) library is used to align the spaces. The focus then shifts to understanding and studying the results. This includes benchmarks for top-N, top-1 performance, and plots study. 
 
Finally, the first section focuses on the machine learning definition of attention and a mathematical exploration.
