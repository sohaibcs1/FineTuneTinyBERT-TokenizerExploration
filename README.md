
# 📝 The Impact of Tokenization on TinyBERT Performance Across Text Classification Tasks

This repository demonstrates the use of text classification techniques by using three popular tokenization methods: **BPE (Byte Pair Encoding)**, **WordPiece**, and **SentencePiece**. In addition to tokenization, the project includes fine-tuning of a lightweight BERT model, Tiny BERT, to achieve efficient and accurate classification on datasets like IMDb, AG News, and Yelp. This combination of tokenization strategies and model fine-tuning showcases the impact of preprocessing and optimization on NLP tasks.

---

## 📖 Table of Contents

1. [🎯 Introduction](#🎯-introduction)
2. [✨ Features](#✨-features)
3. [⚙️ Installation](#⚙️-installation)
4. [🚀 Usage](#🚀-usage)
5. [🔧 Tokenizer Techniques](#🔧-tokenizer-techniques)
6. [🧠 Models and Parameters](#🧠-models-and-parameters)
7. [📊 Datasets](#📊-datasets)
8. [📂 Folder Structure](#📂-folder-structure)
9. [🤝 Contributing](#🤝-contributing)
10. [📜 License](#📜-license)
11. [👏 Acknowledgments](#👏-acknowledgments)

---

## 🎯 Introduction

Tokenization is a crucial step in **Natural Language Processing (NLP)**. This repository explores three popular tokenization techniques:

- **BPE Tokenizer**: Splits text into subwords using frequency-based merges.
- **WordPiece Tokenizer**: A subword tokenization technique used in models like BERT.
- **SentencePiece Tokenizer**: Implements subword tokenization with language model independence.

Each tokenizer is evaluated on text classification tasks using datasets such as **IMDb**, **AG News**, and **Yelp**.

---

## ✨ Features

- 🛠️ Implementation of **BPE**, **WordPiece**, and **SentencePiece** tokenizers.
- 📚 Support for multiple datasets (**IMDb**, **AG News**, and **Yelp**).
- 📊 Interactive demonstrations using **Jupyter Notebooks**.
- 🔍 Visualizations to understand tokenization results.

---

## ⚙️ Installation

### Prerequisites

- 🐍 Python 3.8+
- 📒 Jupyter Notebook or Jupyter Lab
- 📦 Required libraries listed in `requirements.txt`

### Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/tokenizer-techniques.git
   cd tokenizer-techniques
   ```
---

## 🚀 Usage

### Step 1: Open the Jupyter Notebook

```bash
jupyter notebook
```

### Step 2: Choose a Dataset and Tokenizer Notebook

Navigate to the appropriate dataset folder (`imdb`, `ag_news`, `yelp`) and select a notebook for a specific tokenizer (e.g., `BPE_Tokenizer.ipynb`).

### Step 3: Run the Notebook

Follow the step-by-step execution in the notebook to preprocess text, apply tokenization, and visualize results.

---

## 🔧 Tokenizer Techniques

### **1. Byte Pair Encoding (BPE) Tokenizer** 🧩

- **Description**: Splits text into smaller subwords based on frequent pairings of characters or subwords.
- **Parameters**: 
  - Vocabulary size: `30,000`
  - Minimum frequency: `2`
  - Special tokens: `<pad>`, `<cls>`, `<sep>`

### **2. WordPiece Tokenizer** 🧩

- **Description**: Used in models like BERT, WordPiece learns a compact vocabulary and creates tokens based on frequency thresholds.

### **3. SentencePiece Tokenizer** 🧩

- **Description**: A language-independent tokenizer that converts text into sequences of subwords.

---

## 🧠 Models and Parameters

### **BERT-Tiny Model** 🧠
- **Architecture**: A lightweight version of BERT (`prajjwal1/bert-tiny`).
- **Sequence Classification**: Supports binary classification tasks.
- **Hyperparameters**:
  - Learning rate: `2e-6`
  - Weight decay: `2e-4`
  - Epochs: `5`
  - Batch size: `2`
  - Optimizer: AdamW

---

## 📊 Datasets

### **1. IMDb** 🎥
- **Type**: Sentiment Analysis
- **Description**: A dataset of movie reviews with binary sentiment labels (positive/negative).

### **2. AG News** 📰
- **Type**: Topic Classification
- **Description**: Contains news articles categorized into four classes: **World**, **Sports**, **Business**, and **Science/Technology**.

### **3. Yelp** 🍴
- **Type**: Sentiment Analysis
- **Description**: Yelp reviews labeled for positive and negative sentiments.

Preprocessed datasets and tokenizer artifacts (e.g., `vocab.json`, `merges.txt`) are included in their respective folders.

---

## 📂 Folder Structure

```
Notebooks_extracted/
├── imdb/
│   ├── BPE_Tokenizer.ipynb
│   ├── WordPiece_Tokenizer.ipynb
│   ├── SentencePiece_Tokenizer.ipynb
├── ag_news/
│   ├── BPE_Tokenizer.ipynb
│   ├── WordPiece_Tokenizer.ipynb
│   ├── SentencePiece_Tokenizer.ipynb
│   └── bpe_tokenizer/
│       ├── vocab.json
│       ├── merges.txt
├── yelp/
│   ├── BPE_Tokenizer.ipynb
│   ├── WordPiece_Tokenizer.ipynb
│   ├── SentencePiece_Tokenizer.ipynb
```

---

## 🤝 Contributing

We welcome contributions! To contribute:

1. Fork the repository.
2. Create a feature branch.
3. Submit a pull request with your changes.

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 👏 Acknowledgments

Special thanks to:

- The creators of the **IMDb**, **AG News**, and **Yelp** datasets.

