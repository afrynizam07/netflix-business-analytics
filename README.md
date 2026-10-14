# 🎬 Netflix Business Analytics

Exploratory data analysis of **8,790 Netflix titles** covering the content portfolio, global markets, audience segments, and growth trends, built with Python.

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)

## 📌 Project Overview

This project was completed during my **Business Analytics internship at Auspify Technologies** (remote, October 2026). The goal was to turn raw catalogue data into clear, business-focused insights across four tasks:

1. **Content Portfolio:** Movies vs TV Shows
2. **Global Market Performance:** where content comes from
3. **Audience Segmentation:** what audiences the catalogue serves
4. **Growth & Trends:** how the library has evolved over time

> Note: "performance" here means the number of titles available. The dataset contains no viewership data.

## 🛠️ Tools & Techniques

- **Python**: data cleaning and analysis
- **pandas**: date conversion, feature engineering, grouping, cross-tabulation
- **matplotlib & seaborn**: data visualisation
- **Google Colab**: notebook environment

## 🧹 Data Preparation

- Checked for nulls and duplicates (none found)
- Converted `date_added` from text to a real date and extracted `year_added`
- Split `duration` into a number and unit (minutes for movies, seasons for TV shows)
- Relabelled the placeholder "Not Given" as "Unknown" (287 countries, 2,588 directors)
- Grouped ratings into audience segments: Kids, Teens & Family, Adults, Unrated

## 📊 Key Findings

### Task 1: Content Portfolio
- **Movies dominate:** 6,126 of 8,790 titles (69.7%) are movies, against 2,664 TV Shows (30.3%), about 2.3 movies per TV show.
- **Movies are a standard length:** the average runtime is about 100 minutes.
- **TV shows are short-run:** the average show has 1.75 seasons, and 67% have only one season.

![Content portfolio overview](charts/task1_portfolio_overview.png)

### Task 2: Global Market
- **The US is the anchor market:** 3,240 titles (38.1% of titles with a known country), followed by India (1,057) and the UK (638). Together these three make up 58% of the catalogue.
- **Content is concentrated:** the top 5 countries account for 66% and the top 10 for 78%. Pakistan (421) ranks 4th, ahead of Canada, Japan and South Korea.
- **Regions:** North America (41.3%), Asia-Pacific (31.1%) and Europe (16.5%) supply about 89% of titles.
- **Momentum differs by market:** Brazil (67% of titles released since 2018), Spain (61%), Pakistan (59%) and Mexico (55%) have the most recent catalogues, while India (30%), Turkey (25%) and Egypt (22%) lean on older content.
- **Format differs by market:** South Korea (77% TV) and Japan (66% TV) are TV-led, while India (8% TV) and Nigeria (9% TV) are almost entirely movie-led.

![Where Netflix content comes from](charts/task2_market_overview.png)

![Market momentum](charts/task2_market_momentum.png)

### Task 3: Audience Segmentation
- **Adults are the largest segment:** 45.6% of titles, just ahead of Teens & Family (43.2%). Kids content is only 10.3%.
- **Two ratings carry the catalogue:** TV-MA (3,205 titles) and TV-14 (2,157 titles) together make up 61% of everything.
- **Kids content is mostly TV:** 17.4% of TV shows target kids vs only 7.2% of movies.

![Audience segmentation](charts/task3_audience_segments.png)

![Titles by rating](charts/task3_rating_by_type.png)

### Task 4: Growth & Trends
- **Rapid expansion in the 2010s:** titles released per year grew from 192 in 2010 to a peak of 1,146 in 2018 (about 25% compound annual growth). About 71% of the catalogue was released in 2015 or later.
- **Titles added to the platform peaked in 2019** at 2,016, up from just 82 in 2015.
- **The mix is shifting toward TV:** TV's share of titles released rose from 20% in 2010 to 53% in 2021.
- **A caution on recent years:** the drop after 2018 partly reflects the 2021 data cut-off, so it shouldn't be read as a collapse.

![Growth and trend dashboard](charts/task4_growth_dashboard.png)

## 💡 Business Recommendations

1. **Build TV series in India and Nigeria.** Both have large movie catalogues but tiny TV shares.
2. **Invest in fast-growing markets:** Brazil, Spain, Mexico and Nigeria have recent, growing libraries.
3. **Add kids and family movies.** Only 7.2% of movies target children, the thinnest segment.
4. **Refresh older catalogues** in markets such as Egypt and Turkey.
5. **Focus on quality and regional mix,** since additions flattened after 2019.

## 📂 Repository Contents

| File | Description |
|---|---|
| `Netflix_Business_Analytics_Notebook.ipynb` | Full analysis notebook |
| `charts/` | Exported charts used in this README |

## ▶️ How to Run

1. Open the notebook in Google Colab or Jupyter.
2. Upload the dataset (`Dataset.csv`) when prompted.
3. Run all cells (**Runtime → Run all**).

## 👤 Author

**Afry Nizam**: BSc Information Technology student, University of West London
[LinkedIn](https://www.linkedin.com/in/afrynizam) · [GitHub](https://github.com/afrynizam07)
