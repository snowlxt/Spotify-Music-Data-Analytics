# Spotify Music Popularity Classification

![image](https://user-images.githubusercontent.com/62194058/136700862-5956aef5-8961-4ff8-8363-4418c727716c.png)

## Overview
According to previous research, the popularity of music can be explained by the inherent features of the music. Spotify Web API makes this idea testable by providing the information including audio features of songs published. Collecting data via Spotify Web API, we are allowed to collect information about songs and conduct analysis. In this analysis report, we first show how we connected to Spotify API and gathered the data. Then we described and gave some insights based on data visualization. Finally, we established classification models to enhance our conclusions. According to the analysis, we found that artists’ followers have an overwhelming influence on the popularity of songs. Putting artists’ followers aside, a song’s loudness, speechiness and tempo have the greatest effect among all audio features.

## Contents
* Data Collecting & Feature Engioneering
* EDA
* Modelling

## Data Collecting & Feature Engioneering
**Data Source** - Spotify API, Billboard Week 200 Albums
**Data collecting steps** - 
<img width="1014" alt="截屏2021-10-11 上午10 21 03" src="https://user-images.githubusercontent.com/62194058/136806354-d7b041f6-5027-4638-aebd-0736a147cf7a.png">
**Features for next step** - 
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

**Target variable** - 'popularity'
Referring to the distribution of the attribute ‘popularity’, there are few songs that report a popularity of over 60, which is only 3 thousand out of over 20 thousand tracks. Therefore, I cut the sample into two bins: tracks with popularity over 60 are classified as popular songs and others as unpopular songs. I labeled the popular songs as 1 and unpopular ones as 0 under the new binary popularity attribute. 

## Sampling
As with many other classification models, I run into a class imbalance problem. Since there are so many more instances of class 0 than of class 1, the models I train will tend to classify most songs as class 1. Even though this results in an extremely high accuracy, the results are ultimately impractical because most, if not all, of class 1’s are categorized incorrectly. Therefore, I use two methods: 
* Oversampling
* SMOTE (Synthetic Minority Over-sampling Technique)

## Models
* **K-Nearest Neighbors**
* **Naive Bayes**
