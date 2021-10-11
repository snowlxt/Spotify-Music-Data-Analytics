# Spotify Music Popularity Classification

![image](https://user-images.githubusercontent.com/62194058/136700862-5956aef5-8961-4ff8-8363-4418c727716c.png)

## Overview
According to previous research, the popularity of music can be explained by the inherent features of the music. Spotify Web API makes this idea testable by providing the information including audio features of songs published. Collecting data via Spotify Web API, we are allowed to collect information about songs and conduct analysis. In this analysis report, we first show how we connected to Spotify API and gathered the data. Then we described and gave some insights based on data visualization. Finally, we established classification models to enhance our conclusions. According to the analysis, we found that artists’ followers have an overwhelming influence on the popularity of songs. Putting artists’ followers aside, a song’s loudness, speechiness and tempo have the greatest effect among all audio features.

## Contents
* Data Collecting & Feature Engioneering
* EDA
* Modelling

## Data Collecting & Feature Engioneering
Data Source - Spotify API, Billboard Week 200 Albums
Data collecting steps - 
<img width="1014" alt="截屏2021-10-11 上午10 21 03" src="https://user-images.githubusercontent.com/62194058/136806354-d7b041f6-5027-4638-aebd-0736a147cf7a.png">
Features for next step - 
* Track_Id
* Popularity
* Followers
* Key
* Mode
* Time_Signature
* Acousticness
* Danceability
* Instrumentalness
* Liveness
* Loudness
* Speechiness
* Valence
* Tempo



