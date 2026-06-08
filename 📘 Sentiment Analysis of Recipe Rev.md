# 📘 Sentiment Analysis of Recipe Reviews Using Classical NLP Techniques

##### 🔎 Project Overview



This project explores sentiment analysis of recipe reviews using classical NLP techniques and machine learning models.



##### 📊 Dataset

* Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/911/recipe+reviews+and+user+feedback+dataset)
* Records: 18,182 recipe reviews
* Features include:
* Review text
* Star ratings
* User reputation
* Review engagement metrics
* Recipe information
* Timestamps



##### The workflow includes:



* Data cleaning and feature engineering
* Exploratory Data Analysis (EDA)
* Text preprocessing (tokenization, stopword removal, lemmatization)
* Baseline sentiment analysis with VADER
* Text vectorization (CountVectorizer, TF‑IDF)
* Classification models (Logistic Regression, Naive Bayes, Linear SVC)
* Handling class imbalance with SMOTE
* Model evaluation and comparison



##### Key Findings:



* The dataset is strongly imbalanced toward positive reviews and high star ratings.
* VADER sentiment scores show a positive relationship with user ratings.
* TF-IDF generally outperformed CountVectorizer in rating prediction tasks.
* Applying SMOTE improved minority-class detection in sentiment classification.
* Linear SVC achieved the strongest overall performance (Accuracy ≈ 75%, Weighted F1 ≈ 0.78).
* Neutral and negative reviews remain the most difficult classes to predict accurately.



##### 🤖 Models Evaluated



* ###### Rating Classification (1–5 Stars)
* Logistic Regression
* Multinomial Naive Bayes
* ###### Sentiment Classification (3 Classes)
* Logistic Regression + SMOTE
* Multinomial Naive Bayes + SMOTE
* Linear SVC + SMOTE
* ##### Use of AI tools

AI tools (ChatGPT) were used occasionally during the development of this project for:

* debugging support in Python code,
* clarifying machine learning concepts during implementation,
* improving the clarity and structure of explanations in the notebook and presentation slides.

All final code, model decisions, and results were independently developed, tested, and validated.



##### 📂 Included Files in ZIP



* Sentiment\_Analysis\_Notebook.ipynb → Main Jupyter Notebook with full analysis
* Recipe Reviews and User Feedback Dataset.csv → Dataset (from UCI Machine Learning Repository)
* README.txt → Project documentation (this file)
* Presentation slides (PDF format)





##### ⚙️ Instructions to Run the Analysis



1. ###### Unzip the project folder



Extract the ZIP file to your preferred location.



###### 2\. Set up environment



Recommended: create a virtual environment.



Install dependencies using the requirements file:



pip install -r requirements.txt



###### 3\. Run the notebook

&#x20;

Open Jupyter Notebook or JupyterLab and launch:



jupyter notebook Sentiment\_Analysis\_Notebook.ipynb



##### 📦 Required Python Libraries



The analysis uses the following libraries:



* ###### Data Handling \& Visualization



* pandas
* numpy
* matplotlib
* seaborn



* ###### NLP



* nltk (stopwords, wordnet, punkt, vader\_lexicon)



* ###### Machine Learning



* scikit-learn (LogisticRegression, MultinomialNB, LinearSVC, metrics, train\_test\_split, vectorizers)
* imbalanced-learn (SMOTE)

