
# Final Project MDTT — Topic Modelling Comparison (LDA vs LSA)

This project compares two topic modeling techniques: **Latent Dirichlet Allocation (LDA)** and **Latent Semantic Analysis (LSA)** using real customer reviews from **Hotel Bumi Surabaya** (scraped from Google Maps).

---

## 📁 Repository Structure

```
├── final project mdtt data/
│   ├── review_hotel_bumi.csv           # Raw scraped reviews
│   ├── data_clean.csv                  # Cleaned + normalized text
│   ├── best_topic_modelling.csv        # Final result with topic labels
│   └── lda_visualisasi_hotel_bumi.html # PyLDAvis interactive visualization
│
├── kata-baku/
│   ├── katabaku_updated.xlsx           # Normalization dictionary
│   └── stopwords_ind.xlsx              # Extended stopwords list
│
├── Final Project MDTT (LDA LSA).ipynb  # Main analysis notebook
└── README.md                           # Project documentation
```

---

## 🎯 Objectives

- Clean and normalize Bahasa Indonesia review text  
- Compare **LDA** (with `gensim`) and **LSA** (with `TruncatedSVD`)  
- Find optimal number of topics using **Coherence Score**  
- Label topics based on top keywords  
- Visualize results using:
  - 📊 `pyLDAvis` for LDA
  - 🔍 `t-SNE` plots for document distribution
  - ☁️ Word Clouds & Word Link Graphs (Bigram-based)

---

## 🔑 Final Topic Labels (4 Topics)

1. **Fasilitas Umum dan Kenyamanan Area Publik**  
2. **Kebersihan dan Kualitas Sarana Prasarana**  
3. **Kualitas Pelayanan dan Suasana Hotel**  
4. **Pengalaman Kuliner dan Keunikan Menu Lokal**

Topic selection is based on coherence optimization, keyword co-occurrence, and visual interpretability.

---

## 📦 Output Files

| File Path                                      | Description                         |
|-----------------------------------------------|-------------------------------------|
| `best_topic_modelling.csv`                    | Final dataset with topic labels     |
| `lda_visualisasi_hotel_bumi.html`             | Interactive LDA topic explorer      |
| `data_clean.csv`                              | Cleaned and stemmed review text     |

---

## 📚 Libraries Used

- `pandas`, `nltk`, `Sastrawi`, `re`, `emoji`
- `gensim`, `scikit-learn`, `pyLDAvis`, `matplotlib`, `seaborn`
- `wordcloud`, `networkx`, `TSNE`, `collections.Counter`

---

## ▶️ How to Run

1. Open the notebook:

```bash
Final Project MDTT (LDA LSA).ipynb
```

2. Run cells step-by-step:
   - Preprocessing
   - Topic Modeling (LDA & LSA)
   - Coherence Evaluation
   - WordCloud & Word Link Visualizations
   - t-SNE Clustering & Interpretation

---
