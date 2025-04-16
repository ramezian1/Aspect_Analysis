# 📱 Analysis of iPhone Customer Reviews

## Introduction 🚀

This project dives deep into customer feedback for the Apple iPhone 11, going beyond simple star ratings! We're using **Aspect-Based Sentiment Analysis (ABSA)** to pinpoint specific features people talk about (like the 📸 camera, 🔋 battery, or 🖥️ screen) and understand whether they're happy, sad, or neutral about each one. This gives us a much richer understanding of what users really think!

**Author: Robert Mezian**

### **Dataset 📦**
We're working with the "iPhone Reviews from Amazon.com" dataset, packed with over 30,000 reviews scraped from Amazon.com. It includes review text and star ratings.

🔗 **Dataset Link:** [https://www.kaggle.com/datasets/thedevastator/apple-iphone-11-reviews-from-amazon-com](https://www.kaggle.com/datasets/thedevastator/apple-iphone-11-reviews-from-amazon-com)

### **My Approach 🛠️**

Here's how I'll be breaking it down:

1.  **Data Loading & Exploration 🔍** We're starting by loading the data and getting to know it, looking for patterns and insights.
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

### **Setup & Use:**
Download or clone this repo as a zip file. Extract zip file then use Terminal or Command Prompt for the following:
1. **Make sure you have Python 3.11x installed with pip.**
* Activate/Create virtual environment:  
  ``python -m venv myenv``
* Then run a cmd/terminal to the path of the environment: 
  ``cd c://Users//YOURUSERNAME/PATH-TO-GIT-FILE-DOWNLOADED``
* Download all necessary pip files with my 'requirements.txt':

  `pip install -r requirements.txt`

2. **Use your preferred IDE or Jupyter notebook (preferred):**
* Run ``jupyter notebook`` in cmd or terminal (With the path being where the files have been downloaded.)

3. **The notebook will open and you can run code cell by cell, or Run All cells at once and view output.**
*   **NOTE:** Make sure .csv file is in same path as the jupyter notebook source file!


### **Code and Implementation 💻:**
**The complete code for this analysis is available in the `Aspect_Analysis.ipynb` Jupyter Notebook file within this repository.**
1.  **Run the Cells Sequentially:** Once you have pasted all the content into the corresponding cells in your notebook:
2.  Go back to the first cell (Cell 1). You can view Markdown notes to get a summary of each cell thats being outputted.
3.  Run the cells one by one by pressing `Shift + Enter` in each cell, starting from the top.
4.  Watch the output of each code cell to make sure it runs correctly without errors and produces the expected output (tables, plots, verification messages).

---

#### **Limitations 🚧**
* The aspect extraction method relied on a predefined keyword list and simple string matching, which might miss some aspects or misclassify mentions.
* Sentiment analysis used VADER, which is lexicon-based and may not capture complex nuances like sarcasm or context-dependent sentiment as accurately as transformer models.
* The analysis was based on a single dataset for one product model (iPhone 11) from one source (Amazon). Results might differ for other models, time periods, or platforms.
* Sentiment was assigned based on the average score of sentences containing the aspect; more sophisticated methods could link sentiment more directly to the aspect phrase.

#### **Future Work 🚀**
* Implement more advanced aspect extraction techniques (e.g., using dependency parsing or named entity recognition).
* Utilize more sophisticated sentiment analysis models (e.g., fine-tuning BERT or using other transformer-based models).
* Expand the analysis to compare different iPhone models or competitors.
* Analyze the evolution of aspect sentiment over time if timestamps allow.
* Develop an interactive dashboard or tool to explore the results.
---

**© Copyright 2025: Robert Mezian. All Rights Reserved.**
