# Creating the markdown content for GitHub documentation
# Melody Metrics - Song Popularity Prediction

## Project Description

The **Melody Metrics** project aims to analyze the factors influencing the popularity of songs using various musical attributes. By examining a structured dataset containing detailed information about song characteristics such as genre, tempo, lyrical content, and song length, the goal is to predict the popularity of songs and uncover patterns that drive musical success. This project serves as a foundation for applying machine learning techniques to predict song popularity, providing insights into how different song features impact success across various genres.

## Dataset Overview

The dataset consists of two files:

- **train.csv**: Contains 8,000 rows with 7 columns, including the target variable **Popularity**.
- **test.csv**: Contains 2,000 rows with 6 columns, excluding the **Popularity** column (which needs to be predicted).

### Features in the Dataset

1. **SongLength** (Seconds): Duration of the song. Longer songs may have different listener engagement levels compared to shorter ones.
2. **NumInstruments**: Number of instruments used in the song, which indicates its complexity.
3. **Genre**: The genre of the song (e.g., Classical, Jazz, Pop, Country, Rap, Rock).
4. **Tempo** (BPM): Beats per minute of the song, influencing its energy and pace.
5. **LyricalContent**: A metric representing the complexity or positivity of the lyrics.
6. **ReleasedYear**: The year the song was released, capturing temporal trends in music preferences.
7. **Popularity** (Target Variable - **train.csv**): A score indicating the song's popularity, which will be predicted for the test set.

## Objective

The primary goal is to predict the **Popularity** of songs in the **test.csv** file using various musical attributes present in the dataset. By analyzing correlations and exploring patterns, we aim to gain insights into the features that contribute most to a song's success.

## Statistical Summary

- **SongLength**: The mean song length is around 273 seconds for both the training and test datasets, with consistent distributions.
- **NumInstruments**: On average, songs in both datasets use about 4.94 to 5.05 instruments, with a range from 1 to 9.
- **Tempo**: The mean tempo is around 129 BPM for the training set and 131 BPM for the test set, suggesting minimal variance between datasets.
- **LyricalContent**: The average value is 0.5, with values ranging from near 0 to 1, indicating varied complexity or positivity of lyrics.
- **ReleasedYear**: The dataset spans from 1980 to 2022, with median release years around 2001-2002.
- **Popularity**: The popularity scores range from 0 to 100, with an average score of 49 and significant variation in popularity.

## Genre-Wise Analysis

The analysis shows the following trends for different genres:

- **Pop**: Tends to have the highest popularity, with a richer instrumentation and average tempo.
- **Rock**: Generally has lower popularity and slightly lower lyrical content.
- **Classical and Jazz**: These genres have slightly longer average song lengths and similar tempos (around 129 BPM).
- **Country**: Shows slightly higher lyrical content, with a good average popularity score.

## Correlation Insights

### Training Data

- **SongLength**: Weak positive correlation with popularity (0.0997).
- **NumInstruments**: Weak positive correlation with popularity (0.0599).
- **Tempo**: Moderate positive correlation with popularity (0.4723), suggesting tempo has a stronger influence on success.
- **LyricalContent**: Strong positive correlation with popularity (0.8453), indicating that higher lyrical content tends to correlate with higher popularity.
- **ReleasedYear**: Weak negative correlation with popularity (-0.0644), suggesting a minor inverse trend with more recent releases.

### Test Data

The correlations between features in the test set align closely with those in the training set, suggesting consistent feature behavior.

## Key Insights

- **LyricalContent** is the strongest predictor of popularity, indicating that more complex or positive lyrics are associated with higher popularity.
- **Tempo** has a moderate impact on popularity, showing that faster-paced songs tend to perform better.
- **SongLength** and **NumInstruments** have minimal influence on popularity, but they still contribute in subtle ways.
- **Genre** plays a role in shaping popularity, with Pop songs showing the highest average popularity and Rock songs having the lowest.

## Project Goals

1. Perform exploratory data analysis (EDA) to uncover additional patterns.
2. Build machine learning models to predict song popularity based on the features.
3. Optimize the models to achieve high predictive accuracy.
