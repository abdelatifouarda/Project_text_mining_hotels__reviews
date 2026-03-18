# Project_text_mining_hotels__reviews
# Hotel Reviews Text Mining Analysis

## Project Overview

Understanding customer feedback is essential in the hospitality industry.
Online reviews provide valuable insights into how guests perceive hotel services, facilities, and overall experiences.

This project applies **Natural Language Processing (NLP)** and **text mining techniques** to analyze hotel review data and identify common themes in guest feedback.

Using Python-based data analysis tools, the project explores linguistic patterns in hotel reviews, extracts important keywords, and examines sentiment trends across the dataset.

The main objective is to demonstrate how text mining methods can transform unstructured review text into meaningful insights.

---

# Dataset Description

The dataset used in this project contains information about 30 hotels, including:

* Hotel name
* Star rating
* Total number of reviews
* Aggregated review text

The dataset represents publicly available hotel review information.

It is important to note that:

* The dataset is relatively small
* Reviews appear in aggregated form rather than individual entries
* Most hotels have high ratings (above 4.5)

Because of these characteristics, the analysis should be interpreted as **exploratory rather than statistically conclusive**.

---

# Project Workflow

The analysis follows a standard **NLP text mining pipeline**.

### 1. Data Preparation

* Loading the dataset
* Cleaning column formats
* Converting numerical values
* Handling missing data

### 2. Exploratory Data Analysis (EDA)

* Distribution of hotel ratings
* Review volume comparison
* Identification of highly reviewed hotels

### 3. Text Preprocessing

The review text was cleaned using common NLP preprocessing techniques:

* Lowercasing
* Tokenization
* Stopword removal
* Removal of punctuation
* Text normalization

These steps help standardize the text and improve the quality of text analysis.

### 4. Keyword Extraction (TF-IDF)

Term Frequency–Inverse Document Frequency (TF-IDF) was applied to identify the most important words within the corpus.

TF-IDF highlights words that appear frequently in specific documents while being less common across the entire dataset.

This allows the analysis to detect distinctive terms used in hotel reviews.

### 5. N-gram Analysis

Bigram analysis was performed to identify commonly occurring word pairs.

Examples of recurring expressions include:

* "great service"
* "friendly staff"
* "excellent location"

These phrase patterns provide insight into how guests summarize their experiences.

### 6. Text Similarity Analysis

Cosine similarity was used to measure similarity between hotel review texts.

This method helps identify hotels with similar review language and potentially similar guest experiences.

### 7. Sentiment Analysis

Sentiment analysis was conducted using the VADER sentiment analyzer.

The model assigns polarity scores to review text, indicating whether the sentiment is:

* Positive
* Neutral
* Negative

These scores were compared with hotel star ratings to observe general sentiment patterns.

---

# Key Insights

Several patterns emerge from the text mining analysis.

### 1. Ratings Distribution

The dataset is heavily skewed toward highly rated hotels.
More than half of the hotels have ratings above 4.5.

As a result, the textual corpus is dominated by **positive guest experiences**.

---

### 2. Relationship Between Reviews and Ratings

Exploratory analysis suggests a weak positive relationship between review volume and hotel rating.

Hotels with strong ratings tend to accumulate a larger number of reviews.
However, the dataset does not allow causal interpretation.

---

### 3. Dominant Themes in Reviews

TF-IDF analysis highlights several key themes frequently mentioned by guests:

Service quality
Room comfort
Location
Food and dining

These categories appear consistently across many hotel reviews.

---

### 4. Common Review Phrases

Bigram analysis reveals recurring phrases that guests commonly use to evaluate hotels.

Examples include:

* great service
* friendly staff
* excellent location

These short expressions function as concise summaries of guest satisfaction.

---

### 5. Differences Between Higher and Lower Rated Hotels

Vocabulary patterns differ slightly between higher-rated and relatively lower-rated hotels.

Highly rated hotels often appear with strong evaluative language such as:

* excellent
* wonderful
* great

In contrast, lower-rated hotels contain more operational descriptions such as:

* front desk
* check-in
* reception

This suggests that guests tend to describe operational issues when experiences are less positive.

---

### 6. Sentiment Patterns

Sentiment analysis indicates that most reviews carry positive sentiment scores.

This result aligns with the rating distribution of the dataset, where most hotels receive high ratings.

However, sentiment analysis results should be interpreted cautiously due to the limited dataset size.

---

# Tools and Technologies

The project was implemented using the following tools:

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
NLTK
Word clouds
These libraries are commonly used in **data analysis and natural language processing workflows**.

# Limitations

Several limitations affect the scope of the analysis.

* The dataset contains only 30 hotels.
* Review text appears aggregated rather than individual.
* The dataset lacks timestamps and reviewer metadata.
* Sentiment analysis relies on a rule-based model.

Because of these factors, the findings should be interpreted as **exploratory insights rather than definitive conclusions**.

---

# Future Work

Future improvements could significantly extend this analysis.

Possible directions include:

* Expanding the dataset with hundreds of hotels
* Collecting individual review entries
* Applying topic modeling techniques (LDA)
* Training machine learning models for sentiment classification
* Building predictive models linking review text to hotel ratings

These extensions would enable deeper and more robust text analysis.

---

# Author

This project was created as part of a personal **Data Analysis and Natural Language Processing learning portfolio**.

It demonstrates practical applications of text mining techniques for analyzing customer feedback data.
