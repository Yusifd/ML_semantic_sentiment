# ML_semantic_sentiment
# 📊 Sentiment Analysis on Azerbaijani Sentences

In this project, I experimented with **multilingual sentiment analysis** using two different transformer-based models:

- 🟢 **BERT-base multilingual uncased sentiment** (`nlptown/bert-base-multilingual-uncased-sentiment`)
- 🔵 **XLM-Roberta-base sentiment** (`cardiffnlp/twitter-xlm-roberta-base-sentiment`)

---

## ⚔️ Model Comparison

To evaluate performance, I tested both models on **100 Azerbaijani sentences** across five sentiment categories:
- Çox mənfi (Very Negative)
- Mənfi (Negative)
- Neytral (Neutral)
- Müsbət (Positive)
- Çox müsbət (Very Positive)

### ✅ Results:
- **XLM-Roberta** achieved **accuracy between 79% – 91%**  
- **BERT-base multilingual** achieved **accuracy between 51% – 78%**

👉 This shows that **XLM-Roberta** is more robust and reliable for Azerbaijani text sentiment classification compared to the multilingual BERT baseline.

---

## 🔥 Key Highlights
- Built embeddings with `sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2` for semantic similarity search.
- Generated **heatmaps** with `seaborn` to visualize sentiment probabilities across sentences.
- Grouped predictions into **negative, neutral, positive** categories for easier interpretation.
- Compared **fine-grained sentiment labels** (1★ to 5★) vs. **3-class sentiment labels** (Negative, Neutral, Positive).

---

## 📊 Model Performance Comparison

| Model | Accuracy Range | Strengths | Weaknesses |
|-------|----------------|-----------|------------|
| 🔵 **XLM-Roberta-base sentiment** | **79% – 91%** | Handles Azerbaijani text very well, robust across categories, consistent predictions | Slightly heavier model, requires more resources |
| 🟢 **BERT-base multilingual uncased sentiment** | **51% – 78%** | Lightweight, faster inference, decent for general multilingual tasks | Struggles with nuanced Azerbaijani expressions, less accurate and less consistent |

---

### 📝 Key Takeaway
- **XLM-Roberta** clearly outperforms **BERT-base multilingual** for **Azerbaijani sentiment analysis**.  
- If accuracy is the priority → go with **XLM-Roberta**.  
- If speed and lightweight inference matter more → **BERT-base multilingual** can still be used, but expect weaker results.

---


## 🚀 Conclusion
- **XLM-Roberta** is the better choice for **Azerbaijani sentiment analysis**, offering higher accuracy and more consistent predictions.  
- **BERT-base multilingual** works but struggles with nuanced Azerbaijani expressions.  
- Future work: fine-tuning XLM-Roberta on a larger Azerbaijani dataset for even better performance.

---

✨ With this comparison, I demonstrated how **model choice** significantly impacts performance in multilingual NLP tasks.  
