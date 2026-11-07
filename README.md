# 🌍 Detecting Stance in Media on Global Warming for Indic Languages

**An NLP-based system for identifying public opinions on climate change and global warming in Hindi and Bengali social media comments.**

## 📌 Overview

Climate change and global warming have become important topics of public discussion across social media platforms. Understanding public opinion in regional languages is challenging because of informal expressions, spelling variations, code-mixing, and language-specific linguistic patterns.

This project aims to develop a Natural Language Processing (NLP) based **Stance Detection System** that analyses Hindi and Bengali social media comments and identifies the author's position towards the claim:

> "Climate change and global warming is a serious concern."

Unlike traditional sentiment analysis, which identifies positive, negative, or neutral emotions, stance detection determines whether a person supports, opposes, or expresses no clear position towards a specific claim.

## 🎯 Objectives

- Develop a three-class stance detection system for Hindi and Bengali.
- Analyse social media comments using NLP techniques.
- Establish a baseline using TF-IDF and traditional machine learning classifiers.
- Fine-tune multilingual and Indic-language transformer models.
- Compare different models using consistent evaluation metrics.
- Analyse classification errors across languages and stance categories.
- Identify public opinion trends regarding climate change and global warming.

## 🏷️ Stance Categories

The system will classify each comment into one of three categories:

| Label | Description |
|---|---|
| **Favour** | The comment supports the claim that climate change and global warming are serious concerns. |
| **Against** | The comment opposes or rejects the claim. |
| **None** | The comment does not express a clear stance towards the claim. |

**Note:** This is a comment-level stance classification task, not a fact-checking system or a measure of scientific truth.

## ⚙️ Proposed Methodology

The project will follow a structured NLP development pipeline.

1. **Data Collection and Exploration**
   - Load the provided Hindi and Bengali datasets.
   - Inspect class distribution and missing values.
   - Analyse duplicates, language patterns, and text characteristics.

2. **Text Preprocessing**
   - Clean noisy text and unnecessary characters.
   - Handle spelling variations and informal expressions.
   - Analyse Hindi and Bengali text separately.
   - Examine code-mixed comments.

3. **Baseline Model Development**
   - Apply TF-IDF vectorization.
   - Train traditional machine learning classifiers.
   - Establish baseline performance.

4. **Transformer Model Development**
   - Experiment with pretrained multilingual and Indic-language models.
   - Fine-tune selected transformer architectures.
   - Compare their performance with traditional ML approaches.

5. **Evaluation and Analysis**
   - Evaluate models using Macro F1-score, Accuracy, Precision, and Recall.
   - Generate confusion matrices.
   - Analyse incorrect predictions across languages and classes.

6. **Final Model Comparison**
   - Compare all implemented approaches.
   - Identify the most suitable model.
   - Document limitations and future improvements.

## 🧠 Proposed Models

The following models are planned for experimentation:

| Approach | Proposed Models |
|---|---|
| Traditional ML | Logistic Regression, Linear SVM |
| Multilingual Transformers | mBERT, XLM-RoBERTa |
| Indic Language Models | IndicBERT |

*The final selection will depend on dataset characteristics, computational resources, and experimental results.*

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| NLP | NLTK, Scikit-learn |
| Deep Learning | PyTorch |
| Transformers | Hugging Face Transformers |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Development Environment | Google Colab, VS Code |
| Version Control | Git and GitHub |

## 📊 Evaluation Metrics

The models will be evaluated using:

- Accuracy
- Precision
- Recall
- Macro F1-score
- Confusion Matrix

**Primary Evaluation Metric: Macro F1-score**

Macro F1-score will be prioritised because it gives equal importance to all three stance categories, including potentially underrepresented classes.

## 📁 Planned Project Structure

```text
Indic-Climate-Stance-Detection/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_baseline_models.ipynb
│   └── 04_transformer_models.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── feature_extraction.py
│   ├── train.py
│   ├── evaluate.py
│   └── predict.py
│
├── results/
│   ├── metrics/
│   └── visualizations/
│
├── models/
│
├── requirements.txt
├── README.md
└── .gitignore
```

*The directory structure is planned and will evolve during development.*

## 👥 Team CODE MINIONS

| Team Member |
| Rupanshi | [@Rupanshi-git](https://github.com/Rupanshi-git) |
| Molly Agarwal | [@MollyAgarwal7](https://github.com/MollyAgarwal7) |
| Shagun | [@shagunlakhlan](https://github.com/shagunlakhlan) |
| Aditya Utkarsh | [@adityautkarsh52-art](https://github.com/adityautkarsh52-art) |
| Moksh Varshney | [@MokshFF](https://github.com/MokshFF) |

**Project Mentor:** Dr. Supriya Chanda

## 📈 Current Development Status

<code>Project Status: Initial Development</code>

- [ ] Dataset collection and inspection
- [ ] Exploratory Data Analysis
- [ ] Text preprocessing
- [ ] TF-IDF baseline implementation
- [ ] Traditional ML model training
- [ ] Transformer model fine-tuning
- [ ] Model evaluation and comparison
- [ ] Error analysis
- [ ] Final documentation

We are beginning development and will update this repository as different stages of the project are completed.

## 🚀 Future Scope

- Extend stance detection to additional Indic languages.
- Improve handling of code-mixed and informal social media text.
- Explore multilingual and cross-lingual transfer learning.
- Develop an interactive interface for analysing stance predictions.
- Generate language-wise and category-wise public opinion summaries.

## 📚 Research References

The project is informed by research in climate change discourse analysis, multilingual NLP, and stance detection, including:

1. Dhoroni: Exploring Bengali Climate Change and Environmental Views with a Multi-Perspective News Dataset and Natural Language Processing.
2. A Survey of NLP Approaches for Climate Change Sentiment Analysis in Global and Indian Contexts.
3. Analyzing the Dynamics of Climate Change Discourse on Twitter: A New Annotated Corpus and Multi-Aspect Classification.
4. A Multi-Task Model for Sentiment Aided Stance Detection of Climate Change Tweets.
5. Towards Fine-grained Classification of Climate Change related Social Media Text.

---

**Developed by Team CODE MINIONS** ❤️

*Building NLP solutions for understanding climate discourse in Indic languages.*
