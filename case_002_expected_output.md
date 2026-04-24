# Expected Output for Case 2

## Extracted Flow

```json
{
  "steps": [
    {
      "id": "data_collection",
      "description": "Collect tweets using climate-related keywords",
      "input": "Twitter API",
      "output": "Raw tweet dataset (500,000 posts)",
      "methods": ["API queries", "Keywords: climate change, global warming, carbon emissions"]
    },
    {
      "id": "language_filtering",
      "description": "Filter for English posts only",
      "input": "Raw tweets",
      "output": "English-only dataset",
      "methods": ["Language detection"]
    },
    {
      "id": "retweet_removal",
      "description": "Remove retweets",
      "input": "English tweets",
      "output": "Original posts only",
      "methods": ["Retweet filtering"]
    },
    {
      "id": "text_cleaning",
      "description": "Clean text content",
      "input": "Original posts",
      "output": "Cleaned text",
      "methods": ["URL removal", "Mention removal", "Special character removal"]
    },
    {
      "id": "tokenization",
      "description": "Tokenize and remove stop words",
      "input": "Cleaned text",
      "output": "Tokenized text",
      "methods": ["NLTK tokenization", "Stop word removal"]
    },
    {
      "id": "sentiment_analysis",
      "description": "Score sentiment using VADER",
      "input": "Tokenized text",
      "output": "Sentiment scores",
      "methods": ["VADER sentiment analyzer"]
    },
    {
      "id": "temporal_aggregation",
      "description": "Aggregate by week and topic",
      "input": "Sentiment scores",
      "output": "Weekly sentiment aggregates",
      "methods": ["Time-based grouping", "Topic categorization"]
    },
    {
      "id": "trend_analysis",
      "description": "Analyze sentiment trends over time",
      "input": "Weekly aggregates",
      "output": "Trend analysis results",
      "methods": ["Time series analysis"]
    }
  ]
}
```

## Validation Issues

- Sampling bias in keyword-based collection
- No validation of sentiment analysis accuracy
- Stop word list not specified
- Topic categorization method unclear
- No assessment of data representativeness

## Grade: C+