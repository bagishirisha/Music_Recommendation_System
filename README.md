# DA 204o Data Science in Practice Project

## Team members :
1. ***Vineet Kumar Tripathi***
2. ***Bagi Shirisha***
3. ***Priyabrata Samantaray***
4. ***Gayatri Yendamury***

## Project Title : **MUSIC RECOMMENDATION SYSTEM**

This repo will contain Python implementation of music recommendation system using Spotify dataset.<br/>

## Table of Contents

* [Problem Statement](#problem-statement)
* [Objectives](#objectives)
* [Dataset Overview and Column Descriptions](#dataset-overview-and-column-descriptions)
* [Setup](#setup)
* [Notebooks](#notebooks)
* [Obtained results](#obtained-results)
* [Future scope](#future-scope)

## Problem Statement
- Music streaming platforms offer millions of tracks, but users often struggle to find songs that match their choice. Existing recommendation systems are limited, often suggesting irrelevant content, leading to user disappointment and disengagement.
- A smarter, data-driven recommendation system is needed to enhance personalization and improve user experience by offering more accurate music suggestions.

## Objectives
- Build a content-based music recommendation system using features from the dataset.
- Explore and understand the key audio features that influence song similarity.
- Develop visualizations and perform Exploratory Data Analysis (EDA) to identify trends and patterns within the music data.

## Dataset Overview and Column Descriptions

### **Dataset used** : 
Kaggle spotify dataset : https://www.kaggle.com/datasets/vatsalmavani/spotify-dataset/data

For this project, we have used below datasets:\
1. Raw dataset: *data.csv , data_by_genre.csv* -Raw dataset from Kaggle
2. Cleaned dataset: *data_cleaned.csv , genre_data_cleaned.csv* - Generated after running 02_data_preprocessing.ipynb.

### **Dataset columns description** : 

- **valence**: Indicates the musical positiveness of a track, where high values represent happier and more positive sounds, and low values indicate sadder or negative tones.
- **year**: The release year of the track.It is useful for analyzing trends over time.
- **acousticness**: Measures how acoustic a track sounds. High values suggest the track is more acoustic, while low values imply more electronic or synthetic sounds.
- **artists**: Names of the artists involved in the track.It helps to group songs by same artist.
- **danceability**: Reflects how suitable a track is for dancing. High values denote easier dance rhythms, while low values indicate more complex or irregular beats.
- **duration_ms**: Duration of the track in milliseconds.The longer durations values are associated with extended compositions or live recordings.
- **energy**: It Represents the intensity and activity level of a track. Higher values suggest energetic tracks, while lower values indicate calm or mellow tracks.
- **explicit**: Indicates if the track has explicit lyrics (1 = yes, 0 = no).
- **id**: Unique Spotify ID for the track.
- **instrumentalness**: Predicts the likelihood of a track being instrumental. High values (close to 1.0) suggest little or no vocals, while low values indicate vocal presence.
- **key**: The Musical key of the track, represented by numbers (0 to 11).
- **liveness**: It Estimates the presence of a live audience. High values suggest live performance , while low values indicate studio recordings.
- **loudness**: Overall loudness of the track in decibels. Higher values mean louder tracks, while lower values are quieter.
- **mode**: Indicates modality (1 = major, 0 = minor); major often sounds happier, while minor is generally more somber.
- **name**: The Title of the track.
- **popularity**: Popularity score on Spotify (0 to 100). High values indicate popular tracks, while low values indicate less popular tracks.
- **release_date**: The Date the track was released.It helps to analyze time-based trends.
- **speechiness**: Measures the presence of spoken words in the track. High values indicate more speech-like content (e.g., podcasts), while low values suggest minimal or no speech.
- **tempo**: Tempo of the track in beats per minute (BPM). High values indicate faster tracks, while low values indicate slower songs.

This dataset provides a range of audio features that describe the musical characteristics and popularity metrics for each track, essential for building a recommendation system.

## Setup
Please install all the needed libraries as mentioned in [requirements.txt](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/requirements.txt)

## Notebooks
The complete project is divided into different data science workflow steps as mentioned below.
The input , output , and description is provided for all the notebooks.
Please make sure the notebooks are run sequentially .

| **Notebook**         | **Input artifacts**      | **Output artifacts**          | **Discription**     |
| ------------------- | ------------------ | ------------------ | ------------------ |
| [01_data_collection](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/01_data_collection.ipynb)   | data.csv , data_by_genres.csv  | None | Load the raw dataset and check overview , missing values etc..  |
| [02_data_preprocessing](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/02_data_preprocessing.ipynb)   | data.csv , data_by_genres.csv  | data_cleaned.csv,genre_data_cleaned.csv | Perform descriptive statistics analysis , outlier handling and feature engineering.After this the cleaned dataset is stored.   |
| [03_data_exploration](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/03_data_Exploration.ipynb)   | data_cleaned.csv,genre_data_cleaned.csv  | None | Check key observations based on popularity, observe distributions of various audio feature.Perform univariate , bivariate and trend analysis  |
| [04_model_selection](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/04_model_selection.ipynb)   | data_cleaned.csv,genre_data_cleaned.csv  | None | Performs clustering analysis on cleaned datasets (data_cleaned.csv,genre_data_cleaned.csv) using methods like KMeans, KMedoids, Agglomerative Clustering, DBSCAN, and Gaussian Mixture. It includes steps for optimal cluster detection, clustering processes, result visualization, and a conclusion on model selection.  |
| [05_hyperparameter_tuning](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/05_hyperparameter_tuning.ipynb)   | data_cleaned.csv,genre_data_cleaned.csv  | None | Performs hyperparameter tuning for KMeans clustering and dimensionality reduction techniques like t-SNE, and PCA. |
| [06_model_training](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/06_model_training.ipynb)   | data_cleaned.csv,genre_data_cleaned.csv  | data_cleaned_clustering.csv , genre_data_cleaned_clustering.csv | Using K-Means clustering we analyze and group music genres and songs. It prepares clustering pipelines, applies t-SNE and PCA for dimensionality reduction, visualizes the results.Finally we store the pre-processed dataset as data_cleaned_clustering.csv , genre_data_cleaned_clustering.csv.|
| [07_model_deployment](https://github.com/bagishirisha/Music_Recommendation_System/blob/main/Code/07_model_deployment.ipynb)   | data_cleaned_clustering.csv , genre_data_cleaned_clustering.csv | None | It deploys the music recommendation system based on content-based filtering, and discusses the future scope |


## Future Scope
**Real Time Processing**
- Build user profiles, integrate real-time feedback (likes/dislikes) and apply collaborative filtering for more accurate, personalized suggestions.

**Advanced Models**
- Implement Hybrid models combining collaborative, content-based and context-aware filtering for better recommendations.

**Enhanced Features**
- Incorporate audio features, sentiment analysis of lyrics and temporal trends for better recommendations.
