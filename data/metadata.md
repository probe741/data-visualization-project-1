# 📄 **Dataset Metadata**

---

## 1. Dataset Overview

- **Title**: TidyTuesday Rolling Stone Album Rankings Dataset
- **Description**:
  It compiles the **500 Greatest Albums of All Time** according to Rolling Stone magazine and provides insights into rankings across multiple years (**2003, 2012, and 2020**), as well as additional metadata on the albums and artists.

## 2. Provenance

- **Source:** [TidyTuesday Rolling Stone Album Rankings Dataset](https://github.com/rfordatascience/tidytuesday/tree/main/data/2024/2024-05-07)
- **Original Publisher:** Rolling Stone Magazine
- **Data Collection:** Information compiled from Rolling Stone’s published rankings, Billboard statistics, and Spotify metadata

## 3. Dataset Structure

| variable                 | class     | description                                                                                                              |
| :----------------------- | :-------- | :----------------------------------------------------------------------------------------------------------------------- |
| sort_name                | character | Name used for sorting                                                                                                    |
| clean_name               | character | Clean name                                                                                                               |
| album                    | character | Album name                                                                                                               |
| rank_2003                | double    | Rank in 2003. NA if album not released yet or not in top 500.                                                            |
| rank_2012                | double    | Rank in 2012. NA if album not released yet or not in top 500.                                                            |
| rank_2020                | double    | Rank in 2020. NA if not in top 500.                                                                                      |
| differential             | double    | 2020-2003 Differential. Negative value if it went down in the chart. Positive value if it went up.                       |
| release_year             | double    | Release Year                                                                                                             |
| genre                    | character | Album Genre                                                                                                              |
| type                     | character | Album Type                                                                                                               |
| weeks_on_billboard       | double    | Weeks on Billboard                                                                                                       |
| peak_billboard_position  | double    | Peak Billboard Position                                                                                                  |
| spotify_popularity       | double    | Spotify Popularity. NA if not on Spotify.                                                                                |
| spotify_url              | character | Spotify URL. NA if not on Spotify.                                                                                       |
| artist_member_count      | double    | Number of artists in the group                                                                                           |
| artist_gender            | character | Gender of the artist(s). Male/Female if it's a mixed-gender group.                                                       |
| artist_birth_year_sum    | double    | Sum of the artists birth year. e.g. for a 2 member group, with one person born 1945 and another 1950, the value is 3895. |
| debut_album_release_year | double    | Debut Album Release Year                                                                                                 |
| ave_age_at_top_500       | double    | Average age at top 500 Album                                                                                             |
| years_between            | double    | Years Between Debut and Top 500 Album                                                                                    |
| album_id                 | character | Album ID. NOS at the beginning of the ID if not on Spotify.                                                              |
