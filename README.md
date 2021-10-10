# Spotify Music Popularity Classification

![image](https://user-images.githubusercontent.com/62194058/136700862-5956aef5-8961-4ff8-8363-4418c727716c.png)

## Overview
According to previous research, the popularity of music can be explained by the inherent features of the music. Spotify Web API makes this idea testable by providing the information including audio features of songs published. Collecting data via Spotify Web API, we are allowed to collect information about songs and conduct analysis. In this analysis report, we first show how we connected to Spotify API and gathered the data. Then we described and gave some insights based on data visualization. Finally, we established classification models to enhance our conclusions. According to the analysis, we found that artists’ followers have an overwhelming influence on the popularity of songs. Putting artists’ followers aside, a song’s loudness, speechiness and tempo have the greatest effect among all audio features.

## Contents
* Data Collecting & Feature Engioneering
* EDA
* Modelling

## Data Collecting & Feature Engioneering
### Data Source - Spotify API
Spotify Web API offers several sources for developers and analysts to use the data from Spotify music platform from different endpoints.
In this project, I aimed at figuring out the contribution of each of the features to popularity. Fortunately, Spotify published both the popularity and the features of each song. We were able to acquire information of the albums by searching the endpoints . However, we encountered an obstacle: Spotify only returned 50 results per search, but I have far more than 50 instances as our sample. We figured out one way to resolve this in order to obtain a list for indexing.
