# 📚 Maven Bookshelf Challenge – Power BI Dashboard

> **Challenge Name:** [Maven Analytics Bookshelf Challenge](https://www.mavenanalytics.io/challenges/maven-bookshelf-challenge)  
> **Created by:** Thejaswini H  
> **Role:** Data Analyst | Dashboard Designer  
> **Tools Used:** Power BI, DAX, Power Query, Excel  

---

## 🎯 Project Objective

The goal of this project was to create an interactive Power BI dashboard using Goodreads book review data to help users build their **ideal summer reading list**. The dashboard empowers readers to explore books by genre, rating, publication year, and page count to uncover:

- ⭐ Hidden literary gems  
- 📈 Reader favorites by genre  
- 📚 Quick, high-quality reads  
- 🔍 Patterns in publishing and reader trends  

This project focuses on solving the real problem statement — providing **personalized, data-driven book discovery**.

---

## 🗃️ Dataset Overview

Provided by Maven Analytics, this dataset includes:

- Over **1.4 million reviews**
- More than **13,000 books**
- Data collected from **Goodreads public user shelves** (2017)

### 🔸 Files Used:
1. `Works.csv` – Book-level data (title, author, ratings, pages, pub date)  
2. `Genre.csv` – Genre associations for each book  
3. `Reviews.csv` – User review ratings (no text or sentiment used in this project)

---

## 🔧 Step-by-Step Implementation

### 🔹 1. Data Loading & Relationships
- Loaded all CSVs into **Power BI**
- Defined relationships:
  - `Works` → `Genre` (many-to-many via bridge)
  - `Works` → `Reviews` (1-to-many)

### 🔹 2. Data Cleaning & Transformation
- Removed duplicates and null values
- Created new columns like:
  - `Publication Year`
  - Page bins: “<200 pages”, “200–400”, “400+”
- Ensured consistent datatypes (dates, integers, text)

### 🔹 3. Data Modeling in Power BI
- Defined relationships to support one-to-many joins
- Built dimensional model for genre filtering, rating analysis, etc.

### 🔹 4. DAX Measures & KPIs
- `Average Rating`
- `Total Reviews`
- `Book Count by Genre`
- `Books with High Ratings & Low Review Count` – Hidden Gems
- `Avg Pages by Genre`
- `Books by Publication Year`

### 🔹 5. Dashboard Design
Designed an intuitive, reader-friendly layout in Power BI including:
- Bar charts for average rating by genre
- Scatter plot of popularity vs quality
- Year-wise publishing trends
- Book length vs rating comparison
- Slicers for:
  - Genre
  - Publication Year
  - Rating
  - Page Count

---

## 📊 Key Insights from the Dashboard

### 🟢 Hidden Gems
- Books rated 4.5+ but reviewed fewer than 500 times  
- Helped surface 50+ underrated but highly loved books

### 🟡 Genre Trends
- Historical Fiction and Memoir genres have the **highest average ratings**
- Fantasy and Romance dominate in **review volume**

### 🔵 Publishing Patterns
- Most books in dataset published between **2005–2015**
- Book output peaked around 2010–2013

### 🟠 Reader Preferences
- Shorter books (<300 pages) tend to receive **more consistent positive ratings**
- Mid-length books (200–400 pages) make up the majority of highly rated titles

---

## 🖥️ Dashboard Preview

![Dashboard]("C:\Users\Teja\OneDrive\Pictures\Screenshots\Top_Authors.png")

---


---

## 🧠 Learnings

- Practiced data modeling with real-world relational datasets  
- Used Power BI to create interactive and story-driven visualizations  
- Gained experience in DAX for aggregations and custom KPIs  
- Designed user-centric filters to support personalized discovery  

---

## 🙌 Let's Connect

**Thejaswini H**  
📧 thejaswiniv5@gmail.com  

> _“Data tells stories — this one helps you find yours on the shelf.”_



