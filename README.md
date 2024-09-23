# IMDB Movie Analysis

This project analyzes a dataset of movies from IMDB to identify factors that influence a movie's success, measured through IMDB ratings. The analysis covers various aspects like movie genres, budget, director impact, and more, providing filmmakers and stakeholders with actionable insights to make data-driven decisions.

## Project Description
**Objective**:  
The goal of this project is to explore and uncover trends and patterns in the IMDB dataset to understand what contributes to a movie’s success. The insights will guide filmmakers, producers, and other stakeholders in optimizing their movie production strategies based on data-driven evidence.
**Target Audience**:  
- Filmmakers
- Producers
- Studio Executives
- Movie Analysts

## Dataset Overview
**Number of Movies**: 5043  
**Number of Features**: 28
**Features Include**:
- `director_name`: Name of the movie’s director.
- `actor_1_name`, `actor_2_name`, `actor_3_name`: Names of the main actors.
- `genres`: Movie genres.
- `budget`: The budget of the movie.
- `gross`: The gross revenue.
- `imdb_score`: IMDB rating of the movie.
- `duration`: Duration of the movie.
- `language`, `country`, `content_rating`: Various metadata about the movie.
  
## Data Preprocessing
Several data cleaning steps were performed to prepare the data for analysis:
1. **Handling Missing Values**: Missing data in key columns like `gross`, `budget`, and `aspect_ratio` were handled using methods like imputation (via regression models) and data scraping from external sources (Wikipedia).
2. **Removing Duplicates**: We found and removed 90 duplicate rows, keeping the first instance.
3. **Outlier Detection**: Outliers in columns such as `duration` and `budget` were handled by replacing extreme values with the median.
4. **Feature Engineering**: Created new columns like `margin` (difference between gross revenue and budget) and `genre_no` (number of genres per movie).

## Key Insights and Findings
### 1. **Genre Analysis**  
- The most common genres are **Drama**, **Comedy**, and **Thriller**.
- **Horror** movies show the widest range of IMDB scores, suggesting variability in quality.
- **Comedy** movies, on average, have the lowest IMDB ratings (mean = 6.43).
### 2. **Duration Analysis**  
- A slight positive correlation exists between movie duration and IMDB scores.
- Most movies are between 90 and 120 minutes, with higher-rated films tending to be longer.

### 3. **Language Analysis**  
- **English** is the most common language in the dataset, followed by **French** and **Spanish**.
- **Mandarin** films have the highest average IMDB scores, with a mean score of 7.60.
### 4. **Director Analysis**  
- **Peter Jackson** has the highest average IMDB score (7.89) among top directors.
- Directors like **Andrew Stanton** and **Morten Tyldum** are in the 97th percentile for high IMDB ratings.
### 5. **Budget and Profit Analysis**  
- **Avatar**, **Jurassic World**, and **Titanic** have the highest profit margins.
- There is a positive relationship between budget and gross earnings, but high-budget movies don’t always guarantee high profits.

## Tools & Technologies
- **Python (Jupyter Notebook)**: Used for data preprocessing and analysis.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations and handling arrays.
- **Matplotlib & Seaborn**: For data visualization.
- **Microsoft Excel**: For data extraction, filtering, and visual analysis.
- **Web Scraping (BeautifulSoup)**: Used for filling missing values by scraping data from Wikipedia.

## Conclusion
This project demonstrates how data analytics can provide valuable insights into the factors influencing movie success. By understanding trends in genres, budget allocations, director impact, and more, filmmakers and stakeholders can make more informed, data-driven decisions in the film industry.

## How to Run the Project
1. Download the dataset from the provided Google Spreadsheet.
2. Run the Jupyter Notebook to explore the data preprocessing, analysis, and visualizations.
3. Review the PowerPoint presentation for a summary of insights.
