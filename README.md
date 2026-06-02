## Movie Genre Classifier

A big data machine learning pipeline that predicts movie genres using a 
One-vs-Rest classification strategy with PySpark ML — training a separate 
model per genre across Random Forest, Decision Tree, and Naive Bayes.

## Models Used
- Random Forest (best performer)
- Decision Tree
- Naive Bayes

## Results After Hyperparameter Tuning

### Random Forest
| Genre | Accuracy |
|---|---|
| TV Movie | 0.9900 |
| Western | 0.9820 |
| War | 0.9795 |
| Music | 0.9775 |
| History | 0.9800 |
| Foreign | 0.9810 |
| Animation | 0.9700 |
| Fantasy | 0.9600 |
| Science Fiction | 0.9485 |
| Mystery | 0.9480 |
| Adventure | 0.9400 |
| Crime | 0.9350 |
| Romance | 0.9300 |
| Drama | 0.9200 |
| Comedy | 0.9250 |
| Documentary | 0.9250 |
| Horror | 0.9150 |
| Thriller | 0.9155 |
| Action | 0.9125 |
| Family | 0.9465 |

### Decision Tree
| Genre | Accuracy |
|---|---|
| TV Movie | 0.9840 |
| Western | 0.9827 |
| War | 0.9748 |
| Music | 0.9721 |
| History | 0.9741 |
| Foreign | 0.9684 |
| Animation | 0.9692 |
| Fantasy | 0.9558 |
| Science Fiction | 0.9485 |
| Mystery | 0.9505 |
| Adventure | 0.9312 |
| Crime | 0.9205 |
| Romance | 0.8725 |
| Drama | 0.6953 |
| Comedy | 0.7669 |
| Documentary | 0.9452 |
| Horror | 0.9159 |
| Thriller | 0.8571 |
| Action | 0.8789 |
| Family | 0.9463 |

> Random Forest outperformed Decision Tree across almost all genres, 
> particularly on Drama (0.92 vs 0.70), Comedy (0.93 vs 0.77) 
> and Thriller (0.92 vs 0.86).

## What's Inside
- Data cleaning and preprocessing with PySpark
- Categorical encoding using StringIndexer
- Feature engineering with VectorAssembler and Word2Vec
- One-vs-Rest classification across 20 genres
- Model evaluation using Accuracy, F1 Score, Precision and Recall
- Hyperparameter tuning on top 2 models
- Confusion matrix analysis for Random Forest and Decision Tree

## Stack
`PySpark` · `PySpark ML` · `Google Colab`

## Dataset
TMDB Movies Dataset — contains movie metadata including genres, 
popularity, revenue, runtime and vote averages.
