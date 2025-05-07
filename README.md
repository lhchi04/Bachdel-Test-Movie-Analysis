# Bachdel-Test-Movie-Analysis
Data analysis and predictive modeling on gender representation in films using Bechdel Test scores and movie metadata.

# Bechdel Test Movie Analysis

This project analyzes gender representation in films using Bechdel Test scores, movie metadata, and financial information. Drawing from two public datasets, we explore historical trends and build predictive models to estimate the likelihood that a film passes the Bechdel Test.

## Datasets

We combined two sources:
- **Kaggle: [IMDb and Bechdel Dataset](https://www.kaggle.com/datasets/nliabzd/movies-imdb-and-bechdel-information)** — over 9,000 films with Bechdel Test ratings, genres, IMDb ratings, and runtimes.
- **[FiveThirtyEight GitHub Dataset](https://github.com/fivethirtyeight/data/blob/master/bechdel/movies.csv)** — ~1,700 films with additional financial attributes (budgets, domestic and international gross).

## Objective

- Understand trends in female representation in film using Bechdel ratings.
- Engineer features such as profit, decade of release, and pass/fail binary label.
- Train machine learning models to predict whether a film passes the Bechdel Test.
- Evaluate model performance across different time ranges (full dataset vs. 1970–2010).

## Methods

- **Data Cleaning & Merging**: Merged datasets using movie titles, resolved inconsistencies in formatting and missing values.
- **Feature Engineering**: Created new features such as `total_gross`, `profit`, `release_decade`, and a binary `bechdel_pass` label.
- **Visualization**: Trend analysis by decade, feature averages by Bechdel rating, and network graphs to explore relationships.
- **Modeling**: Built classifiers (Logistic Regression, Decision Tree, Random Forest, KNN) to predict Bechdel Test outcomes.

## Results

- Logistic Regression showed high recall for passing films but poor performance on non-passing films.
- Decision Tree and Random Forest offered more balanced results.
- KNN benefited from feature scaling but did not outperform simpler models.
- Filtering to films from 1970–2010 did not significantly improve accuracy but improved interpretability.

