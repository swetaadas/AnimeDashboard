# 🎌 Anime Dashboard Analysis
 
> *Transforming raw anime data into actionable insights — one chart at a time.*
 
---
 
## 📖 Overview
 
The **Anime Dashboard Analysis** project is an interactive data analytics dashboard built on a curated dataset of anime titles spanning multiple seasons from **2021 to 2026**. It consolidates key metrics — popularity, ratings, genres, studios, and seasonal trends — into a single, easy-to-navigate visual interface.
 
The primary purpose of this dashboard is to help anime enthusiasts, content researchers, and industry analysts answer meaningful questions:
 
- Which genres consistently produce the highest-rated anime?
- How does popularity (member count) correlate with critical scores?
- Which studios are the most prolific or highest-rated?
- Are certain seasons (Winter, Spring, Summer, Fall) more competitive than others?
Rather than sifting through thousands of rows manually, the dashboard surfaces these insights instantly through KPIs, slicers, and interactive charts.
 
---
 
## ✨ Features
 
- **Interactive Dashboard** — A fully navigable Excel dashboard with dynamic charts and slicers that update in real time as filters are applied.
- **KPI Tracking** — At-a-glance summary metrics including average rating, total anime count, maximum popularity, and top-rated titles.
- **Multi-Dimensional Filters** — Slice and explore the data by Genre, Year, Studio, and Season independently or in combination.
- **Trend Analysis** — Visual breakdowns of how ratings and popularity shift across years and seasonal cycles.
- **Genre & Studio Comparisons** — Ranked bar charts and pie charts that highlight dominant genres and leading production studios.
- **Popularity vs. Rating Scatter View** — Understand whether the most-watched anime are also the most critically acclaimed.
---
 
## 📂 Dataset
 
The dataset contains approximately **2,500 anime entries** sourced from anime tracking platforms, covering seasonal releases across five years. Each row represents a unique anime title with the following fields:
 
| Column | Description |
|---|---|
| `Anime Title` | The name of the anime series or film |
| `Popularity / Members` | Number of users who have added the title to their list — a proxy for popularity |
| `Rating / Score` | Average community score on a scale of 1–10 |
| `Genres` | Comma-separated list of genres (e.g., Action, Romance, Fantasy) |
| `Studios` | The animation studio(s) responsible for production |
| `Year` | The broadcast year of the anime |
| `Season` | The seasonal slot — Winter, Spring, Summer, or Fall |
 
> **Note:** This dataset is compiled from publicly available anime community data and is intended for educational and analytical purposes. Some entries include multiple genres and/or co-producing studios.
 
---
 
## 🛠️ Tools & Technologies Used
 
- **Microsoft Excel** — Primary platform for data storage, cleaning, analysis, and dashboard creation
- **Pivot Tables** — Used to aggregate and summarize data by genre, studio, year, and season
- **Pivot Charts** — Bar charts, line charts, and pie charts generated from pivot table sources
- **Slicers & Timelines** — Interactive filter controls linked to all charts for seamless data exploration
- **Conditional Formatting** — Applied to highlight top performers and outliers in the dataset
- **Data Cleaning** — Handled inconsistent genre tags, removed trailing commas/spaces from multi-value fields, standardized studio names, and validated score ranges
---
 
## 📊 Dashboard Components
 
### KPIs Tracked
- Total number of anime in the dataset
- Average rating across all titles
- Highest-rated anime title and its score
- Most popular anime by member count
- Total number of unique studios and genres represented
### Visualizations Used
- **Bar Charts** — Top anime by rating; top studios by average score; genre frequency distribution
- **Line Charts** — Rating and popularity trends across years and seasons
- **Pie / Donut Charts** — Genre share and seasonal distribution of releases
- **Scatter Plot** — Popularity (members) vs. Rating (score) correlation
- **Ranked Tables** — Sortable top-N lists for quick reference
### Slicers & Filters
- Genre slicer (multi-select)
- Year slicer (2021–2026)
- Season slicer (Winter, Spring, Summer, Fall)
- Studio slicer
### Timeline
A timeline control is connected to the Year field, allowing users to drag and select specific date ranges for dynamic filtering across all dashboard components.
 
---
 
## 💡 Key Insights
 
Based on the data analyzed in this dashboard, several notable patterns emerge:
 
**Ratings & Popularity**
- Highly popular anime (e.g., *One Piece*, *Jujutsu Kaisen*) do not always have the highest scores — community size and critical reception diverge significantly for mainstream titles.
- Scores cluster heavily between **6.5 and 8.5**, with fewer than 5% of titles scoring above 9.0.
- *Steel Ball Run: JoJo no Kimyou na Bouken* holds one of the highest scores in the dataset at **9.18**, paired with a strong member count.
**Genre Trends**
- **Action** and **Fantasy** are the most frequently occurring genres, dominating both popularity and sheer volume of releases.
- **Drama** and **Romance** titles tend to have more stable, mid-range scores with niche but loyal audiences.
- Niche genres like **Boys Love**, **Villainess**, and **Isekai** have grown significantly in representation from 2021 to 2026.
**Studio Insights**
- **MAPPA**, **David Production**, and **Wit Studio** consistently produce titles with above-average ratings.
- **Toei Animation** leads in member reach due to long-running series like *One Piece* and *Detective Conan*.
- Smaller studios like **Doga Kobo** and **feel.** punch above their weight in terms of average score relative to output volume.
**Seasonal Patterns**
- The **Winter** season hosts the highest number of anime releases in this dataset, particularly for 2026.
- **Fall** seasons historically feature some of the most critically acclaimed titles.
- Spring tends to be a strong season for continuation seasons (sequels and second cours).
---
 
## 🚀 How to Use
 
1. **Open the file** — Download and open `AnimeDashboard.xlsx` in Microsoft Excel (2016 or later recommended for full slicer support).
2. **Navigate to the Dashboard sheet** — Use the sheet tabs at the bottom to switch to the `Dashboard` or `PlatformWiseDashboard` view.
3. **Apply filters** — Click on any slicer button (Genre, Year, Season, Studio) to filter all charts simultaneously. Hold `Ctrl` to multi-select values.
4. **Use the timeline** — Drag the timeline handles to zoom into a specific year range.
5. **Hover for details** — Hover over any chart element to see exact values in a tooltip.
6. **Reset filters** — Click the funnel/clear icon in the top-right corner of each slicer to remove that filter.
> **Tip:** For the best experience, use Excel in full-screen mode and ensure macros/content are enabled if prompted.
 
 
---
 
## ⚠️ Challenges
 
- **Multi-value fields** — Genres and Studios columns contain comma-separated values, making aggregation non-trivial without data transformation. Pivot tables required pre-processing to split and normalize these fields.
- **Inconsistent data formatting** — Several entries had trailing commas, extra spaces, or blank genre tags that needed cleaning before analysis.
- **Scale disparity in popularity** — Member counts range from under 1,000 to over 2.7 million (One Piece), which compresses most titles visually. Logarithmic scaling was considered for scatter plots.
- **Studio co-productions** — Many anime are produced by multiple studios listed together. Attribution to a single studio required a consistent parsing strategy.
---
 
## 🔮 Future Improvements
 
- **Power BI or Tableau migration** — Rebuilding the dashboard in Power BI would enable richer interactivity, DAX-based KPIs, and web publishing.
- **Automatic data refresh** — Connecting to a live API (e.g., MyAnimeList or AniList) to keep the dataset current without manual updates.
- **Sentiment analysis** — Incorporating user review text to complement the numerical score with qualitative insights.
- **Episode count & duration** — Adding runtime data to analyze whether longer series accumulate popularity differently than short-form content.
- **Geographic breakdown** — Mapping which studios and genres are most popular by region or platform.
- **Predictive scoring model** — Using historical data to estimate the expected rating of a new anime based on its genre, studio, and season.
---
 
## ✅ Conclusion
 
The **Anime Dashboard Analysis** project demonstrates how raw, multi-dimensional data can be transformed into a compelling and actionable visual narrative. By combining clean data preparation with thoughtful chart selection and interactive filtering, the dashboard enables users to explore the anime landscape across five years — uncovering trends in genre popularity, studio performance, seasonal patterns, and the nuanced relationship between popularity and quality.
 
Whether you are a casual fan curious about what topped the charts, or a researcher studying content production patterns, this dashboard provides a structured and intuitive entry point into the data.
 
---
 
*Built with 📊 Excel | Data sourced from anime community platforms | 2021–2026*
