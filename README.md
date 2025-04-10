# Telugu-Wiki-Corpus-From-Raw-Text-to-Linguistic-Insight
# 🇮🇳 Telugu Wikipedia NLP Toolkit

This project is a **computational tribute to the Telugu language**, focusing on Natural Language Processing (NLP) techniques applied to raw data collected from **Telugu Wikipedia**. From data collection to morphological analysis, this pipeline demonstrates the power of combining linguistic insights with computational tools.

---

## 📌 Project Objectives

- To build a structured corpus from Telugu Wikipedia
- To clean and preprocess Telugu text
- To perform sentence-level and word-level statistical analysis
- To implement unigram and bigram models
- To design a basic morphological analyzer for Telugu
- To curate and apply a stop word removal module

---

## 📁 Directory Structure


---

## 🔍 Processing Pipeline

### 🧾 Step 1: Data Download
Used `wget` to recursively download Telugu Wikipedia articles, excluding non-text media.

### 🧼 Step 2: HTML to Text Conversion
Parsed HTML to extract meaningful article content from `<div class="mw-parser-output">`.

### 🗃️ Step 3: Merging and Cleaning
Merged individual `.txt` files into a single corpus. Cleaned the text for analysis.

### ✂️ Step 4: Sentence Segmentation
Each line in `sentence_corpus.txt` contains a single sentence from the corpus.

### 📊 Step 5: Sentence Statistics
For each sentence, computed:
- Sentence ID
- Word count
- Average words per sentence
- Total character count

### ❌ Step 6: Punctuation Removal
Removed all punctuation except sentence termination markers like `.`, `?`, and `!`.

### 📈 Step 7: N-Gram Analysis
Generated:
- Word unigrams and bigrams
- Frequency counts
- Visualizations using matplotlib

### 🧠 Step 8: Morphological Analysis
Implemented using:
- **N-gram modeling (unigram, bigram, trigram)**
- **Maximum Likelihood Estimation (MLE)**
- **Backoff Smoothing**

Used to identify morphemes and affixes in Telugu words.

### 🛑 Step 9: Stop Word Removal
Generated stop word list using:
- Words appearing in >5% of sentences
- NLTK Telugu stopwords (if available)
- Manually curated functional words

Filtered out stop words from each sentence for better downstream NLP performance.

---

## 📊 Outputs

- **Corpus Statistics**: Word and character distributions
- **N-gram Frequency Files**: Stored in `.txt` format
- **Cleaned & Processed Corpora**: Useful for training Telugu NLP models
- **Stop Word-Free Corpus**: Ideal for tasks like summarization and classification

---

## 💻 Tech Stack

- Python 3
- NLTK
- Regular Expressions (`re`)
- `collections.Counter`
- `matplotlib` (for plotting)
- Shell Scripting (`wget`, `cat`)
- Jupyter Notebooks

---

## 🪔 Dedication

This work is dedicated to **Telugu**, one of India’s most elegant and ancient languages. Through computational tools, we aim to preserve, promote, and unlock its digital potential for research, education, and innovation in language technology.

---

## 📎 License

This project is open-source under the [MIT License](LICENSE).

---

## 🤝 Contributions

Feel free to open issues, suggest improvements, or contribute new modules related to:
- Named Entity Recognition
- Part-of-Speech Tagging
- Telugu WordNet Integration
- Deep Learning Models for Telugu





