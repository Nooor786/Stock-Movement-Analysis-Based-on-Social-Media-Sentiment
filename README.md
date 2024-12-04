#  📊 Reddit Sentiment Analysis and Stock Movement Prediction

<i>Analyze Reddit discussions, uncover market sentiment, and predict stock trends.</i>

## 📜 Project Overview
This project leverages Reddit data to analyze sentiment, extract meaningful features, and predict stock market movements. By combining natural language processing (NLP) with machine learning, the project highlights the power of social media in understanding market dynamics.

### Key Features:
* Reddit Data Scraping: Fetch Reddit posts using the PRAW API.
* Sentiment Analysis: Use VADER and TextBlob to calculate sentiment scores.
* Data Visualization: Identify trends through word clouds, score distributions, and scatter plots.
* Machine Learning: Train models to predict sentiment and its correlation to stock behavior.




## 🚀 Getting Started
### 1. Prerequisites
Ensure you have Python latest version installed, along with the following libraries:

+ praw
+ pandas
+ nltk
+ TextBlob
+ matplotlib
+ seaborn
+ scikit-learn
+ wordcloud
  
### 2. Configure Reddit API
+ Create an app in the Reddit Developer Portal.
+ Replace client_id, client_secret, and user_agent placeholders in the script with your credentials.

## 📊 Visualizations
	
+ Sentiment Trends Over Time  ---> Line graph showing daily sentiment averages.	
+ Word Cloud	               ---> Highlights common keywords in post titles.	
+ Score Distribution	       ---> Histogram showing the frequency of post scores.	
+ Sentiment vs. Post Score	 ---> Scatter plot showing the relationship between sentiment scores and post scores.


## 📂 Project Structure


├── code.ipynb ::::::::        # Main Jupyter Notebook

├── README.md        ::::::::        # Project Documentation

├── requirements.txt ::::::::        # Python Dependencies

└── data/            ::::::::        # Placeholder for Datasets (Optional)

## 🔬 Model Evaluation
Model Used: Logistic Regression

Metrics:
+ Accuracy: 85%
+ Precision: High for positive sentiment predictions
+ Recall: Needs improvement for neutral sentiment
  
Insights:
VADER sentiment scores are the strongest predictors.
Combining VADER and TextBlob improves accuracy.


## 🔮 Future Expansions
### Data Source Integration:

- Incorporate data from other platforms like Twitter and StockTwits.
- Use financial news sentiment analysis (e.g., NewsAPI or Alpha Vantage).
  
### Feature Enhancements:

- Include Reddit post comments for deeper insights.
- Analyze sentiment around specific stock mentions (e.g., $AAPL).

### Advanced Modeling:

- Experiment with transformer models (e.g., BERT) for nuanced sentiment detection.
- Implement time-series models (e.g., LSTM) for trend predictions.

### Real-Time Analytics:

- Build a pipeline for live sentiment analysis and stock trend predictions.



## STEP BY STEP PROCESS 

### Step 1: Define the Objective
The primary goal is to use Reddit discussions to analyze market sentiment and predict stock trends. The objectives include:

Scraping Reddit data for relevant posts.
Performing sentiment analysis to understand public opinion.
Using sentiment and metadata to predict stock movement patterns.

### Step 2: Setup and Prerequisites
### Environment Setup:
Install Python (3.7+ recommended) and required libraries. Use pip install -r requirements.txt to ensure dependencies like praw, nltk, and scikit-learn are installed.

### Reddit API Configuration:

Register a new app on the Reddit Developer Portal.
Obtain the client_id, client_secret, and user_agent.
Configure the API in the code to authenticate and connect to Reddit.

### Step 3: Scrape Reddit Data
### Connect to Reddit API:
Use the praw library to fetch posts from target subreddits like r/stocks or r/wallstreetbets.

Query parameters define the data scope (e.g., time period, keywords).
Extract metadata such as:
Post title.
Upvote score.
Timestamp.
Challenges and Resolutions:

Limited API responses: Handle this using pagination techniques.
Irrelevant posts: Filter based on specific keywords related to stocks.

### Step 4: Preprocess Data
### Clean Text Data:

Remove special characters, URLs, and non-alphabetic text from post titles.
Convert text to lowercase for uniformity.
Filter Posts:

Retain only posts with a minimum engagement score to focus on influential discussions.
Generate New Features:

Add sentiment scores using VADER and TextBlob.
Convert timestamps to readable dates for time-based trend analysis.

### Step 5: Sentiment Analysis
### Tools Used:

VADER (Valence Aware Dictionary and sEntiment Reasoner):
Provides a compound sentiment score, categorizing posts as positive, negative, or neutral.
TextBlob:
Offers polarity (sentiment strength) and subjectivity (level of opinion vs. fact).
Output:
Each post is labeled with sentiment scores, enabling correlation with stock trends.

### Step 6: Visualization and Analysis
### Data Exploration:

Use pandas to understand trends, outliers, and distributions.
Examine relationships between sentiment scores, upvotes, and timestamps.
Visualizations:

Word Cloud: Identify frequently discussed terms.
Sentiment Trends: Plot sentiment scores over time to observe fluctuations.
Score Distribution: Analyze the distribution of post scores.
Scatter Plot: Visualize correlations between sentiment scores and engagement.

### Step 7: Machine Learning Model
### Model Selection:

Train a logistic regression model to predict sentiment categories (positive, negative, neutral).
Features Used:

Sentiment scores (VADER and TextBlob).
Post engagement metrics (upvotes).
Temporal features (day or time).
Evaluation Metrics:

Accuracy, precision, recall, and F1-score were calculated.
Confusion matrix highlights performance for each sentiment category.

### Step 8: Model Insights
### Findings:

Sentiment scores (especially from VADER) strongly correlate with stock movement indicators.
Post engagement (upvotes) adds valuable predictive power.
Limitations:

Neutral sentiments were harder to classify accurately.
Model accuracy could improve with more advanced algorithms and larger datasets.


### Step 9: Suggestions for Future Work
### Data Integration:

Combine Reddit data with other platforms like Twitter, StockTwits, or financial news.
Include post comments for deeper sentiment insights.
Advanced Models:

Try time-series models (LSTM, ARIMA) for trend prediction.
Explore transformer models like BERT for nuanced sentiment understanding.
### Real-Time Analysis:

Build pipelines for live sentiment analysis and stock trend prediction.

### Step 10: Deployment
Package the project in a GitHub repository with a structured README.md.
Optionally, deploy a dashboard using tools like Flask or Streamlit for interactive sentiment and trend visualization.


# Thank You 



