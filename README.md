# PRODIGY_DS_04

# Twitter Sentiment Analysis

## Overview

This project analyzes Twitter data to explore sentiment associated with various entities mentioned in tweets. The primary goal is to visualize the distribution of sentiments and entities, providing insights into how different entities are perceived in terms of sentiment.

## Dataset

The dataset consists of two CSV files:

- **twitter_training.csv**: Contains training data with tweets labeled by sentiment.
- **twitter_validation.csv**: Contains validation data with tweets labeled by sentiment.

### Columns in the Dataset

- **TweetID**: Unique identifier for each tweet.
- **Entity**: The entity being referenced in the tweet.
- **Sentiment**: The sentiment associated with the tweet (e.g., Positive, Negative, Neutral).
- **Tweet_Content**: The actual text of the tweet.

## Data Processing

1. **Loading Data**: The training and validation datasets are loaded into separate DataFrames using Pandas.
2. **Column Naming**: The columns are renamed for consistency and clarity.
3. **Data Concatenation**: The two DataFrames are combined into a single DataFrame for analysis.
4. **Data Cleaning**:
   - **Missing Values**: Any rows with missing `Tweet_Content` values are removed.
   - **Duplicate Entries**: Duplicate rows are identified and removed.
5. **Dropping Irrelevant Columns**: The `TweetID` and `Tweet_Content` columns are dropped to focus on the `Entity` and `Sentiment`.

## Data Visualization

The following visualizations are created to better understand the data:

1. **Entity Distribution**: A pie chart visualizes the distribution of different entities within the dataset.
2. **Sentiment Distribution**: A bar chart displays the counts of various sentiments associated with the tweets.
3. **Entity vs Sentiment**: A bar chart shows the relationship between different entities and their associated sentiments using a crosstab.

## Conclusion

This analysis provides insights into how various entities are perceived on Twitter based on sentiment. The visualizations created help to identify trends and relationships in the data, facilitating further analysis or decision-making processes.

## Requirements

- Python 3.x
- Pandas
- Matplotlib
- NumPy


## Usage
Run the script to visualize the data as described above. Ensure that the CSV files are in the same directory as the script.


