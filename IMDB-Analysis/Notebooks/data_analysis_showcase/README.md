# IMDB Data Analysis

Analysis of IMDB dataset using SQL and Python.

## 📊 Analysis Overview

This project explores the IMDB database to identify top-rated movies, popular genres, and most frequent actors in highly-rated productions.

## 🎯 Key Analyses

### 1. Top Rated Movies
**Query:** Find 5 highest-rated movies with vote count as tie-breaker

**Results:**
- "Ozymandias" - ⭐ 10.0 (228,900 votes)
- "Kadifeyi Kesfet" - ⭐ 10.0 (2,904 votes)
- "Tatilde CUK Oturur Mukemmel Durur" - ⭐ 10.0 (2,878 votes)

### 2. Most Frequent High-Rated Genre
**Method:** Genre count for movies rated > 8.0

**Finding:** **Drama** dominates with 108,356 occurrences

### 3. Most Active Actors in Quality Films
**Query:** Actors with most appearances in movies rated > 7.5

**Top Performers:**
- Actor 1: 4,027 participations
- Actor 2: 3,792 participations  
- Actor 3: 2,801 participations

## Technical Stack

- **Python** + **Pandas** for data analysis
- **SQL** for database queries
- **SQLite** as database management system

## Files

- `imdb_sql_analysis.ipynb` - Main analysis notebook
- `imdb_sql_analysis.html` - Exported notebook for quick viewing


