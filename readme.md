# Mid Bootcamp Project: Bestseller books on Amazon 2009-2019

# Questions:

1. Is there consistency in the bestselling books during the decade?
2. Which book is the most durable?
3. Which actor is the best seller?
4. Evolution of genres
5. Is price any relevant?
6. Distribution of ratings, reviews and pricing
7. All time top rating (20)

---

# About the Dataset

Dataset on Amazon's Top 50 bestselling books from 2009 to 2019. Contains 550 books, data has been categorized into fiction and non-fiction using Goodreads.

# General observations

- Data was scrapped from amazon site. Primary source: [https://www.amazon.com/-/es/gp/bestsellers/2014/books/ref=zg_bsar_cal_ye?language=en_US](https://www.amazon.com/-/es/gp/bestsellers/2014/books/ref=zg_bsar_cal_ye?language=en_US)
- The dataset includes 550 entries, matching the 50 best-selling books across 11 years (2009 - 2019).
- We infer that the ranking of each book in a year is based on its sales. The way web scrappers work is in an orderly manner, so its position in every year is indeed the order of the ranking → **create a new column called ‘Ranking’ for every year.**
- There are books with the same user rating and quantity of reviews in different years → This means that the same book was in the top50 for more than just one year.
- Throughout the years the same rating and reviews → it gets the reviews and rating from the moment it was scrapped, according to Amazon (if you scrapped it today the dataset would include different data)
- The same book might have different prices along the years. This might be related to book format (hardcover, paperback).
- Currency of the Price column is USD.

# Things to do

1. Data types, table size.
2. Create a column with ID to identificate books more easily
3. Concatenate the genre 2 and genre 3
4. Unique values
5. Look for NaNs, if any, and process them
6. Create data tables per years and create ranking