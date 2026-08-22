# LLM Text Generation & NLP Practice

This repository contains a small collection of notebook-based experiments for natural language processing, sentiment analysis, and word embeddings.

## Project contents

### 1. Movie sentiment analysis
File: `movie-sentimental-analysis.ipynb`

This notebook explores sentiment classification on Amazon movie reviews using:
- NLTK tokenization and basic text processing
- VADER sentiment scoring
- Hugging Face RoBERTa sentiment model
- Visualization and comparison of model outputs

The dataset used is the Amazon review dataset. Because the raw CSV is too large for GitHub, it must be downloaded from Kaggle and placed in the project folder as `Reviews.csv` before running the notebook.

### 2. Word2Vec practice
File: `word2vec-practice.ipynb`

This notebook demonstrates a basic Word2Vec workflow using `gensim`, including:
- Text preprocessing
- Building a vocabulary
- Training word embeddings
- Similarity and analogy-style checks
- Dimensionality reduction and visualization

This notebook expects a corpus under a `data/` directory containing text files to train on.

## Environment setup

Recommended Python version: 3.10+

Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn nltk gensim scikit-learn plotly transformers torch tqdm
```

If you use Jupyter notebooks, also install:

```bash
pip install jupyter
```

## Data setup

### Movie sentiment notebook
1. Download the Amazon reviews dataset from Kaggle.
2. Save the file as `Reviews.csv` in the repository root.
3. Run the notebook cells in order.

### Word2Vec notebook
1. Create a `data/` folder in the project root.
2. Add text corpus files (for example `.txt` files) for training.
3. Run the notebook cells in order.

## Typical workflow

```bash
# optional: create and activate a virtual environment
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
# .venv\Scripts\activate    # Windows

pip install -r requirements.txt
```

If you do not have a `requirements.txt` file yet, install the packages listed above manually, then open the notebooks in Jupyter.

## Notes

- The notebooks are intended for learning and experimentation rather than production deployment.
- Some model downloads from Hugging Face may take time on first use.
- The exact output may vary depending on your dataset version and dependency versions.

## Repository structure

```text
llm-text-gen/
├── README.md
├── movie-sentimental-analysis.ipynb
├── word2vec-practice.ipynb
├── Reviews.csv      # downloaded for the sentiment notebook
├── data/            # text corpus for the Word2Vec notebook
└── .venv/           # optional local virtual environment
```

This project is meant to serve as a practical introduction to sentiment analysis techniques and vector-space language modeling with Python notebooks.
