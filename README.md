# 🎬 Movie Recommendation System

A Python-based Movie Recommendation System that recommends similar movies using movie metadata and TF-IDF text vectorization. The project includes a Jupyter Notebook for data exploration, saved preprocessing artifacts, and application entry points.

## ✨ Features

- Content-based movie recommendations.
- TF-IDF vectorization for processing movie text metadata.
- Saved movie data and model artifacts for reuse.
- Movie metadata stored in a CSV dataset.
- Optional integration with the TMDB API for movie details and posters.
- Jupyter Notebook for data exploration and model development.

## 🛠️ Tech Stack

- **Language:** Python
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn, TF-IDF
- **Development:** Jupyter Notebook, VS Code
- **Movie Data API:** The Movie Database (TMDB), if configured

## 📁 Project Structure

```text
Movie-Recommendation-System/
├── .gitattributes
├── .gitignore
├── app.py
├── df.pkl
├── indices.pkl
├── main.py
├── movies_metadata.csv
├── movies.ipynb
├── README.md
├── requirements.txt
├── runtime.txt
├── tfidf_matrix.pkl
└── tfidf.pkl
```

## 📄 File Description

| File | Description |
|---|---|
| `app.py` | Application entry point or user interface |
| `main.py` | Main application or recommendation logic |
| `movies.ipynb` | Notebook for data exploration and development |
| `movies_metadata.csv` | Movie metadata dataset |
| `df.pkl` | Serialized DataFrame or processed movie data |
| `indices.pkl` | Saved movie-to-index mapping |
| `tfidf.pkl` | Saved TF-IDF vectorizer |
| `tfidf_matrix.pkl` | Saved TF-IDF feature matrix |
| `requirements.txt` | Required Python packages |
| `runtime.txt` | Runtime configuration |
| `.gitignore` | Files excluded from Git tracking |
| `.gitattributes` | Git file-handling configuration |

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

### 2. Create a virtual environment

On Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Run the application

If `app.py` is a standard Python script:

```bash
python app.py
```

If it uses Streamlit:

```bash
python -m streamlit run app.py
```

Alternatively, if `main.py` is the intended entry point:

```bash
python main.py
```

Use the command appropriate to the framework and implementation in your source files.

## 🧠 How It Works

The typical content-based recommendation workflow is:

1. Load movie metadata from the CSV dataset.
2. Clean and preprocess relevant movie information.
3. Convert textual features into numerical vectors using TF-IDF.
4. Compare movie representations using a similarity measure, such as cosine similarity.
5. Identify movies similar to the selected movie.
6. Reuse saved preprocessing objects and feature matrices when appropriate.
7. Optionally retrieve movie posters and additional details through TMDB.

The exact features and recommendation logic depend on the implementation in `movies.ipynb`, `app.py`, and `main.py`.

## 🎞️ TMDB API Integration

TMDB can provide movie information and poster images for the application.

Useful resources:

- [TMDB Developer Documentation](https://developer.themoviedb.org/docs)
- [TMDB API Reference](https://developer.themoviedb.org/reference/intro/getting-started)
- [TMDB Website](https://www.themoviedb.org/)

If you use a TMDB API key, keep it private and store it in an environment variable or an untracked `.env` file. Follow TMDB's current API terms and attribution requirements.

## 🚀 Future Improvements

- Add movie search and genre-based filtering.
- Display movie posters, ratings, and release dates.
- Improve recommendation quality through metadata and similarity tuning.
- Build a responsive interface.
- Deploy the application online.
- Add user ratings and personalized recommendations.

## ⚠️ Important Notes

- Keep the saved `.pkl` artifacts consistent with the dataset and preprocessing code.
- Regenerate the artifacts when relevant preprocessing or model settings change.
- Only load pickle files from trusted sources.
- Check dataset size and repository hosting limits before committing large files.

## 📚 Acknowledgements

- [The Movie Database (TMDB)](https://www.themoviedb.org/), if used by the application.
- The Python and open-source machine learning ecosystem.

---

**Built as a learning project to explore Python, text vectorization, and movie recommendation systems.**
