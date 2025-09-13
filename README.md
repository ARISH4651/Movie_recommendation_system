#  Movie Recommendation System  

## Project Overview  
This project implements a **Content-Based Movie Recommendation System** using the **TMDB dataset**.  
It recommends movies based on similarity in **genres, keywords, tagline, cast, and director** using **TF-IDF Vectorization** and **Cosine Similarity**.  

---

## 🛠Tech Stack  
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib, Difflib  
- **Algorithm:** Content-based filtering using TF-IDF & Cosine Similarity  
- **Tools:** Jupyter Notebook / Google Colab  

---

##  Dataset  
The dataset used is **movies.csv** (from [TMDB Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) or similar sources).  
It contains movie information such as:  
- Title  
- Genres  
- Keywords  
- Tagline  
- Cast  
- Director  

---

##  Workflow  

1. **Data Preprocessing**  
   - Handle missing values in selected features  
   - Select important textual features: *genres, keywords, tagline, cast, director*  

2. **Feature Engineering**  
   - Combine selected features into a single text string  

3. **Vectorization**  
   - Use **TF-IDF Vectorizer** to convert text data into numerical vectors  

4. **Similarity Calculation**  
   - Compute **Cosine Similarity** between movies  

5. **Recommendation Function**  
   - Input: User’s favorite movie  
   - Output: Top 10 most similar movies  

---

Sample Output

Input:

Enter your favorite movie: Avatar

Output:

Movies suggested for you:
1. Avatar
2. Guardians of the Galaxy
3. Thor
4. Star Trek
5. Avengers: Age of Ultron
...
 Results & Insights

Built a content-based recommender that suggests movies based on metadata similarity.

Achieved meaningful recommendations with TF-IDF + Cosine Similarity.

System can be extended with hybrid or collaborative filtering for more accuracy.
---
Future Improvements

Deploy the model using Flask/Streamlit for a web-based app.

Integrate collaborative filtering to improve personalization.

Enhance with deep learning models (e.g., embeddings).
