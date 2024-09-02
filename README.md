# Netflix Data Analytics Case Study

## Project Overview

This project aims to analyze Netflix's content library to provide actionable insights that can guide strategic decisions in content creation, acquisition, and release planning. The analysis covers various aspects such as content distribution by country, actor and director influence, optimal release timing, genre distribution, and more.

## Problem Statement : 

Netflix is a subscription-based streaming service headquartered in the United States, offering on-demand video content over the internet. We want to use this data to help Netflix figure out what kinds of shows and movies to make and how to grow their business in different countries. We'll look at things like how many movies come out each year, compare TV shows to movies, figure out the best time to release TV shows, check out the actorsand directors, and see what kinds of content are available globally. The main goal is to give Netflix practical advice based on the data so they can make better decisions about what to show and where to expand their business.

## Tools :
- Jupyter Notebook (for Python)
- Python Libraries

## Steps Involved

### 1. Data Collection
- **Dataset:** The analysis uses a dataset containing 8,807 entries with 12 columns, including information about titles, directors, cast, country, release dates, and more.

### 2. Data Preprocessing
- **Handling Missing Values:** Addressed missing data in columns like `director`, `cast`, `country`, `date_added`, and `rating` through data imputation or exclusion as necessary.
- **Data Type Conversion:** Converted relevant columns such as `date_added` to datetime format for accurate time-based analysis.
- **Exploding Columns:** Split and exploded columns like `listed_in` (genres) and `country` to handle multiple values and perform more granular analysis.

### 3. Exploratory Data Analysis (EDA)
- **Data Summary:** Generated a statistical summary of numerical columns, such as `release_year`.
- **Value Counts:** Calculated value counts for categorical variables such as `type` (Movie or TV Show) and `rating`.
- **Distribution Analysis:** Created histograms and count plots to understand the distribution of content by release year, genre, and country.

### 4. Data Transformation
- **Duration and Seasons:** Split the `duration` column into `duration_min` and `num_seasons` for Movies and TV Shows, respectively.
- **Time Lag Calculation:** Calculated the time lag between a movie's release and its addition to Netflix, identifying a mode lag of 334 days.

### 5. Visualization
- **Count Plots:** Created visualizations to show the distribution of content by release year, rating, and month.
- **Pie Charts:** Visualized the distribution of top genres and top countries contributing content to Netflix.
- **Correlation Heatmaps:** Generated heatmaps to identify correlations between numerical features like `release_year`, `duration_min`, and `num_seasons`.
- **Pair Plots:** Explored relationships between variables using pair plots, categorized by content type (Movie or TV Show).

### 6. Business Insights
- **Country Dominance:** The United States has the highest number of titles (3,689), showing its dominant influence on the platform's content.
- **Top Cast and Directors:** Identified key actors (Anupam Kher, Shah Rukh Khan) and directors (Rajiv Chilaka, Jan Suter) with the most titles, suggesting opportunities for strategic partnerships.
- **Optimal Release Timing:** December is the best month for TV show releases, while July is optimal for movies. Weekly strategies identified specific weeks that are most productive for TV show and movie releases.
- **Genre Distribution:** Analysis of genre distribution highlighted the popularity of categories like International Movies and Dramas, informing targeted content creation.

### 7. Recommendations
- **Expand Global Content:** Focus on increasing diverse international titles to cater to a global audience.
- **Invest in Star Talent:** Collaborate with popular actors and directors to enhance the platform's appeal.
- **Strategic Release Planning:** Utilize insights on optimal release months and weeks to maximize viewership.
- **Content Acquisition Strategy:** Ensure timely addition of popular titles to the Netflix library based on the identified time lag.

## Conclusion

The insights derived from this analysis provide Netflix with valuable data-driven recommendations to optimize content strategy, enhance viewer engagement, and strengthen its global presence.
