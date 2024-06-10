# Enhancing Spotify's Recommendation System: Music Genre Analysis and Prediction Using Musical Features

**Authors:** Jules Saldivar and Brianna Browning
***
## Overview
The purpose of this Data Analysis project is to identify trends in musical/audio features based on genre and use these insights to develop a prediction model for genre classification. By analyzing the musical features of songs, we aim to uncover distinctive patterns that characterize different genres such as EDM, Emo, R&B/Pop, and Trap/Rap/Hiphop. These patterns will then be leveraged to create a machine learning model that can accurately predict the genre of songs. This project aims to enhance music recommendation systems by ensuring accurate genre classification, thereby improving user satisfaction through more relevant music suggestions.

## Business Problem 
Spotify’s recommendation system currently suggests music based on users' listening habits. However, the system can be further refined by accurately categorizing songs into their respective genres. Misclassification of songs can lead to less relevant recommendations, negatively impacting user experience. This project analyzes trends of musical features in order to create and improve a genre classification model that accurately identifies the genre of each song based on its audio features. The ultimate goal is to integrate this model into Spotify’s recommendation system, ensuring that users receive more precise and enjoyable music recommendations.

## Data
The first dataset for this project was sourced from Spotify's music database, comprising over 40,000 songs with detailed audio features. The genre distribution within the dataset is as follows:

- Trap/Rap/Hiphop: 20,272 songs
- EDM: 17,793 songs
- R&B/Pop: 2,560 songs
- Emo: 1,680 songs

The data includes features such as danceability, energy, loudness, speechiness, acousticness, instrumentalness, liveness, valence, tempo.

The second dataset includes genre sorted playlists from Spotify

## Methods
To identify trends in musical features and build the genre prediction model, the following steps were undertaken:

- Data Analysis: Exploratory data analysis was performed to identify trends and patterns in audio features across different genres.
- Data Preprocessing: Handling missing values, normalizing the data, transforming columns.
- Feature Engineering: Identifying and selecting the most relevant features for genre classification based on the analysis.
- Model Training: Training a logistic regression model to predict the genre of songs
- Evaluation: Assessing models using accuracy scores, confusion matrices, and classification reports.

## Results
The logistic regression model was evaluated using accuracy scores and a confusion matrix, with the following results:

Logistic Regression Model:
Accuracy: 0.77
### Confusion Matrix:
![image](https://github.com/julessaldivar/Data_Analysis_Spotify_Music_Report/assets/165840445/c34a241d-013d-46a8-a0c5-2f500b8ff386)

Interpretation of the Confusion Matrix

EDM:

- Correctly classified as EDM: 2986
- Misclassified as Emo: 44
- Misclassified as R&B/Pop: 2
- Misclassified as Trap/Rap/Hiphop: 504
  
Emo:

- Correctly classified as Emo: 83
- Misclassified as EDM: 119
- Misclassified as R&B/Pop: 20
- Misclassified as Trap/Rap/Hiphop: 119
  
R&B/Pop:

- Correctly classified as R&B/Pop: 41
- Misclassified as EDM: 23
- Misclassified as Emo: 12
- Misclassified as Trap/Rap/Hiphop: 418
  
Trap/Rap/Hiphop:

- Correctly classified as Trap/Rap/Hiphop: 3412
- Misclassified as EDM: 618
- Misclassified as Emo: 30
- Misclassified as R&B/Pop: 30

### Distribution of Genre
![image](https://github.com/julessaldivar/Data_Analysis_Spotify_Music_Report/assets/165840445/7d982f17-2aff-45f8-9cdb-45c452fe55ee)

This Distribution of Genre graph shows a heavy imbalance amongst the Genre distribution, with data falling primarily under Trap/Rap/Hiphop and EDM music, impacting the accuracy and reliability of R&B/Pop and Emo results. 

## Conclusion
The analysis revealed distinct trends in musical features across different genres, which were effectively used to build a genre prediction model. Our most influencial musical features were energy, valence, speechiness, instrumentalness, acousticness, tempo, and danceability. The logistic regression model showed a respectable accuracy and is recommended for genre classification. To further enhance the model's performance, especially for less represented genres like Emo and R&B/Pop, future steps include balancing the dataset in order to better represent these under reported genres. Integrating this improved classification model into Spotify's recommendation system can lead to more relevant and satisfying user experiences by ensuring songs are correctly categorized by genre.

## For More Information

Please review the full analysis in [the Jupyter Notebook](https://github.com/julessaldivar/Data_Analysis_Spotify_Music_Report/blob/main/Data_Analysis_Spotify_Music_Genres.ipynb) or [Spotify Music Analysis in PowerBI](https://github.com/julessaldivar/Data_Analysis_Spotify_Music_Report/blob/main/DA_Spotify_Music_Genres.pdf)


For any additional questions, please contact Jules Saldivar at <julessaldivar@gmail.com> or [LinkedIn](https://www.linkedin.com/in/jules-saldivar-7054792a8/), or Brianna Browning at <bdb97@cornell.edu> or [LinkedIn](https://www.linkedin.com/in/brianna-browning) 
