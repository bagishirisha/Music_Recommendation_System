# DA 204o Data Science in Practice Project

## Team members :
1. ***Vineet Kumar Tripathi***
2. ***Bagi Shirisha***
3. ***Priyabrata Samantaray***
4. ***Gayatri Yendamury***

## Project Title : 
## **MUSIC RECOMMENDATION SYSTEM**

## **Problem Statement:**
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
*data.csv , data_by_genre.csv*

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
