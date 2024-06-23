# Letterboxd Data Analysis Project

## Table of Contents

- [Introduction](#introduction)
- [Project Objectives](#project-objectives)
- [Data Preparation](#data-preparation)
- [Exploration and Visualization](#exploration-and-visualization)
- [Insights and Findings](#insights-and-findings)
- [Technologies Used](#technologies-used)
- [Future Directions](#future-directions)
- [General Information](#general-information)

## Introduction

Welcome to my data analysis project, where I delve into my personal movie-watching habits using my Letterboxd diary. This exploration is powered by enriching the dataset with extensive metadata from the TMDb API and visualizing it through Python and Tableau. This project aims to uncover patterns and insights that inform future film recommendations, demonstrating my capacity to translate personal data into actionable insights. Letterboxd, a platform for film enthusiasts, serves as the foundation for this analysis, illustrating the potential of storytelling through data in making informed viewing choices.

## Project Objectives | Business Questions

1. **Viewing Habits:**
    - What are the most common genres watched?
    - How have viewing patterns changed over time?
    - What are the most watched directors, actors, or writers?
    - What are some insights into the movies I end up rewatching?
2. **Movie Ratings:**
    - What is the distribution of movie ratings?
    - Are there particular genres or directors that consistently receive higher ratings?
3. **Correlations and Insights:**
    - Is there a correlation between the length of a movie and its rating?
    - Are certain genres or types of movies more popular during specific seasons or months?
    - Does watching movies from certain countries or in certain languages correlate with higher enjoyment or ratings?
    - Are newer movies rated more favorably than older ones?

## Data Preparation

326 entries were first extracted from my Letterboxd account as a CSV file with basic movie details like title, release year, and ratings. I then enriched this data using the TMDb API to include genres, runtime, and cast details, as detailed in the `consolidate_data.ipynb` Jupyter Notebook. The data cleaning phase involved removing duplicates, handling missing values, converting data types for analysis, and merging the TMDb data with the Letterboxd exports. For a detailed walkthrough of the cleaning procedures, refer to the `consolidate_data.ipynb` notebook. There are also three additional tables for genres, directors, and origin countries; pivoted values to facilitate analysis.


## Exploration and Visualization

A comprehensive analysis was conducted to understand the dataset's structure and to uncover any underlying patterns. Key focus areas included:
- Counts by watch-date and release-date.
- Genre popularity and ratings distribution.
- Top directors and actors by movie count.
- Insights on rewatches and ratings.
- Deep dives into highly rated movies and their attributes.
Check out `EDA.working_data.ipynb` for detailed exploratory steps.

The insights derived from the analysis were visualized through engaging graphs and interactive dashboards in Tableau, [accessible here](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary). Highlights include KPI summaries and detailed genre, watch-date, and release-date analytics.

## Insights and Findings

The project revealed fascinating insights such as my preference trends over different genres and how my movie ratings correlate with each rewatch/cast & crew. Here is what I discovered:

### 1. Targeted Genre Exploration:

- **Discovery:** While Drama, Comedy, Action, Science Fiction, Adventure, Romance, Thriller, and Crime dominate my viewing habits, I've developed a higher appreciation for less-watched genres like Music, War, History, and Mystery.
- **Action:** Intentionally seek out and watch more films from these underrepresented genres to diversify my cinematic experience and potentially discover new favorites.

### 2. Rewatch Strategy:

- **Discovery:** My ratings generally increase on rewatch, particularly for films initially rated above 3 stars, while some like “Train to Busan” rated lower. This insight is complemented by the finding that movies with initially high ratings are more likely to be rewatched and often maintain or improve in ratings.
- **Action:** Implement a strategy to rewatch films I rated lower than 3 stars to see if my perceptions change over time, providing deeper insights into my rating patterns and preferences.

### 3. Director and Actor Emphasis:

- **Discovery:** Quentin Tarantino, and Denis Villeneuve are the most watched directors. Samuel L. Jackson, Brad Pitt, J.K. Simmons, Chris Pratt, Scarlett Johansson, and Willem Dafoe are the most watched actors.
- **Action:** Explore more films by directors with a distinct style, especially those I enjoy but haven’t watched much. Also, consider watching more films featuring under-appreciated actors who have positively surprised me.

### 4. Support for Local Cinema:

- **Discovery:** There's a predominance of US-origin films in my watch history. Making up 85.58% of the entries, while PH-origin movies are only about 3.68%.
- **Action:** Actively seek out films produced in the Philippines to balance my viewing habits and support local industry growth.

### 5. High-Rating Patterns:

- **Discovery:** High ratings are often given to genres like Music, War, History, Mystery, Family, and Drama; directors like Christopher Nolan, Richard Linklater, Richard Curtis, Luca Guadagnino, and Denis Villeneuve have at least two watched-moves that were highly rated; actors like Michael Stuhlbarg, Ethan Hawke, Jake Gyllenhaal, Dave Bautista, Linda Cardellini, Kyle Bornheimer, Haruka Abe, Tom Stourton, Julie Delpy, Angela Bassett, and Domhnall Gleeson are highly rated.
- **Action:** Dive into movies with these specific attributes to see if my interest aligns with these high ratings. If not, I could normalize my data to provide a deeper understanding of my preferences.
- Just for fun, I plugged these highly-rated attributes into ChatGPT and these are 15 movies it told me to watch next.
    
🤠: Recommend me 15 movies that meet these attributes. At least 3 of the attributes should be met.

High ratings are often given to genres like Music, War, History, Mystery, Family, and Drama; directors like Christopher Nolan, Richard Linklater, Richard Curtis, Luca Guadagnino, and Denis Villeneuve have at least two watched-moves that were highly rated; actors like Michael Stuhlbarg, Ethan Hawke, Jake Gyllenhaal, Dave Bautista, Linda Cardellini, Kyle Bornheimer, Haruka Abe, Tom Stourton, Julie Delpy, Angela Bassett, and Domhnall Gleeson are highly rated. 

For each movie, pinpoint the attribute/s that were met. Feel free to scour for movies that overlap in genre, directors, or actors.

🤖: 
Here's a curated list of 15 movies that meet your criteria, each featuring a combination of the genres, directors, or actors you prefer:

1. **Dunkirk (2017)** - Directed by Christopher Nolan. Genres: War, History, Drama. This film covers multiple attributes with its acclaimed direction by Nolan and its intense portrayal of war.

2. **Arrival (2016)** - Directed by Denis Villeneuve. Genres: Mystery, Drama. This sci-fi mystery features a compelling narrative directed by Villeneuve.

3. **Sicario (2015)** - Directed by Denis Villeneuve. Genre: Mystery. Another intense and highly-rated film directed by Villeneuve, known for its gripping storyline and mystery elements.

4. **Interstellar (2014)** - Directed by Christopher Nolan. Genre: Drama. Nolan's directorial brilliance shines in this dramatic space exploration epic.

5. **Call Me by Your Name (2017)** - Directed by Luca Guadagnino. Genre: Drama, Family. This romantic drama highlights Guadagnino's sensitive direction and explores deep emotional and family themes.

6. **Before Sunset (2004)** - Directed by Richard Linklater. Genre: Drama. Featuring Ethan Hawke, this film excels in its dramatic portrayal of a romantic encounter, directed by Linklater.

7. **Boyhood (2014)** - Directed by Richard Linklater. Genre: Drama, Family. Another Linklater classic, known for its unique filming over many years, capturing family and drama.

8. **Prisoners (2013)** - Directed by Denis Villeneuve. Genre: Mystery, Drama. This film features Jake Gyllenhaal and showcases Villeneuve's mastery in creating a tense mystery drama.

9. **Atonement (2007)** - Genre: Drama, War, History. While not directed by one of your listed directors, this film fits well within the highly-rated war, history, and drama genres.

10. **The Theory of Everything (2014)** - Genre: Drama, Family. Focusing on the life of Stephen Hawking, this film captures deep family and dramatic elements.

11. **Blade Runner 2049 (2017)** - Directed by Denis Villeneuve. Genre: Mystery, Drama. Featuring Dave Bautista and directed by Villeneuve, this sequel brings together mystery and drama in a visually stunning way.

12. **Nightcrawler (2014)** - Genre: Mystery, Drama. Featuring Jake Gyllenhaal, this film delivers an intense mystery and dramatic narrative.

13. **Love Actually (2003)** - Directed by Richard Curtis. Genre: Drama, Family. A classic romantic drama that's highly acclaimed for its ensemble cast and Curtis's engaging storytelling.

14. **Green Book (2018)** - Genre: Drama, Family, History. While not directly meeting the director or specific actor criteria, it excellently captures the essence of family, drama, and historical themes.

15. **Mudbound (2017)** - Genre: Drama, History, War. This film delves deeply into historical and war themes with a dramatic narrative, fitting your genre preferences well.

Each movie listed meets at least three of the specified attributes, whether through its genre, director, or featured actors.

-- Fun fact: I've watched 7/15 films! Time to watch the rest ;)


## Technologies Used

- Python (Pandas, Matplotlib)
- Jupyter Notebook
- Excel
- Tableau

## Future Directions

- Development of a web application to interactively explore the data of other people's movie diaries.
- Not all business questions were answered; I thought of additional business questions that could be answered with the data after finishing the project. Did not pursue answering them due to time constraints.
- Deepclean the code and optimize for performance.
	- Define functions to reduce code replication.
	- Utilize the `tmdbsimple` Python library for data retrieval.
	- Minimize file generation and manual data editing.
	- Optimize API requests for efficiency.
	- Enhance data update capabilities.

## General Information

For more insights and visual presentations, check out the [Letterboxd All-Time Stats - Tableau Workbook](https://public.tableau.com/views/LetterboxdAll-TimeStats/Summary).

For more about my projects and data journey, visit my [Portfolio](https://www.notion.so/ruizdelcarmen/Ruiz-del-Carmen-Data-Portfolio-e725748d0e0546c386be6c6c7dc49099).
