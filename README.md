# 🏏 Sentiment Analysis of Cricket Commentary

Analyses the emotional tone of ball-by-ball **IPL 2018** commentary using transformer models (**RoBERTa** and **BERT**).

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Transformers](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![NLTK](https://img.shields.io/badge/NLTK-154F5B?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

## 📌 Overview

Commentary captures the drama of a match: boundaries, wickets, close finishes. This project scores each commentary line as **negative, neutral or positive** to see how sentiment moves through a game.

## 📂 Repository structure

```
Sentiment_Analysis_Cricket_Commentary/
├── IPL2018 - Commentary Data (2).csv  # ball-by-ball commentary dataset
├── Roberta.ipynb                      # RoBERTa sentiment scoring
└── sentiment_bert.ipynb               # BERT-based sentiment analysis
```

## 🧠 Approach

- **Data:** ~14,000 commentary rows with over, short_text and long_text columns
- **Model:** cardiffnlp/twitter-roberta-base-sentiment from Hugging Face, used for inference
- **Output:** softmax probabilities for negative, neutral and positive sentiment per line
- Text tokenised with NLTK and the model's own tokenizer

## ▶️ Run it

1. Open Roberta.ipynb in [Google Colab](https://colab.research.google.com/).
2. Upload the CSV to Google Drive and update the file path.
3. Run all cells; model weights download automatically from Hugging Face.

Requirements: transformers, torch, nltk, pandas, numpy, scipy, seaborn, tqdm.

## 🔭 Next steps

- Aggregate sentiment per over, innings and team
- Plot sentiment timelines against match events (wickets, sixes)
- Compare RoBERTa and BERT results side by side

## 👤 Author

**Siva Pasupuleti** · [GitHub](https://github.com/siva-0104)
