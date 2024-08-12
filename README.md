
# Twitter Sentiment Analysis

Overview

This project focuses on analyzing the sentiment of tweets using machine learning techniques. It aims to classify tweets into categories such as positive, negative, or neutral based on their content.


## Features

- Data Collection: Extracts tweets using the Twitter API.
- Data Preprocessing: Cleans and processes raw tweet data, including handling hashtags, mentions, and emoticons.
- Sentiment Analysis: Implements various machine learning models to classify tweet sentiments.
- Visualization: Displays the results with graphs and charts to highlight the sentiment distribution.


## Prerequisites


- Python 3.8 or higher
- Twitter API credentials (API key, API secret key, Access token, and Access token secret)
- Required Python libraries (listed in requirements.txt)

## Installation

1 Clone this repository:

```bash
git clone https://github.com/your-username/Twitter-Sentiment-Analysis.git
cd Twitter-Sentiment-Analysis
```

2 Install the necessary dependencies:

```bash
pip install -r requirements.txt
```

3 Set up your Twitter API credentials:

- Create a .env file in the root directory.
- Add your Twitter API credentials to the .env file as follows:

 makefile
```
TWITTER_API_KEY=your_api_key
TWITTER_API_SECRET_KEY=your_api_secret_key
TWITTER_ACCESS_TOKEN=your_access_token
TWITTER_ACCESS_TOKEN_SECRET=your_access_token_secret
```
## Usage
Run the script to collect tweets:

```bash 
python collect_tweets.py --query "keyword" --count 1000
Replace "keyword" with the topic of interest and adjust --count to the desired number of tweets.
```
Perform sentiment analysis:

```
python analyze_sentiment.py --input tweets.csv --output sentiment_results.csv
```
Visualize the results:

```bash
python visualize_results.py --input sentiment_results.csv
```

## Example
Here's an example of how to run the entire pipeline:

```bash
python collect_tweets.py --query "climate change" --count 500
python analyze_sentiment.py --input tweets.csv --output sentiment_results.csv
python visualize_results.py --input sentiment_results.csv
```

## Project Structure
- collect_tweets.py: Script to collect tweets from Twitter.
- analyze_sentiment.py: Script to analyze the sentiment of collected tweets.
- visualize_results.py: Script to visualize the sentiment analysis results.
- requirements.txt: List of Python dependencies.
- .env.example: Example file for Twitter API credentials.
- README.md: Project documentation.

## Contributing
Contributions are welcome! Please create a pull request or open an issue to discuss potential changes.


## Acknowledgements
1 Twitter API

2 TextBlob

3 Matplotlib