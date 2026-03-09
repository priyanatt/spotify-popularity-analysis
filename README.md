# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)
# Project Overview

This project analyses Spotify track data to investigate how different audio characteristics influence song popularity. The dataset includes characteristics such as danceability, energy, tempo, and explicit content.

Python is used to clean, analyse, and visualise the data in order to explore patterns between audio features and popularity. The results are presented through visualisations and an interactive dashboard that allows users to explore the dataset and key insights.

Spotify Tracks Dataset from Kaggle: https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset 

Key Features:

- ETL pipeline for extracting, cleaning, and preparing the dataset using Python
- Exploratory Data Analysis (EDA) to identify patterns in song popularity and audio features
- Statistical analysis to examine relationships between variables such as danceability, energy, and popularity
- Machine learning model implemented using Scikit-learn
- Interactive dashboard created using Tableau for data exploration
- Data visualisations including scatter plots, histograms, bar charts, and correlation analysis


# Business Requirements

## Context

Music streaming platforms collect a large amount of data about songs and their audio features. This project uses Spotify track data to explore how different features relate to song popularity.

The dataset includes features such as danceability, energy, tempo, and whether a track is explicit. The aim is to analyse these features and identify patterns that may be associated with more popular songs.

## Stakeholder Needs

Music platforms, analysts, and artists may be interested in understanding how audio characteristics relate to song popularity. Insights from this analysis may help identify trends in song features that appear more frequently among popular tracks.

## Business Requirements

### BR1: Audio Features and Popularity

Analyse which audio features are most related to song popularity.

**Success Criteria:**

Visualisations and analysis showing the relationship between popularity and features such as danceability and energy.

### BR2: Acousticness and Song Popularity

Analyse whether songs with high acousticness have different popularity levels than songs with low acousticness.

**Success Criteria:**

Visualisations and analysis showing whether songs with higher acousticness levels differ in popularity compared to less acoustic songs.

### BR3: Tempo and Popular Songs

Explore what tempo ranges are common among popular songs.

**Success Criteria:**

Visualisations showing how tempo is distributed and how it relates to song popularity.


# Project Hypothesis & Validation

### Hypothesis 1 – Energy and Song Popularity

H₀: Average song popularity is equal across low, medium, and high energy songs.  
H₁: At least one energy group has a different average song popularity.

Test: One-way ANOVA.

Results:
- Test Statistic: F = 330.86  
- P-Value: < 0.001  
- Decision: Reject the null hypothesis

Business Implication:

Energy levels are associated with differences in song popularity, suggesting that energy may play a role in how songs perform on streaming platforms.


### Hypothesis 2 – Acousticness and Song Popularity

H₀: Songs with high acousticness and low acousticness have equal average popularity.  
H₁: Songs with high acousticness have different average popularity compared to songs with low acousticness.

Test: Mann-Whitney U Test.

Results:
- P-Value: < 0.001  
- Decision: Reject the null hypothesis

Business Implication:

Songs with different acousticness levels show statistically significant differences in popularity, suggesting that acoustic characteristics may influence listener engagement.


### Hypothesis 3 – Tempo and Popular Songs

H₀: Tempo range and song popularity category are independent.  
H₁: Tempo range and song popularity category are associated.

Test: Chi-Squared Test.

Results:
- Test Statistic: χ² = 179.83  
- P-Value: < 0.001  
- Decision: Reject the null hypothesis

Business Implication:

Certain tempo ranges appear more frequently among popular songs, indicating that tempo may influence listening preferences.


# Dataset Description

**Source:** Kaggle – Spotify Tracks Dataset  
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset 

**Records:** 114,000 songs  

The dataset contains information about Spotify tracks along with various audio features that describe the characteristics of each song. These features are generated using Spotify’s audio analysis system and help describe different aspects of a track such as rhythm, intensity, and mood.

## Features

track_id: Unique identifier for each track  

artists: Name of the artist(s) who performed the track  

album_name: Name of the album the track belongs to  

track_name: Name of the song  

popularity: Popularity score of the track on Spotify  

duration_ms: Length of the track in milliseconds  

explicit: Indicates whether the track contains explicit content  

danceability: Measure of how suitable a track is for dancing  

energy: Measure of the intensity and activity level of the track  

key: The musical key the track is played in  

loudness: Overall loudness of the track in decibels  

mode: Indicates the modality of the track (major or minor)  

speechiness: Measure of spoken words within the track  

acousticness: Confidence measure of whether the track is acoustic  

instrumentalness: Measure of how likely a track contains no vocals  

liveness: Probability that the track was performed live  

valence: Measure of the musical positivity conveyed by the track  

tempo: The estimated tempo of the track in beats per minute (BPM)  

time_signature: Number of beats in each bar of the track  

track_genre: Genre classification of the track  


# Technologies Used

Python  
Pandas  
NumPy  
Matplotlib  
Seaborn  
SciPy  
Scikit-learn  
Jupyter Notebook  
Tableau Public  
Git & GitHub  


# Project Structure
```
spotify-popularity-analysis
│
├── Data
│   ├── raw
│   └── clean
│
├── jupyter_notebooks
│   ├── Data Preparation & Exploration.ipynb
│   └── Statistical Analysis & Modelling.ipynb
│
├── README.md
└── requirements.txt
```

# Project Objectives

The aim of this project is to:

- Implement an ETL pipeline using Python
- Analyse Spotify track data to explore factors influencing song popularity
- Investigate relationships between audio features such as danceability, energy and tempo
- Perform statistical hypothesis testing to evaluate relationships between variables
- Build a simple machine learning model to predict song popularity
- Create visualisations and an interactive dashboard to explore insights


# Methodology

The project follows a structured data analytics workflow:

1. Data extraction and cleaning using Python
2. Exploratory Data Analysis (EDA) to understand dataset patterns
3. Statistical hypothesis testing to evaluate relationships between variables
4. Machine learning modelling using Linear Regression
5. Data visualisation and dashboard creation using Tableau


# Key Findings

The analysis found that several audio features show statistically significant relationships with song popularity.

Energy levels, acousticness and tempo ranges were all associated with differences in popularity based on the statistical tests performed.

However, correlation analysis shows that no single audio feature strongly predicts popularity, suggesting that multiple factors influence song success.


# Results & Performance

A Linear Regression model was trained to predict song popularity using Spotify audio features.

Model performance:

- Mean Squared Error (MSE): 483.40
- R² Score: 0.02

The low R² score indicates that audio features alone explain only a small portion of the variation in popularity. External factors such as artist popularity, marketing exposure and playlist placement likely play an important role.


# Interactive Tableau Dashboard

An interactive Tableau dashboard was created to present the key insights from the analysis and allow users to explore the Spotify dataset visually.

The dashboard includes visualisations such as popularity distributions, scatter plots comparing audio features with popularity, and tempo distributions across songs. These visualisations help illustrate patterns identified during the exploratory data analysis and statistical testing.

Interactive filters allow users to explore how different song characteristics relate to popularity and examine patterns across the dataset.

Tableau Dashboard Link:  
https://public.tableau.com/app/profile/priya.kaur.natt/viz/Spotifyanalysis_17729117990390/SpotifyAudioFeaturesandSongPopularityAnalysis


# Learning Journey & Reflections

This project provided practical experience applying core data analytics techniques including data cleaning, exploratory data analysis, statistical testing and machine learning modelling.

Working with a real-world dataset helped develop skills in interpreting statistical results and translating findings into meaningful insights.


# Future Improvements

Future work could include:

- testing additional machine learning models
- including additional variables such as artist popularity or playlist data
- expanding the analysis with larger or more recent datasets
- enhancing the Tableau dashboard with additional interactive visualisations