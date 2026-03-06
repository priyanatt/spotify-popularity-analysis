# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)
# # Project Overview

This project analyses Spotify track data to investigate how different audio characteristics influence song popularity. The dataset includes characteristics such as danceability, energy, tempo, and explicit content.

The project uses Python to clean, analyse, and visualise the data in order to explore patterns between audio features and popularity. The results are presented through visualisations and an interactive dashboard that allows users to explore the dataset and key insights.

Dataset: **Spotify Tracks Dataset from Kaggle**

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

The dataset includes features such as danceability, energy, tempo, and whether a track is explicit. The aim is to analyse these features and see if any patterns appear in more popular songs.

## Stakeholder Needs

information pending

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

### Hypothesis 1: Audio Features and Popularity

H₀: Energy and danceability have no relationship with song popularity.  
H₁: Tracks with higher energy and danceability tend to have higher popularity scores.

Test:

Results:
- Test Statistic: t =
- P-Value:
- Effect Size:
- Decision:

Business Implication:


### Hypothesis 2: Acousticness and Popularity

H₀: Songs with high acousticness and low acousticness have equal average popularity.
H₁: Songs with high acousticness have different average popularity compared to songs with low acousticness.


Test:

Results:
- Test Statistic: t =
- P-Value:
- Effect Size:
- Decision:

Business Implication:


### Hypothesis 3: Tempo and Popular Songs

H₀: Tempo has no relationship with song popularity.  
H₁: Songs with moderate tempo (approximately 90–130 BPM) tend to have higher popularity than songs with very slow or very fast tempos.

Test:

Results:
- Test Statistic: t =
- P-Value:
- Effect Size:
- Decision:

Business Implication:


# Dataset Description

**Source:** Kaggle – Spotify Tracks Dataset

**Records:** information pending

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

information pending


# Project Structure

information pending


# Project Objectives

The aim of this project is to:

- Implement a basic ETL (Extract, Transform, Load) pipeline using Python
- Analyse Spotify track data to explore factors that may influence song popularity
- Investigate relationships between audio features such as danceability, energy, and tempo
- Compare the popularity of explicit and non-explicit tracks
- Create data visualisations to show patterns and trends in the dataset
- Build an interactive Tableau dashboard to allow users to explore the data


# Methodology

information pending


# Key Findings

information pending


# Results & Performance

information pending


# Learning Journey & Reflections

information pending


# Future Improvements

information pending