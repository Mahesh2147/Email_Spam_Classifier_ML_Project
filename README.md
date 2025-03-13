# Email_Spam_Classifier_ML_Project

The project involves building a spam email classifier using machine learning techniques. 
The notebook follows a structured pipeline:

1. Data Cleaning:
```
	Reads a dataset (spam (2).csv) containing labeled email messages.
	Drops unnecessary columns and renames relevant ones (v1 → target, v2 → text).
	Converts categorical labels (spam and ham) into numerical values using Label Encoding.
	Removes missing values and duplicate entries.
```
2. Exploratory Data Analysis (EDA):
```	
  	Analyzes class distribution (imbalanced dataset with more "ham" emails).
	Uses visualizations like pie charts to show the proportion of spam vs. ham.
	Computes basic statistics like message length, word count, and sentence count.
```
3. Text Preprocessing:
```
	Tokenizes messages using NLTK.
	Removes stopwords, punctuation, and applies stemming for feature extraction.
```
4. Model Building:
```
	Uses TF-IDF vectorization to convert text into numerical form.
	Trains multiple machine learning models, including Naïve Bayes, Logistic Regression, and Random Forest.
```
5. Evaluation:
```
	Assesses models using accuracy, precision, recall, and F1-score.
	Compares different models to determine the best performer.
```
Key Insights
```
	The dataset is imbalanced, meaning the classifier needs techniques like resampling or weighting to improve spam detection.
	Spam emails tend to be shorter but more keyword-dense compared to ham emails.
	Naïve Bayes often performs well on text classification due to its probabilistic nature.
	Feature engineering (removing stopwords, stemming) significantly impacts model performance.
```
Conclusion
```
	The best-performing model should be chosen based on a trade-off between precision and recall (since false positives and
	false negatives impact users differently).
	Further improvements could involve deep learning models (LSTMs, Transformers) or ensemble techniques.
	Additional real-world datasets would help improve generalization.
	Deploying the model via a web app or API would make it usable for real-world applications.
```
