# 🎬 MovieLens 100K EDA

Exploratory Data Analysis (EDA) on the [MovieLens 100K dataset](https://grouplens.org/datasets/movielens/100k/).  
This analysis explores rating patterns, user behavior, movie popularity, and genre trends using Python (Pandas, Matplotlib, Seaborn).  

---

## 📂 Dataset
The dataset contains:
- **u.data** → User ratings (user_id, movie_id, rating, timestamp)  
- **u.item** → Movie metadata (title, release date, genres)  
- **u.user** → User demographics (not used in this analysis but available)  

📌 Download from: [MovieLens 100K dataset](https://grouplens.org/datasets/movielens/100k/)  

---

## ⚙️ Setup

```bash
# Clone repo
git clone https://github.com/<your-username>/movielens-eda.git
cd movielens-eda

# Install dependencies
pip install -r requirements.txt

📊 Analysis Highlights
1. User Behavior & Demographics

User bias → Some users consistently rate higher or lower than others.

Demographic breakdowns → Ratings compared by gender, age group, and occupation.

Which occupations are “generous” vs “strict” raters.

Age group trends in generosity vs harshness.

2. Movie Similarity & Correlation

Correlation matrix of movies → Found clusters of movies rated similarly by the same users (e.g. Star Wars vs Empire Strikes Back).

Genre overlap heatmap → Identified which genres share strong fan bases.

Hierarchical clustering & network graph → Visualized groups of similar movies.

3. Temporal Trends

User rating behavior over time → Do users become stricter/more generous as they watch more?

Long-term popularity → Which movies sustain attention vs fade quickly.

Decay analysis → Compared how older classics are rated vs newer releases.

4. Advanced Analytics

Cold-start problem → New/unrated movies vs well-known ones.

Added Bayesian shrinkage to adjust inflated ratings of little-known movies.

Compared “top movies” before vs after adjustment.

Rating variance → Identified polarizing movies with the highest disagreement (love-it-or-hate-it titles).

📈 Key Learnings

Bias exists at both the user and occupation level.

Genres cluster naturally, showing shared audiences (e.g. Sci-Fi & Action).

Movie lifecycles reveal how quickly popularity fades vs sustains.

Cold-start adjustment is critical in recommender systems — prevents overrating obscure films.

High variance movies highlight cult classics, controversial dramas, and divisive comedies.
