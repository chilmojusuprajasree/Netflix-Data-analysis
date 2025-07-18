# 📺 Netflix SQL Analysis Project

## 🧾 Overview
This project presents a comprehensive analysis of Netflix's Movies and TV Shows dataset using SQL. The goal is to extract actionable business insights and demonstrate data handling capabilities through real-world queries.

---

## 🎯 Objectives

- Analyze the distribution of content types (Movies vs TV Shows).
- Identify the most common ratings for each content type.
- Explore content trends based on release year, country, and duration.
- Categorize and filter content using keywords and criteria.
- Highlight top actors, directors, and genres.

---

## 📊 Dataset

- **Source:** [Kaggle – Netflix Shows Dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- **Table Name:** `netflix`

### 📁 Table Schema

```sql
DROP TABLE IF EXISTS netflix;
CREATE TABLE netflix (
    show_id      VARCHAR(5),
    type         VARCHAR(10),
    title        VARCHAR(250),
    director     VARCHAR(550),
    casts        VARCHAR(1050),
    country      VARCHAR(550),
    date_added   VARCHAR(55),
    release_year INT,
    rating       VARCHAR(15),
    duration     VARCHAR(15),
    listed_in    VARCHAR(250),
    description  VARCHAR(550)
);

📌 Findings & Conclusion
- Content Type: ~69% Movies and ~31% TV Shows.

Popular Ratings: 'TV-MA' is the most frequent rating.

Top Countries: USA, India, and UK produce the most content.

Genre Spread: **Dramas and Documentaries dominate the genres.

Content Flagging: 23% labeled as ‘Bad’ due to violent/kill-related keywords.

India Trend: Over 60% of Indian content was added in the last 5 years.

Celebrity Insight: Salman Khan featured in multiple titles over the last decade.
