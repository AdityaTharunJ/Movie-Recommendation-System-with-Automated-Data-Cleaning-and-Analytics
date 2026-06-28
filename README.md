# 🎬 IMDb Movie Recommendation System

A Python-based movie recommendation system that suggests movies based on user preferences such as **Genre**, **Minimum IMDb Rating**, and **Maximum Runtime**. The project also demonstrates **data cleaning, preprocessing, and automation** using the IMDb Top 1000 Movies dataset.

---

## 📌 Project Overview

Choosing a movie can often be overwhelming due to the large number of available options. This project simplifies the process by allowing users to filter movies based on their preferred genre, IMDb rating, and runtime.

The system first performs data preprocessing and cleaning on the IMDb dataset and then provides personalized movie recommendations through an interactive command-line interface.

---

## 🚀 Features 

* Interactive command-line interface
* Displays all available movie genres for easy selection
* Validates user inputs to prevent invalid entries

Filters movies based on:
* Genre
* Minimum IMDb Rating
* Maximum Runtime

* Recommends the Top 10 matching movies
* Performs automated data cleaning using Pandas
* Generates visualizations for exploratory data analysis (EDA)
* Handles cases where no matching movies are found
* Allows users to perform multiple searches without restarting the application

---

## 🛠️ Technologies Used

* Python
* Pandas
* Google Colab / Jupyter Notebook
* CSV Dataset (IMDb Top 1000 Movies)

---

## 📂 Dataset

Dataset Used:

**IMDb Top 1000 Movies Dataset**

The dataset contains information such as:

* Movie Title
* Genre
* IMDb Rating
* Runtime
* Director
* Cast
* Certificate
* Meta Score
* Number of Votes
* Gross Collection
* Overview
* Release Year

---

## ⚙️ Data Cleaning

Before building the recommendation system, the dataset was cleaned and preprocessed using Pandas.

The following operations were performed:

* Removed duplicate records
* Handled missing values
* Removed unnecessary whitespace
* Standardized runtime values
* Converted runtime into numeric format
* Exported a cleaned dataset for recommendation

---

## ▶️ How It Works

### Step 1

Run the recommendation script.

```
python recommendation.py
```

---

### Step 2

The application displays all available genres.

Example:

```
==================================================
🎬 IMDb Movie Recommendation System
==================================================

--- Movie Recommendation Menu ---

Available Genres:
1. Action
2. Adventure
3. Animation
4. Biography
5. Biography
6. Comedy
7. Crime
8. Drama
9. Family
10. Fantasy
11. Film-Noir
12. History
13. Horror
14. Music
15. Musical
16. Mystery
17. Romance
18. Sci-Fi
19. Sport
20. Thriller
21. War
22. Western
```

---

### Step 3

Enter the following:

* Genre Number
* Minimum IMDb Rating
* Maximum Runtime

Example:

```

Enter a number for Genre (1-22): 20
Minimum IMDb Rating (0-10): 5
Maximum Runtime (minutes): 200
```

---

### Step 4

The system recommends the best matching movies.

Example Output

```
Recommended Movies for Genre: Thriller, Min Rating: 5.0, Max Runtime: 200 minutes

************************
Title:  Gisaengchung
Genre:  Comedy, Drama, Thriller
IMDB Rating:  8.6
Runtime:  132 min
Director:  Bong Joon Ho
************************
************************
Title:  The Silence of the Lambs
Genre:  Crime, Drama, Thriller
IMDB Rating:  8.6
Runtime:  118 min
Director:  Jonathan Demme
************************
************************
Title:  Joker
Genre:  Crime, Drama, Thriller
IMDB Rating:  8.5
Runtime:  122 min
Director:  Todd Phillips
************************
************************
Title:  The Departed
Genre:  Crime, Drama, Thriller
IMDB Rating:  8.5
Runtime:  151 min
Director:  Martin Scorsese
************************
************************
Title:  The Usual Suspects
Genre:  Crime, Mystery, Thriller
IMDB Rating:  8.5
Runtime:  106 min
Director:  Bryan Singer
************************
************************
Title:  Psycho
Genre:  Horror, Mystery, Thriller
IMDB Rating:  8.5
Runtime:  109 min
Director:  Alfred Hitchcock
************************
************************
Title:  The Lives of Others
Genre:  Drama, Mystery, Thriller
IMDB Rating:  8.4
Runtime:  137 min
Director:  Florian Henckel von Donnersmarck
************************
************************
Title:  Memento
Genre:  Mystery, Thriller
IMDB Rating:  8.4
Runtime:  113 min
Director:  Christopher Nolan
************************
************************
Title:  Rear Window
Genre:  Mystery, Thriller
IMDB Rating:  8.4
Runtime:  112 min
Director:  Alfred Hitchcock
************************
************************
Title:  1917
Genre:  Drama, Thriller, War
IMDB Rating:  8.3
Runtime:  119 min
Director:  Sam Mendes
************************

Do you want to find more movies? (yes/no): no
Thank you for using the IMDb Movie Recommendation System!
```

---

## 📊 Recommendation Logic

The recommendation engine filters movies using the following criteria:

* Selected Genre
* IMDb Rating greater than or equal to the user-defined minimum rating
* Runtime less than or equal to the user-defined maximum runtime

The filtered movies are then sorted in descending order of IMDb Rating, and the top 10 recommendations are displayed.

---

## 📸 Sample Workflow

```
Start Program
      │
      ▼
Load Cleaned Dataset
      │
      ▼
Display Available Genres
      │
      ▼
Take User Inputs
      │
      ▼
Validate Inputs
      │
      ▼
Filter Movies
      │
      ▼
Sort by IMDb Rating
      │
      ▼
Display Top 10 Recommendations
      │
      ▼
Search Again?
      │
      ├── Yes → Repeat
      │
      └── No → Exit
```
---
## 📊 Data Visualization

To better understand the IMDb dataset, several visualizations were created after data cleaning.

1. IMDb Ratings Distribution

This histogram shows the distribution of IMDb ratings across all movies in the dataset.

Insights:

* Most movies have IMDb ratings between 7.5 and 8.2.
* Very few movies have ratings above 9.0, highlighting their rarity.
* The distribution is slightly right-skewed, indicating that exceptionally high-rated movies are uncommon.

2. IMDb Ratings Distribution Across Genres

A box plot was generated to compare IMDb ratings across different movie genres.

Insights:

* Most genres have median IMDb ratings around 8.0.
* Some genres, such as Drama and Biography, tend to have slightly higher ratings.
* Outliers represent critically acclaimed movies with exceptionally high IMDb ratings.
* The visualization helps compare rating consistency across genres.
---

## 📈 Exploratory Data Analysis (EDA)

The project includes exploratory data analysis to identify patterns and trends in the dataset before building the recommendation system.

EDA techniques include:

Distribution of IMDb Ratings
IMDb Ratings Across Genres
Missing Value Analysis
Duplicate Record Detection
Runtime Conversion and Analysis
Genre Frequency Analysis

## 🎯 Future Improvements

* Develop a graphical user interface using Streamlit
* Add movie posters using TMDb API
* Include actor-based recommendations
* Include director-based recommendations
* Recommend similar movies using Machine Learning
* Deploy the application online

---

## 👨‍💻 Author

**Aditya Tarun J**

B.Tech Student (Computer Science - AI & Data Science)

---

## 📄 License
This project is intended for educational and learning purposes.


