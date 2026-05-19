# MovieLens 100K Dataset

## Overview
This dataset contains 100,000 ratings (ranging from 1 to 5) from 943 users across 1,682 movies. Every user included has rated at least 20 movies and has complete demographic information. 

The data was collected by the **GroupLens Research Project** at the University of Minnesota through the MovieLens website (`movielens.umn.edu`) between September 19, 1997, and April 22, 1998.

---

## Dataset Download Links
If you need to re-download the dataset or access it directly from the source, you can find it via the official GroupLens channels:
* **Direct Download (Stable Link):** [GroupLens MovieLens 100k Dataset](https://files.grouplens.org/datasets/movielens/ml-100k.zip)
* **Official Website:** [GroupLens Datasets Page](https://grouplens.org/datasets/movielens/)
* **MovieLens Platform:** [MovieLens Web App](http://www.movielens.org/)

---

## Core Data Files

### 1. `u.data` (Ratings Matrix)
* **Description:** The full ratings dataset consisting of 100,000 rows. Users and items are numbered consecutively starting from 1.
* **Format:** Tab-separated values (`\t`)  
  `user id | item id | rating | timestamp`
* **Notes:** Timestamps represent Unix seconds elapsed since January 1, 1970, UTC.

### 2. `u.item` (Movie Information)
* **Description:** A dataset containing details for all 1,682 movies. The movie IDs match the ones used in `u.data`.
* **Format:** Tab-separated values (`\t`)  
  `movie id | movie title | release date | video release date | IMDb URL | [19 Genre Fields]`
* **Genres:** The final 19 fields are binary flags (`1` for yes, `0` for no) indicating the movie's genres. A movie can belong to multiple genres simultaneously. 
  * *Genres include:* Action, Adventure, Animation, Children's, Comedy, Crime, Documentary, Drama, Fantasy, Film-Noir, Horror, Musical, Mystery, Romance, Sci-Fi, Thriller, War, Western, and unknown.

### 3. `u.user` (User Demographics)
* **Description:** Demographic information for the 943 unique users. The user IDs match the ones used in `u.data`.
* **Format:** Tab-separated values (`\t`)  
  `user id | age | gender | occupation | zip code`

---

## Metadata Reference Files
* **`u.info`:** Displays the total count of users (943), items (1682), and ratings (100000) in the dataset.
* **`u.genre`:** A list of the 19 movie genres used in the dataset.
* **`u.occupation`:** A list of the unique occupations recorded for the users.

---

## Terms & Conditions
* **Research Use Only:** The data may be used for research purposes. It cannot be used for commercial or revenue-bearing purposes without separate permission from GroupLens.
* **No Redistribution:** You are not permitted to redistribute the data files without explicit permission.
* **Citation:** Any publication resulting from the use of this dataset must cite the following paper:
  > F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. *ACM Transactions on Interactive Intelligent Systems (TiiS)* 5, 4, Article 19 (December 2015). DOI: http://dx.doi.org/10.1145/2827872
