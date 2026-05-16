# 🎬 Movie Recommendation System

A content-based movie recommendation system built using the IMDB dataset. Given a movie title, the system recommends similar movies based on their metadata using TF-IDF vectorization and cosine similarity.

---

## 📌 Features

- Recommends movies similar to a given title
- Uses content-based filtering (no user data required)
- Built on top of the IMDB movies metadata dataset
- Preprocessed and saved as pickle files for fast loading

---

## 🗂️ Dataset

- **Source:** IMDB Movies Metadata (`movies_metadata.csv`)
- Contains information such as title, genres, overview, cast, crew, and more

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core language |
| Pandas | Data manipulation |
| Scikit-learn | TF-IDF Vectorizer & Cosine Similarity |
| Pickle | Model serialization |
| Google Colab | Development environment |

---

## 🚀 How It Works

1. **Data Loading** — Load and clean the IMDB movies metadata CSV
2. **Feature Extraction** — Apply TF-IDF vectorization on movie descriptions/metadata
3. **Similarity Computation** — Compute cosine similarity between all movie vectors
4. **Recommendation** — Given a movie title, return the top N most similar movies

---

## 📁 Project Structure

```
Movie-recommendation-system/
│
├── movies_metadata.csv       # Raw IMDB dataset
├── tfidf_matrix.pkl          # Saved TF-IDF matrix
├── tfidf.pkl                 # Saved TF-IDF vectorizer
├── indices.pkl               # Movie title to index mapping
├── df.pkl                    # Processed dataframe
└── Movie_recommendation_system.ipynb  # Main notebook
```

---

## ▶️ How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload the `movies_metadata.csv` file
3. Run all cells in order
4. Call the recommendation function with any movie title:

```python
get_recommendations("The Dark Knight")
```

---

## 📊 Example Output

```
Recommendations for "The Dark Knight":
1. Batman Begins
2. The Dark Knight Rises
3. Batman
4. Superman
5. Iron Man
```

---

## 👩‍💻 Author

**Puzziii** — [GitHub Profile](https://github.com/Puzziii)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
