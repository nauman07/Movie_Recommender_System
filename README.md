# 🎬 Movie Recommender System

A **content-based movie recommendation system** built with Python that suggests similar movies based on features like genre, cast, keywords, and overview — powered by NLP and cosine similarity.

---

## 📖 About

This project implements a content-based filtering approach to recommend movies. Given a movie title, the system analyzes its attributes, compares them with other movies using cosine similarity, and returns the top similar movies. A Streamlit web app provides an interactive interface.

---

## 📂 Repository Structure

```
Movie_Recommender_System/
├── app.py                          # Streamlit web application
├── notebook86c26b4f17.ipynb        # Data processing and model building notebook
└── README.md
```

---

## ✨ Features

- Content-based filtering using movie metadata
- NLP pipeline: feature extraction, stemming, and vectorization
- Cosine similarity for finding related movies
- Interactive Streamlit web interface
- Works with the TMDB movies dataset

---

## 🔧 How It Works

1. **Feature Extraction** — Extracts useful columns (genres, cast, crew, keywords, overview)
2. **Data Preprocessing** — Cleans and reformats the data
3. **Stemming** — Reduces words to their base form for consistency
4. **Whitespace Removal** — Merges multi-word items as single tokens (e.g., "Sam Raimi" → "SamRaimi")
5. **Vectorization** — Converts text features into numerical vectors
6. **Cosine Similarity** — Measures similarity between movie vectors
7. **Recommendations** — Returns top N most similar movies

---

## 📦 Dataset

The project uses the **TMDB 5000 Movie Dataset** from Kaggle.

🔗 [Download Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

---

## 🛠️ Tech Stack

| Library | Purpose |
|--------|---------|
| `Pandas` | Data manipulation |
| `NumPy` | Numerical operations |
| `NLTK` | Stemming and NLP |
| `Scikit-learn` | CountVectorizer and Cosine Similarity |
| `Pickle` | Saving the trained model |
| `Streamlit` | Web application interface |
| `ast` | Parsing stringified lists |

---

## 🚀 Getting Started

### Install Dependencies

```bash
pip install pandas numpy nltk scikit-learn streamlit
```

### Build the Model

Open and run the Jupyter notebook to generate the model and similarity matrix:

```bash
jupyter notebook notebook86c26b4f17.ipynb
```

### Run the Web App

```bash
streamlit run app.py
```

Open your browser at `http://localhost:8501` and start getting recommendations!

---

## 📸 Demo

1. Select or type a movie title
2. Click "Recommend"
3. Get 5 similar movies with posters

---

## 📊 Metric Used

**Cosine Similarity** — Measures the angle between two feature vectors, giving a score between 0 and 1 (1 = identical, 0 = completely different).

---

## 🤝 Contributing

Pull requests are welcome. For major changes, open an issue first.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
