# 📱 Analysis of iPhone Customer Reviews

## Introduction 🚀

This project dives deep into customer feedback for the Apple iPhone 11, going beyond simple star ratings! We're using **Aspect-Based Sentiment Analysis (ABSA)** to pinpoint specific features people talk about (like the 📸 camera, 🔋 battery, or 🖥️ screen) and understand whether they're happy, sad, or neutral about each one. This gives us a much richer understanding of what users really think!

### **Dataset 📦**
We're working with the "iPhone Reviews from Amazon.com" dataset, packed with over 30,000 reviews scraped from Amazon.com. It includes review text and star ratings.

🔗 **Dataset Link:** [https://www.kaggle.com/datasets/thedevastator/apple-iphone-11-reviews-from-amazon-com](https://www.kaggle.com/datasets/thedevastator/apple-iphone-11-reviews-from-amazon-com)

### **My Approach 🛠️**

Here's how I'll be breaking it down:

1.  **Data Loading & Exploration 🔍:** We're starting by loading the data and getting to know it, looking for patterns and insights.
2.  **Text Preprocessing 🧹** We're cleaning up the review text by making everything lowercase, removing punctuation and numbers, and using spaCy to lemmatize words and remove stop words.
3.  **Aspect Extraction 🎯** We're finding the key features people talk about using frequency analysis (CountVectorizer) and matching them against a list of relevant iPhone features.
4.  **Sentiment Assignment 😃😐😞** We're using NLTK's VADER sentiment analyzer to figure out the sentiment (positive, negative, or neutral) for each aspect in the sentences where they appear.
5.  **Analysis & Visualization 📈** Finally, we're summarizing and visualizing the sentiments to see what people really think about each aspect.

### **Key Libraries 📚**

* **Pandas 🐼** For handling and manipulating our data.
* **NLTK 🗣️** For sentiment analysis (VADER) and sentence tokenization.
* **spaCy 💫** For text preprocessing, including lemmatization and stop word removal.
* **Scikit-learn 🤖** For feature extraction using CountVectorizer.
* **Matplotlib & Seaborn 📊** For creating insightful data visualizations.
* **re 🔍** For regular expressions, helping us clean the text.

---

**© Copyright 2025: Robert Mezian. All Rights Reserved.**
