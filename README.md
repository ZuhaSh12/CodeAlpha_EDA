# 📊 Netflix Titles – Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on the [Netflix Titles Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows).
The dataset contains information about movies and TV shows available on Netflix as of 2021.

The goal is to explore:

* Distribution of **Movies vs TV Shows**
* Content trends by **year**, **country**, **rating**, and **genre**
* Average **duration** of Movies and TV Shows
* **Hypothesis testing** using statistical methods
* Detect **patterns, anomalies, and data issues**

---

## 🗂 Dataset

* **Rows:** 8,807
* **Columns:** 12
* **Key Variables:**

  * `type` → Movie / TV Show
  * `title` → Title of the content
  * `director`, `cast`, `country` → Metadata
  * `date_added` → When it was added to Netflix
  * `release_year` → Original release year
  * `rating` → TV rating (e.g., TV-MA, PG-13)
  * `duration` → Minutes (Movies) or Seasons (TV Shows)
  * `listed_in` → Genres
  * `description` → Short summary

⚠️ **Note**: Missing values exist in `director`, `cast`, and `country`.

---

## 🔍 Analysis & Insights

### Key Questions Explored

1. Movies vs TV Shows distribution
2. Content releases over time
3. Top contributing countries
4. Content ratings (TV-MA, PG, etc.)
5. Movie duration analysis
6. Genre popularity and trends
7. Relationship analysis (country vs rating, year vs genre)

### Key Insights

* Netflix started **movie-heavy** but shifted towards **TV Shows** after 2015.
* The **United States** dominates, but India and other countries are rising.
* **TV-MA (mature audience)** is the most common rating.
* Average movie duration ≈ **100 minutes** (normal industry length).
* TV Shows mostly last **1–3 seasons**.
* **Top genres**: Drama, Comedy, Documentaries, International content.
* Regional patterns: **US → Mature content**, **India → Teen/Family content**.

---

## 📊 Visualizations

* Movies vs TV Shows trend (stacked bar)
* Pie chart of top countries
* Ratings distribution (bar chart)
* Movie duration distribution (histogram with range markers)
* Genre trends over time (stacked bar)
* Country vs Rating (bar chart)
* Correlation heatmap

---

## 📈 Hypothesis Testing

* ✅ Netflix has been adding **more TV Shows** in recent years (**Chi-square test, p < 0.05**).
* ✅ Majority of content originates from the **US** (\~55%).
* ✅ **TV-MA dominates** Netflix’s catalog.
* ✅ Average movie duration is **within 90–120 minutes** (**t-test confirmed**).

---

## 🛠 Tools & Libraries

* **Python 3**
* **pandas, numpy** → data cleaning & manipulation
* **matplotlib, seaborn** → visualization
* **scipy.stats** → hypothesis testing

---

## 🚀 How to Run

1. Clone the repo:

   ```bash
   git clone https://github.com/your-username/netflix-eda.git
   cd netflix-eda
   ```
2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebook or Python script for EDA.

---

## 📂 Repository Structure

```
netflix-eda/
│-- data/
│   └── netflix_titles.csv
│-- notebooks/
│   └── netflix_eda.ipynb
│-- visuals/
│   └── plots.png (sample plots)
│-- README.md
│-- requirements.txt
```

---

## 📌 Future Work

* Build interactive **dashboard (Plotly/Dash/Streamlit)**.
* Apply **ML models** to predict rating or genre.
* Update with **latest Netflix dataset** (2025).

---

## 🙌 Acknowledgements

* Dataset source: [Kaggle – Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows).

---

Would you like me to also create a **requirements.txt** file (listing pandas, seaborn, matplotlib, scipy, etc.) so your GitHub repo is fully reproducible?
