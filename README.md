# Letterboxd Data Analysis Project

Welcome to my data analysis project where I dive into my personal movie diary from Letterboxd! Using the TMDb API, I've enriched my dataset with extensive metadata about each film. This project is an exploratory journey into various aspects of my movie-watching habits, visualized through Python and Tableau.

## Table of Contents

- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Data Gathering](#data-gathering)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Visualization](#data-visualization)
- [Insights and Findings](#insights-and-findings)
- [Technologies Used](#technologies-used)
- [Future Directions](#future-directions)
- [General Information](#general-information)

## Introduction

Letterboxd serves as a vibrant social platform for film enthusiasts to share and discover film reviews and ratings. Intrigued by the storytelling potential of data in my own movie-watching experiences, I embarked on this project to uncover trends and patterns from my Letterboxd movie diary.

## Project Objectives

- To merge and clean data exported from Letterboxd and supplemented by the TMDb API.
- To conduct a thorough exploratory data analysis to discover trends in movie ratings, genres, and viewer preferences.
- To visualize the findings using Python's Matplotlib and Tableau for clear, impactful insights.
- To identify my top watched directors, actors, and explore genre popularity over time.

## Data Gathering

Data was initially extracted from my Letterboxd account as a CSV file containing basic movie details such as title, release year, and my personal ratings. To enrich this data, I utilized the TMDb API to fetch additional attributes including genres, runtime, and cast details, as demonstrated in the Jupyter Notebook `consolidate_data.ipynb`.

## Data Cleaning

This phase involved refining the dataset by:
- Eliminating duplicate entries.
- Handling missing values appropriately.
- Converting data types for analysis readiness.
- Merging the enriched TMDb data with my Letterboxd exports.
Refer to the Jupyter Notebook `consolidate_data.ipynb` for detailed cleaning procedures.

## Exploratory Data Analysis

A comprehensive analysis was conducted to understand the dataset's structure and to uncover any underlying patterns. Key focus areas included:
- Counts by watch-date and release-date.
- Genre popularity and ratings distribution.
- Top directors and actors by movie count.
- Insights on rewatches and ratings.
- Deep dives into highly rated movies and their attributes.
Check out `EDA.working_data.ipynb` for detailed exploratory steps.

## Data Visualization

The insights derived from the analysis were visualized through engaging graphs and interactive dashboards in Tableau, accessible [here](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary). Highlights include KPI summaries and detailed genre, watch-date, and release-date analytics.

## Insights and Findings

The project revealed fascinating insights such as my preference trends over different genres and how my movie ratings correlate with movie popularity and critical acclaim.

## Technologies Used

- Python (Pandas, Matplotlib)
- Jupyter Notebook
- Tableau

## Future Directions

- Development of a web application to interactively explore the data of other people's movie diaries.
- Deepclean the code and optimize for performance.
	- Define functions to reduce code replication.
	- Utilize the `tmdbsimple` Python library for data retrieval.
	- Minimize file generation and manual data editing.
	- Optimize API requests for efficiency.
	- Enhance data update capabilities.

## General Information

For more insights and visual presentations, check out the [Letterboxd All-Time Stats - Tableau Workbook](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary).

For more about my projects and data journey, visit my [Portfolio](https://www.notion.so/ruizdelcarmen/Ruiz-del-Carmen-Data-Portfolio-e725748d0e0546c386be6c6c7dc49099).
