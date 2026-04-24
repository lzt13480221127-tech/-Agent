# Case Study 2: Social Media Sentiment Analysis

## Article Excerpt

We analyzed sentiment in social media posts related to climate change. Data was collected from Twitter API using keywords "climate change", "global warming", and "carbon emissions" over a 6-month period, resulting in 500,000 posts.

The processing pipeline included:
1. Filtering out non-English posts and retweets
2. Removing URLs, mentions, and special characters
3. Tokenization and stop-word removal
4. Sentiment scoring using VADER
5. Aggregation by week and topic
6. Time series analysis of sentiment trends

## Key Processing Steps

- Data source: Twitter API
- Preprocessing: Language filtering, text cleaning
- Analysis: Sentiment analysis, temporal aggregation
- Methods: VADER sentiment analyzer, time series modeling