# Email_Spam_Classifier_ML_Project

The project involves building a spam email classifier using machine learning techniques. 
The notebook follows a structured pipeline:

1. Data Cleaning:
```
 1. Reads a dataset (spam (2).csv) containing labeled email messages.
 2. Drops unnecessary columns and renames relevant ones (v1 → target, v2 → text).
 3. Converts categorical labels (spam and ham) into numerical values using Label Encoding.
 4. Removes missing values and duplicate entries.
```
2. Exploratory Data Analysis (EDA):
```	
 1. Analyzes class distribution (imbalanced dataset with more "ham" emails).
 2. Uses visualizations like pie charts to show the proportion of spam vs. ham.
 3. Computes basic statistics like message length, word count, and sentence count.
```
3. Text Preprocessing:
```
 1. Tokenizes messages using NLTK.
 2. Removes stopwords, punctuation, and applies stemming for feature extraction.
```
4. Model Building:
```
 1. Uses TF-IDF vectorization to convert text into numerical form.
 2. Trains multiple machine learning models, including Naïve Bayes, Logistic Regression, and Random Forest.
```
5. Evaluation:
```
 1. Assesses models using accuracy, precision, recall, and F1-score.
 2. Compares different models to determine the best performer.
```
Key Insights
```
 1. The dataset is imbalanced, meaning the classifier needs techniques like resampling or weighting to improve spam detection.
 2. Spam emails tend to be shorter but more keyword-dense compared to ham emails.
 3. Naïve Bayes often performs well on text classification due to its probabilistic nature.
 4. Feature engineering (removing stopwords, stemming) significantly impacts model performance.
```
Conclusion
```
 1. The best-performing model should be chosen based on a trade-off between precision and recall (since false positives and
    false negatives impact users differently).
 2. Further improvements could involve deep learning models (LSTMs, Transformers) or ensemble techniques.
 3. Additional real-world datasets would help improve generalization.
 4. Deploying the model via a web app or API would make it usable for real-world applications.
```
