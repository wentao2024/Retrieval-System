# BM25-Enhanced Language Model for Wikipedia Question Answering

## Overview
This project implements a retrieval-augmented generation (RAG) system for open-domain question answering using Wikipedia data. It combines BM25 retrieval with a large language model to generate accurate answers to natural language questions.

## Key Features
- BM25 retrieval model implementation using Pyserini
- Integration with GPT-2 language model for answer generation
- Corpus of 35+ million indexed Wikipedia passages
- Performance evaluation using Exact Match (EM) and F1 scores
- Analysis of various factors affecting model performance

## Setup
1. Install required libraries:
   ```
   pip install pyserini transformers datasets faiss-cpu pytrec_eval bitsandbytes
   ```
2. Download and preprocess the Wikipedia dataset
3. Index the corpus using Pyserini
4. Set up Hugging Face access token for model downloads

## Usage
1. Run BM25 retrieval on the Natural Questions dataset
2. Generate answers using the language model
3. Evaluate performance and analyze results

## File Descriptions
- `index_corpus.py`: Script for indexing Wikipedia passages
- `bm25_retrieval.py`: Implements BM25 retrieval
- `llm_answer_generation.py`: Generates answers using the language model
- `evaluation.py`: Calculates performance metrics
- `analysis.py`: Analyzes impact of various factors on performance

## Results
The project includes visualizations and analysis of:
- Impact of number of retrieved documents
- Effect of including BM25 scores in prompts
- Influence of document rank and diversity
- Performance with varying levels of noise documents

## Future Work
- Experiment with different language models
- Implement more advanced retrieval techniques
- Explore domain-specific fine-tuning

## Contributors
[Your Name]

## License
[Specify your license here]

This README provides a concise overview of your project, its key features, setup instructions, and main components, making it easy for others to understand and potentially contribute to your work.
