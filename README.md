# Letterboxd Data Analysis Project

Welcome to my data analysis project where I dive into my personal movie diary from Letterboxd! Using the TMDb API, I've enriched my dataset with extensive metadata about each film. This project is an exploratory journey into various aspects of my movie-watching habits, visualized through Python and Tableau.

## Table of Contents

- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Python Skills Used](#python-skills-used)
- [Data Gathering](#data-gathering)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Visualization](#data-visualization)
- [Insights and Findings](#insights-and-findings)
- [Technologies Used](#technologies-used)
- [Future Directions](#future-directions)
- [General Information](#general-information)

## Introduction

Letterboxd is a vibrant social platform where movie lovers can share and discover reviews and ratings. Curious about the patterns in my own movie-watching habits, I started this project to explore the trends in my Letterboxd movie diary.

## Project Objectives

- To merge and clean data exported from my Letterboxd data and supplemented by the TMDb API.
- To conduct a thorough exploratory data analysis to discover trends in movie ratings, genres, and my viewing preferences.
- To visualize the findings using Python's Matplotlib and Tableau for clear, impactful insights.
- To identify my top watched directors, actors, and explore insights over movie release and watch dates.

## Python Skills Used
- **Data Cleaning**: Preparing raw data for analysis by handling missing values, outliers, and inconsistencies.
- **Data Merging**: Combining data from multiple sources into a unified dataset.
- **Pandas**: Utilizing the pandas library for efficient data manipulation and analysis.
- **Data Transformation**: Converting data into a suitable format for analysis.
- **Data Visualization**: Creating informative visualizations using Matplotlib and Seaborn.
- **Statistical Analysis**: Performing statistical tests and analysis to draw insights from data.
- **Jupyter Notebooks**: Documenting and presenting data analysis using Jupyter Notebooks for reproducible research.
- **Exploratory Data Analysis (EDA)**: Analyzing data to summarize its main characteristics, often with visual methods.
- **Data Importing and Exporting**: Reading data from various sources and writing results to files.

Feel free to explore the Jupyter notebooks to see my work in action. If you have any questions or feedback, please don't hesitate to reach out!

## Data Gathering

Data was initially extracted from my Letterboxd account as a CSV file containing basic movie details such as title, release year, and my personal ratings. To enrich this data, I utilized the TMDb API to fetch additional attributes including genres, runtime, and cast details, as demonstrated in the [Data-Get Jupyter Notebook](consolidate_data.ipynb).

## Data Cleaning

This phase involved refining the dataset by:
- Eliminating duplicate entries.
- Handling missing values appropriately.
- Converting data types for analysis readiness.
- Merging the enriched TMDb data with my Letterboxd exports.
Refer to the [Data-Get Jupyter Notebook](consolidate_data.ipynb) for detailed cleaning procedures.

## Dataset Information
This dataset contains my enriched diary of 326 entries. Each entry includes attributes such as:
- Title
- Release Date
- Watch Date
- Rating
- Genres
- Runtime
- Director
- Cast
- Origin Country
- Original Language
- Movie ID in the TMDb
- Many more attributes from the TMDb API that I chose not to include in the analysis, but are available for further exploration in the future.

There are also three additional tables for genres, directors, and origin countries; pivoted values to facilitate analysis.


## Exploratory Data Analysis

A comprehensive analysis was conducted to understand the dataset's structure and to uncover any underlying patterns. Key focus areas included:
- Counts by watch-date and release-date.
- Genre popularity and ratings distribution.
- Top directors and actors by movie count.
- Insights on rewatches and ratings.
- Deep dives into highly rated movies and their attributes.
Check out [Data-Explore Jupyter Notebook](EDA.working_data.ipynb) for detailed exploratory steps.

## Data Visualization

The insights derived from the analysis were visualized through engaging graphs and interactive dashboards in Tableau, accessible [here](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary). Highlights include KPI summaries and detailed genre, watch-date, and release-date analytics.

<div class='tableauPlaceholder' id='viz1718287424225' style='position: relative'><noscript><a href='https:&#47;&#47;letterboxd.com&#47;riuz&#47;stats&#47;'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Le&#47;LetterboxdAll-TimeStats&#47;Summary&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='LetterboxdAll-TimeStats&#47;Summary' /><param name='tabs' value='yes' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Le&#47;LetterboxdAll-TimeStats&#47;Summary&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1718287424225');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='1589px';vizElement.style.height='1015px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

## Insights and Findings

The project revealed fascinating insights such as my preference trends over different genres and how my movie ratings correlate with directors/actors.

## Technologies Used

- Python (Pandas, Matplotlib)
- Jupyter Notebook
- Tableau

## Future Directions

- Development of a web application to interactively explore the data of other people's movie diaries. Either via diary.csv upload or through username → webscraping.
- Deepclean the code and optimize for performance.
	- Define functions to reduce code replication.
	- Utilize the `tmdbsimple` Python library for data retrieval for simplicity.
	- Minimize file generation and manual data editing.
	- Optimize API requests for efficiency.
	- Enhance data update capabilities.

## General Information

For more insights and visual presentations, check out the [Letterboxd All-Time Stats - Tableau Workbook](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary).

For more about my projects and data journey, visit my [Portfolio](https://www.notion.so/ruizdelcarmen/Ruiz-del-Carmen-Data-Portfolio-e725748d0e0546c386be6c6c7dc49099).

---

*Note: To view the Jupyter notebooks, navigate to the respective file paths provided in each project description.*
