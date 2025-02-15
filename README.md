# Song Recommendation System

This repository contains code for building an artist recommendation system based on Spotify's song attributes. The recommendation system leverages clustering algorithms and Spotipy, a Python client for the Spotify Web API, to provide personalized song recommendations tailored to individual user preferences.

## Data and Analysis
The analysis begins by exploring the correlation and covariance between various song attributes such as valence, acousticness, danceability, energy, instrumentalness, and more. Visualizations are created to illustrate how these attributes correlate with the popularity of songs over time. Additionally, clustering techniques are applied to group songs based on their genre and attributes.

## Feature Engineering and Visualization
The analysis includes feature engineering steps such as extracting decades from the 'year' attribute to visualize the distribution of songs by decade. Line plots are generated to visualize the trends of sound features over time, offering insights into the evolution of music characteristics throughout different eras.

## Clustering and Recommendation
The repository implements clustering algorithms, including KMeans and t-SNE, to cluster songs based on their attributes. This clustering facilitates the recommendation of songs that are similar in terms of their musical characteristics. Recommendations are generated by calculating the cosine distance between the mean feature vector of input songs and songs in the Spotify dataset.

## Implementation
The code provides functions for processing input data, calculating feature vectors, performing clustering, and recommending songs. Spotipy is utilized to retrieve song attributes from the Spotify API. The recommendation system takes a list of songs as input and returns a set of recommended songs based on the similarity of their attributes to those of the input songs.

Usage
To use the artist recommendation system:

Install Spotipy using pip install spotipy.
Create an application on the Spotify Developer's page to obtain a Client ID and secret key for authentication and access to the API.
Load Spotify API credentials from a configuration file (config.json).
Use the provided functions to process input data, calculate feature vectors, and recommend songs based on user preferences.
