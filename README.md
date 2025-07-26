# 🎮 Movie Recommendation System

This is a content-based movie recommendation system built using Python and Streamlit. It suggests similar movies based on metadata and displays their posters using the TMDB API.

---

## 📆 Dataset Used

This project is based on the TMDB 5000 Movie Dataset:

* `tmdb_5000_movies.csv`
* `tmdb_5000_credits.csv`

These files contain details about movies, cast, crew, genres, and more.

---

## ⚙️ How It Works

1. The two datasets are merged using the movie title.
2. Metadata like **cast**, **crew**, **genres**, **keywords**, and **overview** are extracted.
3. A new column `tags` is created combining all the important text features.
4. Text vectorization is done using `CountVectorizer`.
5. Cosine similarity is calculated between all movies.
6. The results are saved as:

   * `movie_dict.pkl`: DataFrame of movies
   * `similarity.pkl`: Similarity matrix (Not on GitHub due to size)

---

## 🚀 How to Run the App

### 🧱 Step 1: Install dependencies

```bash
pip install -r requirements.txt
```

### ▶️ Step 2: Run the Streamlit app

```bash
streamlit run app.py
```

---

## 📅 Download similarity.pkl

Due to GitHub's 100MB file limit, the `similarity.pkl` file is hosted externally.

👉 [Click here to download similarity.pkl](https://drive.google.com/uc?id=1K1qB1QUZk44IzOxPTek5UC5ejqqp4Bx-&export=download)

After downloading, place the file in the **same folder** where `app.py` is located.

---

## 🖼️ API Used

* **TMDB API** is used to fetch movie posters dynamically

---

## 🧐 Tech Stack

* Python
* Pandas
* Scikit-learn
* Streamlit
* TMDB API
* Numpy

---

## ✍️ Author

**Himanshu**
📧 [himanshu@example.com](mailto:himanshu@example.com)
📁 GitHub: [himanshu12004](https://github.com/himanshu12004)

---

## ✅ Project Status

This project is fully functional and tested. You can improve it by:

* Adding user ratings
* Collaborative filtering
* Deploying on Streamlit Cloud
