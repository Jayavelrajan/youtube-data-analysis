# YouTube Data Analysis Project

# Overview
This project involves the analysis of YouTube data, focusing on various aspects such as sentiment analysis, word cloud analysis, emoji analysis, and more. The dataset used for this analysis contains information about trending videos on YouTube and is in the project directory.

# Table of Contents

- Installation
- Analysis Steps
  - Sentiment Analysis
  - Wordcloud Analysis
  - Emoji Analysis
  - Exporting Data
  - Most Liked Category
  - Audience Engagement
  - Trending Videos by Channel
  - Relationship between Views & Likes
  - Punctuation Analysis
- Usage
- License

  # Installation

  To run this project, you need the following dependencies installed:
- pandas
- seaborn
- numpy
- matplotlib
- emoji
- plotly

  # Analysis Steps
  
  ### Sentiment Analysis
  Utilized TextBlob to perform sentiment analysis on comments, categorizing them as positive (polarity 1) or negative (polarity -1)
  
  ```bash
  !pip install textblob
  from textblob import TextBlob
  ```
  
  ### Wordcloud Analysis
  Generated word clouds to visualize the most frequently occurring words in the dataset. This provides a visually appealing representation of the most frequently occurring words in a dataset and understanding the audience mindset

  ### Positive Comments

  ### Negative Comments
  

  ### Emoji Analysis
  Identified and analyzed the usage of emojis in comments to gain insights into audience reactions. Also, it provides insights into audience emotions, enhancing understanding of sentiment and engagement in content and 
  how frequently and common the emojis are used.
  
  ### Exporting Data
  Exported the cleaned data into CSV, JSON, and a database for further use.
  #### To CSV:
  ```bash
  full_df[0:1000].to_csv(r'youtube_sample.csv' , index=False)
  ```
  #### To JSON:
  ```bash
  full_df[0:1000].to_json(r'youtube_sample.json')
  ```
  #### To Sqlite DB:
  ```bash
  from sqlalchemy import create_engine
  engine = create_engine(r'sqlite:///youtube_sample.sqlite')
  full_df.to_sql('Users' , con=engine , if_exists='append')
  ```

  ### Most Liked Category
  Determined the category that received the highest number of likes, providing insights into audience preferences. What category in Youtube has more engagement? and Which has more likes with it? These questions are 
  answered using this boxplot.
  
  ### Audience Engagement
  Explored the engagement metrics to understand how viewers interacted with the content and answered using this boxplot.

  ### Relationship between Views & Likes
  Analyzed the correlation between views and likes to uncover patterns in audience behavior is visualised in this regression plot and Heatmap
  
  ### Trending Videos by Channel
  Identified channels with the largest number of trending videos, revealing trends in content creators' success, using this BarGraph
  
  ### Punctuation Analysis
  Investigated whether the presence of punctuations in titles and tags had any correlation with views, likes, dislikes, and comments using these boxplot

  - Relation between Punctutations and Views
   
  - Relation between Punctutations and likes

  # Usage

  Clone the repository:

  ```bash
  git clone https://github.com/your-username/your-repository.git
  cd your-repository
  ```
  Latest Version of Anaconda software environment is required!


 # License
 This project is licensed under the MIT License.



























  
  
