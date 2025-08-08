# 🎵 Power BI Spotify Music Insights

## Overview
This project applies advanced Power BI techniques to analyze Spotify music streaming data and build a dynamic, app-like music discovery experience. It showcases how rich visual interactivity and DAX logic can be used to explore track-level insights, build recommendation systems, and simulate interactive dashboards.

---

## Objective
To develop an interactive report that surfaces top songs and recommendations by mood or characteristics using advanced Power BI features such as:
- Bookmarks
- DAX-based segmentation
- Drillthroughs
- Page navigation
- Dynamic visuals

This project simulates a lightweight, front-end recommendation engine driven entirely in Power BI.

---

## Tools & Technologies
- Power BI Desktop (.pbix files)
- Spotify Music Dataset (via Kaggle / Spotify API)
- Power Query for data cleaning
- DAX for calculated columns, measures, and dynamic filters
- Power BI service (optional for publishing)

---

## Power BI Concepts Applied
### 🧠 Data Modeling & Calculations
- Star schema with a central `Tracks` fact table linked to `Artists`, `Genres`, and `Dates`
- Custom DAX measures:
  - `Top N Songs by Metric`
  - `Dynamic Ranking by Popularity, Danceability, Energy`
  - `Average by Cluster`
  - Mood/Valence calculation

### 🔁 Interactivity & UX
- **Bookmarks**:
  - Toggle between moods (Chill, Energetic, Acoustic)
  - Simulate button-based navigation
- **Page Navigation**:
  - Back and forth across report pages
  - Replaces tabs with intuitive UX
- **Slicers & Sync**:
  - Global filters (e.g., genre, release year)
  - Slicer sync across pages
- **Drillthrough Pages**:
  - Song-specific drillthrough report
  - Provides detail metrics on acousticness, energy, danceability, valence
- **Custom Tooltips**:
  - Visual tooltips for bar charts and scatter plots with extra song context
- **Dynamic Titles**:
  - DAX-based card visuals that change with slicer selection

---

## Reports Included

### 🎧 `Music.pbix` – Popular Song Insights
- Popularity leaderboard
- Track features overview (scatter + bar + custom KPIs)
- Filterable by genre, artist, year, mood

> 📸 _Insert screenshot: music_insights_main_page.png_

### 📻 `song suggestion.pbix` – Recommendation Engine
- Built entirely with bookmarks, buttons, hidden visuals
- Suggests songs based on mood clusters:
  - Chill (low energy + high acoustic)
  - Energetic (high energy + high danceability)
  - Acoustic (low electronic + high acousticness)
- Full navigation and mood switch simulated using bookmarks only

> 📸 _Insert screenshot: suggestion_dashboard.png_

---

## Business & Technical Value
This project demonstrates how Power BI can:

- Simulate recommendation systems
- Enable lightweight application-like dashboards using bookmarks and page navigation
- Support clustering, filtering, and song mood exploration via UX-centric visuals
- Be applied for music industry data exploration, user behavior tracking, and visual storytelling

---

## Usage Instructions
1. Open `.pbix` file in Power BI Desktop
2. Use genre/year/mood slicers to explore trends
3. Click bookmarks to toggle mood recommendations
4. Hover for custom tooltips or drill into song pages
