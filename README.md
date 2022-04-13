# Dissecting-Spotify-Valence-Metric
In this Jupyter Notebook i attempt to examine **"Valence"**, a metric that Spotify uses to measure the "happiness" or "sadness" of every song.

At first, i attempt to find which song features are influencing "Valence" and which are not. A Generalized Linear Model will be used to do so (Beta Regression).</br>
Then, i use various machine learning algorithms in an attempt to predict the "Valence" metric of each new song.  </br>
</br>
The data i will use come from 2 differnet sources:</br>
1) "tracks.csv" (from: [Spotify Songs with Audio Features (from Kaggle)](https://www.kaggle.com/lehaknarnauli/spotify-datasets)) which contains aproximately 586,000 songs and their audio features</br>
2) "spotify_ids.txt" (which contains approximately 1160 song id's). By connecting to Spotify's API, i will iteratively get all these songs ids' audio features,</br>
    and use this dataset for out-of sample predictions.</br>
</br>
For predictions, i will use the following methods:</br>
1. Decision Tree </br> 
2. XGBoost </br>
3. Beta Regression </br>
4. K-Nearest Neighbors. </br>
</br>
At last, a final model will be chosen depending on the Mean Average Error of each Machine Learning Algorithm.
