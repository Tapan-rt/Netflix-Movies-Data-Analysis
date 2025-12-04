Netflix Movie Data Analysis Project
Netflix, founded on August 29, 1997, in Scotts Valley, California, by Reed Hastings and Marc Randolph, began as a DVD-by-mail service. Hastings, a computer scientist and mathematician, co-founded the company after being inspired by a hefty late fee from a traditional video rental store. Randolph, a marketing executive, played a pivotal role in shaping Netflix's early user interface and branding. In 2007, Netflix introduced streaming services, allowing subscribers to watch movies and TV shows instantly online. This strategic shift capitalized on the growing internet bandwidth and changing consumer preferences, propelling Netflix into a leading global streaming platform. By 2010, the company began its international expansion, starting with Canada, and by 2016, it was available in over 190 countries. As of 2024, Netflix reported a revenue of nearly $10 billion in the third quarter, with profits reaching $2.4 billion. 
The platform boasts over 283 million paid memberships across more than 190 countries, offering a vast library of TV series, films, and games in various genres and languages. 
Overall, Netflix's evolution from a DVD rental service to a global streaming giant underscores its adaptability and innovative approach in the entertainment industry.

📌 Project Overview
This project focuses on analyzing a Netflix movie dataset containing 9,827 records and 9 key attributes, including release dates, movie titles, overviews, popularity scores, votes, languages, genres, and poster links. Using Python, we performed exploratory data analysis (EDA) to understand the structure of the dataset, identify patterns, and uncover meaningful insights. The analysis includes cleaning the data, examining distributions, and creating visualizations that help explain trends in movie genres, popularity, votes, and release years. The goal is to better understand what types of movies dominate the platform and how viewers engage with them.

📁 Dataset Overview
The dataset was sourced from Kaggle and has	Rows: 9827 - Columns: 9 

🧾 Columns:
Release_Date: The date on which the movie was released

Title: Includes the title of the movie

Overview: The synopsis of the movie.

Popularity: popularity rating of the movie

Vote_Count: count of the votes of the movie

Vote_Average: Average of the vote count

Original_Language: the language of the movie

Genre: movie category according to drama, action, historical, etc.

Poster_Url: link of the movie poster


🔧 Project Workflow
Here’s a step-by-step breakdown of what we do in this project:

1. Data Import
In Jupyter Notebook, we imported the dataset using pandas.

2. 🔍 Data Exploration
Used df.info() to check structure and .describe() for summary statistics. 

Checked for null values and our dataset looks a bit tidy with no NaNs nor duplicated value.

Release_Date column needs to be casted into date time and to extract only the year value. 

3. 🧹 Data Cleaning
Overview, Original_Language and Poster_Url wouldn't be so useful during analysis, so we have dropped them.

Vote_Average better be categorised for proper analysis. So, We have cut the Vote_Average values and made 4 categories: popular, average, below avg, not popular to describe it more using categorize col() function.

Genre column has comma separated values and white spaces that needs to be handled and casted into category. 

We have split genres into a list and then exploded our dataframe to have only one genre per row for each movie.

5. 📊 Conclusion

From the data analysis, we discovered several useful insights about movies on Netflix:

Some genres appear more frequently than others, showing what type of content Netflix releases the most.

Certain genres receive higher vote counts, meaning viewers engage more with them.

The movie with the highest popularity score stands out because many users interacted with or searched for it, and we identified its genre.

Similarly, the movie with the lowest popularity helps show what type of content performs poorly.

By looking at the release dates, we found which year had the highest number of movie releases, showing trends in Netflix’s content growth.

Overall, this analysis helps us understand what kinds of movies do well on Netflix and how viewer preferences change over time.


🛠️ How to Use This Project
1.Clone the repository
git clone [https://github.com/Tapan-rt/Netflix-Movies-Data-Analysis] 


📜 License
MIT — feel free to fork, star, and use in your portfolio.

👨‍💻 About the Author
Tapan Tiwari [tapan.r.tiwari@gmail.com]
