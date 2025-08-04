# 📚 Maven Bookshelf Challenge – Power BI Dashboard

> **Submitted for:** [Maven Analytics Bookshelf Challenge](https://www.mavenanalytics.io/challenges/maven-bookshelf-challenge)  
> **Created by:** Thejaswini H  
> **Role:** Data Analyst | Dashboard Designer  
> **Tools Used:** Power BI, DAX, Power Query, Excel  

---

## 🧩 Project Objective

To build an **interactive Power BI dashboard** that helps readers curate their **ideal summer reading list** by uncovering hidden gems, popular favorites, and genre trends using real Goodreads data.

This project demonstrates skills in **data cleaning, data modeling, dashboard creation**, and **insight generation** using large and complex datasets.

---

## 🗃️ Dataset Overview

The dataset was provided by Maven Analytics and is based on a 2017 Goodreads public export. It includes over **1.4 million reviews**, covering **13,000+ books** and their associated metadata.

### 🔸 Tables Used:
1. **Works.csv** – Book metadata (title, author, publication year, average rating, rating count, page count)
2. **Genre.csv** – Book-to-genre mapping (many-to-many relationship)
3. **Reviews.csv** – Individual user reviews (ratings, text, spoiler flags)

---

## 🔧 Step-by-Step Implementation

### 🔹 1. **Data Import & Preparation**
- Loaded all three CSV files into **Power BI**
- Explored relationships:
  - `Works` (1-to-many) → `Reviews`
  - `Works` (1-to-many) → `Genre`
- Created proper **data model relationships**
- Checked for missing/null values
- Converted data types (dates, text, integers)

### 🔹 2. **Data Cleaning & Transformation**
- Used **Power Query Editor** to:
  - Remove duplicates and empty rows
  - Standardize rating values
  - Format dates and create `ReviewYear` column
- Merged datasets to enrich `Works` with review and genre info

### 🔹 3. **DAX Measures Created**
- `Average Rating`
- `Total Reviews`
- `Review Count by Year`
- `Books with 4.5+ Rating & <500 Reviews` → **Hidden Gems**
- `Avg Pages by Genre`
- `Spoiler Review %`
- `Sentiment Approx Score` *(basic keyword tagging method used)*

### 🔹 4. **Dashboard Visuals**
- **Bar Chart**: Average Rating by Genre
- **Scatter Plot**: Rating vs Rating Count (popularity vs quality)
- **Line Chart**: Review trend over years
- **Bubble Chart**: Avg Pages vs Avg Rating
- **Word Cloud**: Most common positive/negative words in reviews
- **Slicers** for Genre, Year, Rating Range, Page Count

---

## 📊 Key Insights Uncovered

### 🟢 Hidden Gems
- Identified **50+ books** with 4.5+ average rating but fewer than 500 reviews
- Example: _“The Lost Vintage”_ – High satisfaction but low visibility

### 🟡 Genre Trends
- **Highest Avg Ratings**: Historical Fiction, Biography, Memoir
- **Most Reviewed Genres**: Fantasy, Romance, Thriller

### 🔵 Reader Behavior
- **Spoiler Reviews** made up ~15% of total; often appeared on highly rated books
- Books with **fewer than 300 pages** received **more consistent high ratings**

### 🟠 Publication Insights
- Peak publishing years: **2005–2015**
- 📈 Highest growth in reviews was between 2010 and 2016
- Older books tended to have more balanced review scores

### 🔴 Sentiment Patterns
- Reviews with words like “masterpiece”, “life-changing”, and “couldn’t put it down” heavily correlated with 5⭐ ratings
- Negative reviews included terms like “predictable”, “boring”, “flat ending”

---

## 🖥️ Dashboard Demo (Screenshots)

📌 [Insert screenshot previews here, like dashboard-overview.png, hidden-gems-chart.png]

---

## 🔄 Filters & Slicers Available

| Slicer | Purpose |
|--------|---------|
| **Genre** | View trends within a specific genre |
| **Rating Range** | Focus on high/low rated books |
| **Publication Year** | Analyze historical trends |
| **Pages Range** | Filter books by length (e.g., quick reads) |

---

## 📁 Folder Structure

