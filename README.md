# predict_articles_shares
Analysing Kaggle dataset of online articles and predicting number of shares

In a  hypothetical situation, that can be useful for an online news company to know how to spend budget to promote articles. This data analysis project may help to predict how many shares an article would have.

Kaggle dataset: https://www.kaggle.com/datasets/srikaranelakurthy/online-news-popularity.

Its size 39644 rows, 61 columns.

Data preparation, Exploratory Data Analysis, Feature Engineering and Random Forest regression model with hypertuning to predict number of articles' shares. Columns were MinMax Scaled for the model.

Best MSE: 0.00009

Best MAE: 0.004

About dataset:
* url: URL of the article.(String)
* timedelta: Days between the article publication and the dataset acquisition.(float)
* n_tokens_title: Number of words in the title (Integer)
* n_tokens_content: Number of words in the content((Integer)
* n_unique_tokens: Rate of unique words in the content (Integer)
* n_non_stop_words: Rate of non-stop words in the content (Integer)
* n_non_stop_unique_tokens: Rate of unique non-stop words in the content(Integer)
* num_hrefs: Number of links (Integer)
* num_self_hrefs: Number of links to other articles published by Mashable (Integer)
* num_imgs: Number of images (float)
* num_videos: Number of videos (float)
* average_token_length: Average length of the words in the content (float)
* num_keywords: Number of keywords in the metadata (float)
* data_channel_is_lifestyle: Is data channel 'Lifestyle'? (Binary)
* data_channel_is_entertainment: Is data channel 'Entertainment'? (Binary)
* data_channel_is_bus: Is data channel 'Business'? (Binary)
* data_channel_is_socmed: Is data channel 'Social Media'? (Binary)
* data_channel_is_tech: Is data channel 'Tech'? (Binary)
* data_channel_is_world: Is data channel 'World'? (Binary)
* kw_min_min: Worst keyword (min. shares) (float)
* kw_max_min: Worst keyword (max. shares) (float)
* kw_avg_min: Worst keyword (avg. shares) (float)
* kw_min_max: Best keyword (min. shares) (float)
* kw_max_max: Best keyword (max. shares) (float)
* kw_avg_max: Best keyword (avg. shares) (float)
* kw_min_avg: Avg. keyword (min. shares) (float)
* kw_max_avg: Avg. keyword (max. shares) (float)
* kw_avg_avg: Avg. keyword (avg. shares) (float)
* self_reference_min_shares: Min. shares of referenced articles in Mashable (float)
* self_reference_max_shares: Max. shares of referenced articles in Mashable (float)
* self_reference_avg_sharess: Avg. shares of referenced articles in Mashable (float)
* weekday_is_monday: Was the article published on a Monday? (Binary)
* weekday_is_tuesday: Was the article published on a Tuesday? (Binary)
* weekday_is_wednesday: Was the article published on a Wednesday? (Binary)
* weekday_is_thursday: Was the article published on a Thursday? (Binary)
* weekday_is_friday: Was the article published on a Friday? (Binary)
* weekday_is_saturday: Was the article published on a Saturday? (Binary)
* weekday_is_sunday: Was the article published on a Sunday? (Binary)
* is_weekend: Was the article published on the weekend? (Binary)
* LDA_00: Closeness to LDA topic 0 (float)
* LDA_01: Closeness to LDA topic 1 (float)
* LDA_02: Closeness to LDA topic 2 (float)
* LDA_03: Closeness to LDA topic 3 (float)
* LDA_04: Closeness to LDA topic 4 (float)
* global_subjectivity: Text subjectivity (float)
* global_sentiment_polarity: Text sentiment polarity (float)
* global_rate_positive_words: Rate of positive words in the content (float)
* global_rate_negative_words: Rate of negative words in the content (float)
* rate_positive_words: Rate of positive words among non-neutral tokens (float)
* rate_negative_words: Rate of negative words among non-neutral tokens (float)
* avg_positive_polarity: Avg. polarity of positive words (float)
* min_positive_polarity: Min. polarity of positive words (float)
* max_positive_polarity: Max. polarity of positive words (float)
* avg_negative_polarity: Avg. polarity of negative words (float)
* min_negative_polarity: Min. polarity of negative words (float)
* max_negative_polarity: Max. polarity of negative words (float)
* title_subjectivity: Title subjectivity (float)
* title_sentiment_polarity: Title polarity (float)
* abs_title_subjectivity: Absolute subjectivity level (float)
* abs_title_sentiment_polarity: Absolute polarity level (float)
* shares: Number of shares (target) (Integer)
