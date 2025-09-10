# Worldwide Box Office Analysis - PowerBI
## Project Overview
The Worldwide Box Office Analysis project dives more into the business angle of many popular films over time from different countries and languages across the world. Based on the two datasets from Kaggle 'movies_metadata' and 'Top_200_Movies_Dataset', Worldwide Box Office Analysis focuses on analyzing box office trends and providing data driven insights.

## Problem Description
The goal of this analysis is to study box office performance and trends by combining the two datasets 'movies_metadata' and 'Top_200_Movies_Dataset'. The former being a large dataset while the latter being a curated dataset. This analysis identifies highest/lowest grossing movies, compares vote average vs. vote count to examine audience reception, measure profitability and return on investment (ROI) across languages, explore genre-based, languages-based, and country-based success patterns, Highlight trends in Indian cinema and re-releases in 2023, and analyze revenue trends over the years (2000-present). This provides insights into factors like (budget, country, genre, language, or release year) that drive box office success.

## Dataset Information
### 1. movies_metadata
Contains global movie details:

Title, original title, production countries, spoken/original languages

Budget, revenue, release date, runtime, popularity

Genres, vote average, vote count, overview

~45,000+ movie entries (broad coverage across years and regions).

### 2. Top_200_Movies_Dataset_2023
Focused dataset of the top 200 highest-performing movies in 2023.

Includes:

Title, Total Gross (revenue), Release Date

Acts as a modern benchmark to compare against the broader dataset.

## Project Workflow
1. **Data Transformation:** The data from SQL was directly imported into Power BI and transformed in Power Query to align with the visualizations. Using the SQL queries as a base, I applied type conversions (budget, revenue, votes into numeric formats), cleaned invalid or missing values (removing nulls, empty arrays, and “?” entries), and derived new fields such as Profit (Revenue – Budget), ROI (Revenue ÷ Budget), and Year from release dates. I also merged the movies_metadata table with the Top 200 Movies 2023 dataset to enable combined analysis, ensuring genres, countries, and languages were standardized for grouping. These transformations ensured the Power BI visuals accurately reflected the queries I built in SQL.

2. **Data Visualization:** The transformed data was visualized in Power BI to highlight box office insights. Key visuals included a line chart of yearly revenue trends (2000–2023), bar charts for top grossing movies and genres, and a map showing country-level box office contributions. A scatter plot was used to compare budget vs. revenue with ROI, while treemaps and tables highlighted performance by languages and Indian cinema. Additional visuals like donut charts for 2023 re-releases and scatter plots of vote averages vs. vote counts provided deeper context into audience reception and market performance. Together, the visuals delivered a clear narrative on profitability, regional trends, and changing audience preferences.

## Conclusion:
The analysis reveals key drivers of box office success: budget efficiency (ROI), genre alignment, language reach, and international markets. Combining historical data with the 2023 benchmark highlights evolving audience preferences and the global nature of the film industry.
