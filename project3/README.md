# Project 3 --- Comparative Analysis of Bag-of-Words Representations for Medical Transcript Classification

**Notebook:** `Yalda_Chamani_Project3.ipynb`\
**Folder:** `Project 3`

------------------------------------------------------------------------

## 📌 Project Description

This project explores the effectiveness of **Binary Bag-of-Words** and
**Frequency Bag-of-Words** text representations for **medical transcript
classification**. Several machine learning models are applied and
compared to evaluate which representation yields better performance in
this domain.

------------------------------------------------------------------------

## 📊 Dataset

The project uses three datasets:\
- `train.csv` --- training set\
- `valid.csv` --- validation set\
- `test.csv` --- test set

Each dataset contains two columns:\
- **text** --- medical transcript (string)\
- **label** --- class label (integer)

------------------------------------------------------------------------

## 🛠️ Tools & Libraries

-   Python 3.x\
-   Pandas, NumPy\
-   Regex (`re`), String\
-   Collections (Counter)\
-   Scikit-learn (LogisticRegression, DecisionTreeClassifier,
    RandomForestClassifier, f1_score)\
-   XGBoost (XGBClassifier)\
-   tqdm (progress tracking)

------------------------------------------------------------------------

## 🚀 Workflow

1.  **Load Datasets** --- Import training, validation, and test sets.\
2.  **Preprocessing** --- Lowercasing, punctuation removal, whitespace
    normalization.\
3.  **Vocabulary Building** --- Construct vocabulary from top 10,000
    words in training data.\
4.  **Feature Extraction** --- Represent texts as:
    -   **Binary BoW** (presence/absence of words)\
    -   **Frequency BoW** (word counts)\
5.  **Model Training** --- Train multiple classifiers:
    -   Logistic Regression\
    -   Decision Tree\
    -   Random Forest\
    -   XGBoost\
6.  **Evaluation** --- Compare models using **F1-score** on validation
    and test sets.

------------------------------------------------------------------------

## 📈 Results

-   **Binary BoW** often generalizes better with simpler models (e.g.,
    Logistic Regression).\
-   **Frequency BoW** captures more nuance but can lead to overfitting
    with smaller datasets.\
-   Ensemble methods (Random Forest, XGBoost) show improved performance
    over single classifiers.\
-   **F1-scores** highlight trade-offs between representations depending
    on the chosen model.

------------------------------------------------------------------------

## 🎯 Learning Outcome

-   Understand the differences between **binary vs. frequency-based
    BoW** representations.\
-   Gain hands-on experience in **text preprocessing and feature
    extraction**.\
-   Compare multiple **machine learning classifiers** on the same text
    classification task.\
-   Learn how evaluation metrics (F1-score) guide model and feature
    selection.
