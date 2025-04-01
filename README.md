# Data Visualization Project 1

## Proposal: Analysis of Rolling Stone's Top 500 Albums Dataset

---

## 1. Dataset Overview

The dataset used in this project is the **Rolling Stone Album Rankings**, published on **May 7, 2024**, as part of the **TidyTuesday** initiative. It compiles the **500 Greatest Albums of All Time** according to Rolling Stone magazine and provides insights into rankings across multiple years (**2003, 2012, and 2020**), as well as additional metadata on the albums and artists.

### **Provenance**

- **Source:** [TidyTuesday Rolling Stone Album Rankings Dataset](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-05-07)
- **Original Publisher:** Rolling Stone Magazine
- **Data Collection:** Information compiled from Rolling Stone’s published rankings, Billboard statistics, and Spotify metadata

### **Dataset Dimensions**

- **Number of Observations:** 500 albums
- **Number of Variables:** 15+ (including numerical and categorical data)
- **Key Variables:**

  - **Numerical Variables:**
    - `rank_2003`, `rank_2012`, `rank_2020` (album rankings over the years)
    - `differential` (ranking change between 2020 and 2003)
    - `release_year` (year the album was released)
    - `spotify_popularity` (Spotify popularity score)
    - `weeks_on_billboard` (number of weeks on Billboard charts)
    - `peak_billboard_position` (highest position on Billboard charts)
  - **Categorical Variables:**
    - `album` (album title)
    - `artist` (artist or band name)
    - `genre` (album genre)
    - `artist_gender` (gender classification of the artist)
    - `type` (album classification, e.g., studio, live, compilation)

- **Full Data Dictionary:** [Rolling Stone Data Documentation](https://github.com/rfordatascience/tidytuesday/blob/main/data/2024/2024-05-07/readme.md#rolling_stonecsv)

---

## 2. Reason for Choosing This Dataset

### **Topic of Interest**

- Music rankings have been a **widely discussed topic for decades**, shaping public opinion, artist legacies, and industry recognition. The **Rolling Stone Top 500 Albums** dataset presents a unique opportunity to analyze how factors such as **release year, genre, artist type, and commercial success** impact an album’s standing in music history.

- Additionally, this dataset provides a **rich combination of historical rankings, commercial performance (Billboard data), and modern streaming popularity (Spotify metrics)**, making it ideal for **statistical analysis and data visualization**.

### **Dataset Compliance with Project Requirements**

**Published after 2023** – The dataset was released on **May 7, 2024**, ensuring it meets the publication date requirement.  
**Contains both numerical and categorical variables** – Includes:

- **Numerical variables:** ranking positions, album release years, streaming popularity.
- **Categorical variables:** album genres, artist names, artist gender.  
  **Sufficient complexity for analysis** – Contains multiple dimensions of data (historical rankings, artist metadata, streaming trends), allowing for diverse and meaningful research questions.

**Given these characteristics, this dataset is an excellent choice for our project, offering an opportunity to explore trends in music rankings over time and across various artist demographics.**

---

## 3. Two main questions to answer and

#### Question 1. How do an album's genre and release year influence its ranking changes from 2003 to 2020?

#### Question 2. How do artist gender and group size affect album popularity on Spotify?

---

## 4. Plan for answering each of the questions including the variables involved, variables to be created (if any), external data to be merged in (if any).

#### 1. How do an album's genre and release year influence its ranking changes from 2003 to 2020?

- Variables involved: genre, release_year, differential (rank_2020 - rank_2003)
- Plan: Use statistical methods like ANOVA or regression to assess the relationship between genre, release_year, and differential. Group albums by genre and decade of release, then compare **average differentials (new variable)** to identify trends.
- Visualizations: Box plots and line graphs to depict trends clearly over time.
- External data: None required

#### 2. How do artist gender and group size affect album popularity on Spotify?

- Variables involved: artist_gender, artist_member_count, spotify_popularity
- Plan: Use regression analysis to model spotify_popularity with artist_gender and artist_member_count as predictors, then explore interactions, such as whether gender effects vary by group size.
- Visualizations: Faceted scatter plots and grouped bar charts for clearer depiction of interactions.
- External data: None required
