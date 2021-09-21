# Web-Scrapping-RT100
Web Scrapping Exercise (in Python) for Top 100 Movies rated on Rotten Tomatoes (RT-100)

## Introduction 
A data scraping exercise was performed in Jupyter Notebook `RT100_analysis.ipynb`. 

The purpose of this exercise is to understand how the critic ratings weigh against audience ratings for the _top 100 films_ 
rated on Rotten Tomatoes and answering the following question:

**_Should critic ratings be the ultimate truth metric for a movie's success rating**_

## Project Walkthrough

The exercise involved multiple steps:
1.	Data Wrangling – Data was scrapped from multiple webpages (Primarily using `BeautifulSoup`)
2.	Data Cleaning
3.	Data Analysis & Visualization

#### Data Wrangling:
Data was scrapped from multiple webpages:
a.	The URLs and rankings for the RT top 100 movies were scrapped from the homepage: [here] (https://www.rottentomatoes.com/top/bestofrt/)
b.	The URLs were used to extract the following information:
* Audience Count
* Audience Score
* Critic Count
* Critic Score
* Box Office Earnings
* The review of the top-rated movie was scrapped off the Roger Ebert Review website

Media Wiki API, `wptools`, was used to access Wikipedia data for the top ranked movie.

#### Data Cleaning
Data was cleaning using various tools available in the pandas library. All the data was combined into a single pandas DataFrame for analysis

#### Analysis and Visualization
Data was analyzed using pandas. A **confidence interval test** was conducted by _bootstrapping_ the data points to answer the question given above.

Multiple exploratory and explanatory visualizations were plotted using:
a.	Matplotlib 
b.	Tableau
