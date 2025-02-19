# Tweets Sentiment Analysis  

## Overview  
This project aimed to analyze sentiments expressed in tweets related to vaccination using Natural Language Processing (NLP) techniques. The analysis categorized tweets into positive, negative, or neutral sentiments based on their content. The sentiment classification was performed using a Logistic Regression model trained on a dataset of vaccination-related tweets.  

---

## Objectives  
- **Data Collection and Preparation:** Gather tweets containing keywords related to COVID-19 vaccines from Twitter.  
- **Data Preprocessing:** Clean and preprocess text data to prepare it for sentiment analysis.  
- **Sentiment Analysis:** Use NLP techniques to classify tweets into positive, negative, or neutral sentiments.  
- **Model Training and Evaluation:** Train a Logistic Regression model on the preprocessed data and evaluate its accuracy in sentiment classification.  
- **Visualization:** Generate visualizations such as word clouds and sentiment distribution plots to enhance understanding of tweet sentiments.  

---

## Methodology  

### Data Collection  
Twitter was utilized to collect tweets containing hashtags and keywords related to COVID-19 vaccines, focusing on brands like Pfizer, Moderna, AstraZeneca, and others. The dataset (`vaccination_tweets.csv`) includes fields such as tweet text, user information, timestamps, and engagement metrics.  

### Data Preprocessing  
Text preprocessing steps included:  
- Lowercasing text and removing punctuation.  
- Removing URLs, mentions, and hashtags.  
- Tokenization and removing stop words.  
- Stemming or lemmatization to reduce words to their base form.  

### Sentiment Analysis  
- **TextBlob** was employed to compute sentiment polarity for each tweet, which ranges from -1 (negative) to 1 (positive).  
- Tweets were classified into sentiment categories:  
  - **Positive:** Polarity > 0  
  - **Negative:** Polarity < 0  
  - **Neutral:** Polarity = 0  

### Model Training and Evaluation  
- Utilized **CountVectorizer** to convert text data into numerical features.  
- Split data into training and testing sets (80% training, 20% testing).  
- Trained a **Logistic Regression** model using the training data to classify sentiments.  
- Evaluated model accuracy using the testing data, achieving a test accuracy of **84.64%**.  

### Visualization  
- Generated **Word Clouds** to visualize the most frequent words in tweets categorized as positive, negative, and neutral.  
- Used **Seaborn** and **Matplotlib** for visualizing sentiment distribution among tweets.  

---

## Results  
- **Data Insights:**  
  - Majority of tweets were neutral (54.2%), followed by positive (31.1%) and negative (14.7%).  
- **Word Clouds:**  
  - Positive tweets included terms like "effective", "vaccine", and "thanks".  
  - Negative tweets often mentioned "side effects", "concerns", and "hesitant".  
- **Model Accuracy:**  
  - The Logistic Regression model achieved an accuracy of **84.64%** in classifying tweet sentiments.

