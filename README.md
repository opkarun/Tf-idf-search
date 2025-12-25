# TF-IDF Search Engine (From Scratch)

A simple retrieval-based search system implemented from scratch using Python.
This project builds the core ideas behind classical information retrieval
without using libraries like `sklearn`.

## What this project does

- Builds a vocabulary (Bag of Words)
- Computes:
  - Term Frequency (TF)
  - Document Frequency (DF)
  - Inverse Document Frequency (IDF)
  - TF-IDF vectors
- Compares documents using **cosine similarity**
- Given a query, retrieves the most similar document

## What this project does NOT do

- No spell correction
- No semantic understanding
- No embeddings
- No text generation
- No learning or training

This is a **pure retrieval model**, not a chatbot or LLM.

## Why this project exists

This project was built to understand how:
- TF-IDF actually works internally
- cosine similarity compares vectors geometrically
- common words are down-weighted automatically
- out-of-vocabulary words fail cleanly

Instead of calling a prebuilt library, everything is implemented step by step
for learning purposes.

## Example behavior

- Queries containing common words (like `friend`) are weighted less
- Rare words influence similarity more
- Misspelled or unseen words result in zero contribution
- Similarity is based on vector direction, not length

## Files

- Jupyter notebook contains:
  - Vectorization logic
  - TF, IDF, TF-IDF computation
  - Cosine similarity
  - Simple search demo

## Limitations

- Vocabulary is fixed
- No typo handling
- No synonym handling
- Performance is not optimized for large datasets




