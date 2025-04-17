# Telugu Word Sense Disambiguation (WSD)

### 🧠 Building a Polysemy Dataset & Evaluating NLP Models  
**Author:** Syam Immanuel Paul Bondada  
**MSc Big Data Science, Queen Mary University of London**  
**Supervisor:** Dr. Haim Dubossarsky

---

## 📘 Overview

This project addresses **Word Sense Disambiguation (WSD)** in **Telugu**, a linguistically rich but under-resourced Dravidian language. The core contribution is the creation of a novel, manually validated **polysemy dataset** and an in-depth evaluation of **contextual NLP models** on their ability to resolve ambiguous meanings of Telugu words.

The goal is to bridge the NLP resource gap by improving semantic understanding in low-resource languages.

---

## 📊 Dataset Summary

- **Language**: Telugu  
- **Words**: 50 polysemous words  
- **Senses**: ~102 unique senses  
- **Sentences**: 4,581 total sentences  
- **Annotation**: Expert manual validation  
- **Sampling**: Smart centroid-based clustering of contextual embeddings  
- **Use Case**: WSD, multilingual NLP, transfer learning

---

## 🧪 Models Evaluated

| Model                            | Accuracy | F1 Score |
|----------------------------------|----------|----------|
| `l3cube-pune/telugu-bert`        | 90%      | 89%      |
| `google/muril-base-cased`       | 91%      | 91%      |
| `pierluigic/xl-lexeme`           | 77%      | 76%      |
| Others (e.g., mt5, distilBERT)  | < 70%    | < 70%    |

> Telugu-BERT and MURIL showed the highest effectiveness in context-aware disambiguation.

---

## 🛠️ Methods Used

- **Data Collection**: AI4Bharat IndicNLP, Telugu Wikipedia, Blogspot, WordNet
- **Annotation**: Manual + linguist review
- **Dimensionality Reduction**: UMAP, PCA
- **Clustering**: K-Means (preferred), Agglomerative
- **Embeddings**: BERT, MURIL
- **Evaluation**: Accuracy, F1 score, 2D scatter plots

---

## 📌 Key Findings

- **Language-specific models** outperform multilingual ones in polysemy handling.
- **Telugu BERT** excels at separating subtle contextual meanings.
- A combination of **manual review** and **contextual clustering** yields a reliable dataset.
- **Transfer learning limitations** are evident with general-purpose models.

---

## 🚀 Future Work

- Expand dataset to more polysemous words and varied sentence structures.
- Explore **cross-lingual transfer** with other Dravidian languages.
- Integrate **active learning** to improve annotation scalability.
- Apply models in downstream NLP tasks like **machine translation** or **chatbots**.

---

## 📚 Citation

If using this work or dataset, please cite the dissertation:

**Syam Immanuel Paul Bondada** (2024). *Telugu Word Sense Disambiguation: Building a Polysemy Dataset and Evaluating NLP Models*. Queen Mary University of London.

---

## 🧾 Acknowledgements

Special thanks to **Dr. Haim Dubossarsky** for invaluable supervision and guidance throughout this research.

---

## 🔗 Links

- [HuggingFace Telugu-BERT](https://huggingface.co/l3cube-pune/telugu-bert)
- [AI4Bharat IndicNLP](https://github.com/AI4Bharat/indicnlp_corpus)
- [Telugu Dictionary](https://www.telugudictionary.org/)

