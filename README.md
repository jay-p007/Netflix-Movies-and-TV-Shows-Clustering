# Netflix Content Analysis and Recommendation System

## Project Overview

This project aims to analyze the Netflix dataset of movies and TV shows until 2019, obtained from the third-party search engine Flixable. The primary objective is to group the content into relevant clusters using NLP techniques to enhance user experience through a recommendation system. This system will help mitigate subscriber churn for Netflix, which currently boasts over 220 million subscribers.

Additionally, the project seeks to uncover valuable insights and trends in the streaming entertainment industry by analyzing the dataset.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Description](#data-description)
- [Project Steps](#project-steps)
  - [Handling Null Values](#handling-null-values)
  - [Managing Nested Columns](#managing-nested-columns)
  - [Binning Ratings](#binning-ratings)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Creating Clusters](#creating-clusters)
  - [Dimensionality Reduction](#dimensionality-reduction)
  - [Clustering Algorithms](#clustering-algorithms)
  - [Content-Based Recommender System](#content-based-recommender-system)
- [Conclusion](#conclusion)
- [How to Use](#how-to-use)
- [Dependencies](#dependencies)
- [Acknowledgements](#acknowledgements)

## Data Description

The dataset contains information about movies and TV shows available on Netflix until 2019. Key attributes include:

- `title`: Title of the content
- `director`: Director of the content
- `cast`: Cast of the content
- `country`: Country where the content was produced
- `date_added`: Date when the content was added to Netflix
- `release_year`: Release year of the content
- `rating`: Rating of the content
- `duration`: Duration of the content (in minutes or seasons)
- `listed_in`: Genre of the content
- `description`: Brief description of the content

## Project Steps

### Handling Null Values
Null values in the dataset were addressed to ensure data integrity and accuracy.

### Managing Nested Columns
Columns containing nested data, such as `director`, `cast`, `listed_in`, and `country`, were processed to enable better visualization and analysis.

### Binning Ratings
The `rating` attribute was binned into categories such as adult, children's, family-friendly, and not rated to facilitate analysis and recommendation.

### Exploratory Data Analysis (EDA)
EDA techniques were employed to gain insights and understand patterns and trends in the dataset, with the goal of preventing subscriber churn.

### Creating Clusters
Clustering techniques were applied to group the content based on attributes like `director`, `cast`, `country`, `genre`, `rating`, and `description`. These attributes were tokenized, preprocessed, and vectorized using the TF-IDF vectorizer.

### Dimensionality Reduction
The dimensionality of the dataset was reduced using Principal Component Analysis (PCA) to improve performance and eliminate noise.

### Clustering Algorithms
Both K-Means Clustering and Agglomerative Hierarchical Clustering algorithms were utilized to create clusters. The optimal number of clusters was determined (4 for K-Means and 2 for hierarchical clustering) using various evaluation methods.

### Content-Based Recommender System
A content-based recommender system was developed using the cosine similarity matrix to provide personalized recommendations to users. The aim was to reduce subscriber churn by offering relevant and engaging content.

## Conclusion
By conducting this comprehensive analysis of the Netflix dataset and developing a content-based recommendation system, the project aims to enhance user satisfaction and reduce subscriber churn for Netflix. The clustering of content allows for improved grouping and organization, while the recommender system provides personalized recommendations based on user preferences. It is expected that these efforts will lead to higher user retention rates and ultimately benefit Netflix in maintaining its position as a leading streaming entertainment platform.
