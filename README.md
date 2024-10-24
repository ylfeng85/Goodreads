# Goodreads

## Project Objective

This project analyzes Goodreads publications over several years. Using Tableau for visualization and data analytics, we will explore factors influencing popularities of publications, author and publishers of publications, and seasonal and historical trends. 

## Objectives

The primary objectives of this project are:

1. Analyze Book Popularity Factors:
    - Identify key factors influencing book popularity, such as book type (series/novel) and length.
    - Assess the impact of author popularity on book ratings and reviews.
2. Compare Publisher Outputs:
     - Evaluate the publication output of leading authors and their respective publishers.
     - Analyze the market share of top publishers among the most prolific authors.
3. Investigate Seasonal Trends:
     - Examine the timing of book releases throughout the year and identify peak publication months.
     - Analyze historical trends in publication rates across different years.
4. Generate Strategic Insights:
     - Develop actionable recommendations for publishers to enhance their release strategies based on identified trends and patterns.

## Data Preprocessing 

The dataset was cleaned to address differences in spelling and suffixes in Publisher column to make sure the same variation of Publisher was present for analysis. The publication_year column was split into Month and Year for seasonal trend analysis. The Author column was also cleaned so that there is only one singular author per book title. Two columns were created through feature engineer with by categorizing books according to their num_pages (short, medium, long) and whether the book was a novel, part of a series or a boxed-set collection.  

## Tableau Visualizations

Visit the [Tableau Dashboard](https://public.tableau.com/app/profile/melody.feng/viz/Goodreads_17297441710700/FactorsInfluncingPopularity) to explore the visualizations and insights.

## Key Questions and Insights

### 1. What factors affect a book popularity?

Analysis: I explored the different factors such as book length, book type on the impact of popularity of authors and books.

Visualization: Dashboard made of visualizations including: Rating of Book Types, Book Length Popularity (Pie Chart), Author Popularity (Bubble Chart) and Book Popularity (Bar Chart).

Insight: Series and medium-length books are the most popular genres, with three out of the top five books falling into these categories. The most popular author, J.K. Rowling, is known for her series, Harry Potter. (Popular is defined by number of ratings and the average rating)

<img width="1000" alt="Screenshot 2024-10-23 at 10 08 13 PM" src="https://github.com/user-attachments/assets/9caff592-a60b-42d9-a4ed-08ca18f6522e">

### 2. How does the publication output of the leading publishers compare among the top authors?

Analysis: I compared leading authors and publishers, and the publishers of the leading authors and if that differed from the overall leading publishers. 

Visualization: Top Authors (Bar Chart), Top Publishers (Pie Chart), Top Publishers of Top Authors (Chart)

Insight: Stephen King is the most published author, and Vintage is the leading publisher overall. However, within the top 10 authors, Tor Books contributes 3.54% (20 books) of their publications. This suggests that while Vintage is a top publisher, it may not concentrate on highly prolific authors. This illustrates the different strategies and focuses of various publishers.

<img width="1003" alt="Screenshot 2024-10-23 at 10 08 19 PM" src="https://github.com/user-attachments/assets/88a19fbc-f7c4-4c2c-bc34-85256951858a">

### 3. How do seasonal influences and historical trends in publishing impact the timing of book releases?

Analysis: I evaluated the trends in book publications release timing across the years and months. 

Visualization: Top Months for Publications (Bar Chart), Top Years for Publications (Bubble Chart)

Insight: September ("National Literacy Month") is the peak month for book releases, while December (busy holiday season) sees the fewest. The years 2006, 2005, and the early 2000s marked the highest publication rates, perhaps driven by the popularity of series like Harry Potter and Twilight, which may inspire publishers to release more similar titles.

<img width="1003" alt="Screenshot 2024-10-23 at 10 08 23 PM" src="https://github.com/user-attachments/assets/2500c81f-dca6-4e4f-a0bf-9d0a4b1b4a0e">

## Conclusion and Recomendations 

Based on the insights from this analysis, as a publisher it is valuable to consider:

**1. Leverage Popular Genres:** Invest in developing series and medium-length books, as they are currently the most popular among readers.

**2. Adapt Publication Strategies:** Consider timing releases around September to maximize visibility and engagement, while being mindful of decreased interest in December.

**3. Support Prolific Authors:** Actively seek out and support prolific authors to increase their publication output, as their established fan bases can drive sales and enhance market presence.

**4. Cultivate Author Relationships:** Foster long-term partnerships with prolific authors to encourage consistent output and collaboration on new projects, which can help maintain reader interest and loyalty.

## Dataset

The dataset used in this analysis was scraped from Goodreads via Goodreads API comprising of 11,000 rows.  

### Key Attributes:

- **Book Data:** title, authors, isbn13, num_pages, 
- **Review Data:** average_rating, ratings_amount, text_reviews_count
- **Publication Data:** publisher, publication_date, language_code
- **Sentiment Data:** Sentiment scores derived from review text, common terms used

This project uses Goodread data sourced from [Kaggle](https://www.kaggle.com/datasets/jealousleopard/goodreadsbooks/data).
