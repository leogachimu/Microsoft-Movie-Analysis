# Phase 1 Project Templates and Examples

This repo contains templates and examples to help you get started with your Phase 1 Project. Each of these is in a separate branch as explained below.

- The **template-mvp** branch is the template you should use to for your Phase 1 Project. MVP stands for Minimum Viable Product, but this isn't meant in a negative way - if your project uses this template, it will be functional and accessible.

- The **example-mvp** branch is an example project using the MVP template.

Once you've completed your project using the MVP template, you can improve it using the Above and Beyond (AAB) template if you have time:

- The **template-aab** branch is the AAB template to use to keep improving your project.

- The **example-aab** branch is an example project using the AAB template.

# Phase 1 Project

You've made it all the way through the first phase of this course - take a minute to celebrate your awesomeness!

![awesome](https://raw.githubusercontent.com/learn-co-curriculum/dsc-phase-1-project/master/awesome.gif)

Now you will put your new skills to use with a large end-of-Phase project! This project should take 20 to 30 hours to complete.

## Project Overview

For this project, you will use exploratory data analysis to generate insights for a business stakeholder.

### Business Problem

Microsoft sees all the big companies creating original video content and they want to get in on the fun. They have decided to create a new movie studio, but they don’t know anything about creating movies. You are charged with exploring what types of films are currently doing the best at the box office. You must then translate those findings into actionable insights that the head of Microsoft's new movie studio can use to help decide what type of films to create.

### The Data

In the folder `zippedData` are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMDB](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.org/)
* [The Numbers](https://www.the-numbers.com/)

It is up to you to decide what data from this to use and how to use it. If you want to make this more challenging, you can scrape websites or make API calls to get additional data. If you are feeling overwhelmed or behind (e.g. struggled with the Phase 1 Code Challenge), we recommend you use only the following data files:

* imdb.title.basics
* imdb.title.ratings
* bom.movie_gross

## Deliverables

There are three deliverables for this project:

* A **GitHub repository**
* A **Jupyter Notebook**
* A **non-technical presentation**

Review the "Project Submission & Review" page in the "Milestones Instructions" topic for instructions on creating and submitting your deliverables. Refer to the rubric associated with this assignment for specifications describing high-quality deliverables.

### Key Points

* **Your analysis should yield three concrete business recommendations.** The ultimate purpose of exploratory analysis is not just to learn about the data, but to help an organization perform better. Explicitly relate your findings to business needs by recommending actions that you think the business (Microsoft) should take.

* **Communicating about your work well is extremely important.** Your ability to provide value to an organization - or to land a job there - is directly reliant on your ability to communicate with them about what you have done and why it is valuable. Create a storyline your audience (the head of Microsoft's new movie studio) can follow by walking them through the steps of your process, highlighting the most important points and skipping over the rest.

* **Use plenty of visualizations.** Visualizations are invaluable for exploring your data and making your findings accessible to a non-technical audience. Spotlight visuals in your presentation, but only ones that relate directly to your recommendations. Simple visuals are usually best (e.g. bar charts and line graphs), and don't forget to format them well (e.g. labels, titles).

## Getting Started

Please start by reviewing this assignment, the rubric at the bottom of it, and the "Project Submission & Review" page. If you have any questions, please ask your instructor ASAP.

Next, we recommend you check out [the Phase 1 Project Templates and Examples repo](https://github.com/learn-co-curriculum/dsc-project-template) and use the MVP template for your project.

Alternatively, you can fork [the Phase 1 Project Repository](https://github.com/learn-co-curriculum/dsc-phase-1-project), clone it locally, and work in the `student.ipynb` file. Make sure to also add and commit a PDF of your presentation to your repository with a file name of `presentation.pdf`.

## Project Submission and Review

Review the "Project Submission & Review" page in the "Milestones Instructions" topic to learn how to submit your project and how it will be reviewed. Your project must pass review for you to progress to the next Phase.

## Summary

This project will give you a valuable opportunity to develop your data science skills using real-world data. The end-of-phase projects are a critical part of the program because they give you a chance to bring together all the skills you've learned, apply them to realistic projects for a business stakeholder, practice communication skills, and get feedback to help you improve. You've got this!




# MICROSOFT MOVIE STUDIO BUSINESS ANALYSIS
## PROJECT DONE BY: LEONARD MWANGI GACHIMU

<p align="center"><img src="https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/14d65c79-e38e-4d71-abe6-152fa8756d61" width="608" height="342"></p>

## FILM INDUSTRY OVERVIEW
The US film industry aka Hollywood, is the oldest film industry in the world and also the largest in terms of revenue. In 2019, the box office revenue for the USA and Canada was $11.4 billion, a little over 27% of the worldwide revenue of $42.2 billion.

Research also shows that 14% of American watch movies in cinema halls once a month and 46% of adults watch a movie in a cinema hall at least once a year.

The US cinema industry is expected to grow at a Compound Annual Growth Rate (CAGR) of 8.3% by the year 2027 and these are all indicators of a profitable and growing industry that Microsoft can venture into.

Here's the deal;

Microsoft is not a company that jumps into what everyone else is doing.

There has to be vision, relevant data, analysis of the data, and data-driven strategy.

This is what this report is all about.

## PROJECT OVERVIEW

In this project, I used my data science skills to extract, explore, clean, wrangle, visualize, and interpret the data relevant to helping Microsoft set up a successful movie studio. 

## BUSINESS PROBLEM

Microsoft intends to set up a movie studio but they don't have prior experience in movie production. I was charged with analysing data from the movie industry and developing strategic and actionable insights into the type of films they should produce, the competition, and the talent they should hire. 
                                                              
<p align="center"><img src="https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/187682bb-7c57-4223-b2ea-148343fe2d59" width="540" height="304"></p>
                                                          <p align="center">***Oscar Awards here we come***</p>
                                                          
## PROJECT SCOPE
1. To find out the most popular genres based on the total number of movies produced.
2. To find out the most popular genres based on the IMDB Top 250 Movies.
3. To evaluate content gaps between what every movie studio is producing and the genres that are winning the Top 250 rating.
4. To find out the most profitable genres or genre groups.
5. Competitor analysis of the most profitable movie studios in 2019.
6. To find out the top 15 best-performing movie directors.
7. To find out the top 15 most profitable movie directors.
8. To analyse the correlation between productivity (number of top-rated movies directed) and profitability of a movie director.
   
## THE DATASETS USED
For this project, I used the following datasets:
<ol type="i">
  <li>imdb.title.basics.csv - This dataset was obtained from the IMDb database of all movies in 2019. It contains data about movies and the genres where they fit</li>
  <li>movies.csv - downloaded from [Kaggle](https://www.kaggle.com/datasets/ashishjangra27/imdb-top-250-movies/). This is a list of IMDb's 250 top-rated movies</li>
  <li>bom.movie_gross.csv - A dataset about movie domestic and gross revenue, obtained from Box Office Mojo</li>
  <li>tn.movie_budgets.csv - A dataset about movie production budgets and gross revenue, obtained from The Numbers</li>
  <li>BOM_1000_movies_df - scraped from [Box Office Mojo](https://www.boxofficemojo.com/chart/ww_top_lifetime_gross/?area=XWW/). This is a dataset of 1,000 movies and their box office budgets and worldwide gross revenue</li>
</ol>

## METHODOLOGY
Execution of the project involved the following:
### Data Understanding
I explored the datasets to understand their schema, size, data types, and examine the presence of invalid or inconsistent data such as missing values, duplicates, placeholders, and outliers.
### Data Analysis
I transformed the data into DataFrames using the Pandas library in Python and I performed different transformations and analyses to suit my goals.
### Data Visualization
I used various visualization methods such as bar plots, histograms, and scatter plots to display my findings and facilitate interpretation.
### Data Interpretation
I interpreted the various findings and visualizations to build a recommendation for Microsoft.

## THE FINDINGS
1. I found out that the most popular genres based on the number of movies produced (movie data from IMDb database), include:
   - Documentary
   - Drama
   - Comedy
   - Thriller
   - Horror and
   - Action
     
![Most Popular Genres Based on Number of Movies Produced](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/29d20ac4-2207-43c2-93ee-7be2d386fa02)

2. The most popular genres based on the IMDb Top 250 Movies include:
   - Drama
   - Adventure
   - Crime
   - Action
   - Comedy
   - Mystery
     
![Most Popular Genres Based on IMDb Top 250 Movies](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/c407a0db-d33b-401e-a32d-07d22ae3c356) 

3. The top 250 movies list is the most reliable guide for consumer trends and by plotting the two bar charts on the same figure, we can see Drama is by far the most popular genre but also one of the most crowded. Adventure, Crime, and Action are also popular but are not as crowded as Drama in terms of content.

![Top Genres Based on Number of Movies](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/464ed0be-2148-4e83-84f5-707450e4c140)


4. The top 5 most profitable genres or genre groups are:

<ol type="i">
<li>Action, Adventure & Sci-Fi - approx. $22.05 billion</li>
<li>Adventure, Animation & Comedy - approx. $19.842 billion</li>
<li>Action, Adventure & Fantasy - approx. $7.264 billion</li>
<li>Action, Adventure & Comedy - approx. $5.662 billion</li>
<li>Drama - approx. $5.307 billion</li>
</ol>

![Top 5 Most Profitable Movie Genres](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/ee9ba833-4436-4485-939d-7b34c969f20c) 


5. The top 5 most profitable movie studios are:

<ol type="i">
<li>BV (Buena Vista Studios) - approx. $23.835 billion</li>
<li>Uni. (Universal Studios) - approx. $20.732 billion</li>
<li>Fox Studios - $19.040 billion</li>
<li>WB (Warners Bros) - $13.996 billion</li>
<li>Sony - $12.551 billion</li>
</ol>
 
![Top 5 Most Profitable Movie Studios](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/5c49be67-147c-4dca-a4e7-2dd72ef3bf27) 


6. The most productive movie directors include:

<ol type="i">
<li>Christopher Nolan	- 7 top-rated movies</li>
<li>Steven Spielberg - 7 top-rated movies</li>
<li>Martin Scorsese - 7 top-rated movies</li>
<li>Akira Kurosawa	- 7 top-rated movies</li>
<li>Stanley Kubrick	- 7 top-rated movies</li>
</ol>
   
![Most Productive Directors in IMDb Top 250 Movies](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/cd7494bf-2332-4f71-8716-ecfaf200da86)

7. The most profitable movie directors include:

<ol type="i">
<li>Steven Spielberg - approx. $3.327 billion</li>
<li>Christopher Nolan - approx. $3.195 billion</li>
<li>Peter Jackson - approx. $2.713 billion</li>
<li>Lee Unkrich - approx. $1.446 billion</li>
<li>Anthony Russo - approx. $1.222 billion</li>
<li>Joe Russo - approx. $1.222 billion</li>
</ol>  

![Profit Distribution for Single Movie Directors in IMDb Top 250 Movies](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/bce39aac-af86-4adc-b67c-1baed901d8eb) 


8. The correlation between productivity (number of top-rated movies directed) and profitability of a movie director is about 0.6630.
This indicates a moderate correlation and therefore, there is a moderate likelihood that a director with a high number of movies may direct a movie that realizes a high profit margin.

![Number of Movies Vs Total Profit for Top-Rated Movie Directors](https://github.com/leogachimu/Microsoft-Movie-Business-Analysis/assets/122081776/1d349910-dfb5-413b-a377-2cd2ae33aaaf) 


## CONCLUSION
The box office revenue runs into the billions of dollars and is expected to continue growing at an annual rate of 8.3% up to 2027.

It's evident that some genres are more popular than others, with Documentary, Drama, and Comedy each having more than twice the number of movies in any of the other genres. However, a comparison with the genre distribution among IMDb's Top 250 movies list shows that genres such as Adventure, Crime, and Action are popular but not crowded by producers.

Movies that fit the genres of Action, Adventure & Sci-Fi led the pack with a total profit of about $22.05 billion. Only the first 5 genre groups exceeded $5 billion in total profits, so the dominance of certain genres is evident.

The three most profitable movie studios are BV (Buena Vista Studios), Uni. (Universal Studios), and Fox Studios, each raking in about 20 billion dollars in profits. All studios below position 10 made less than 2 billion dollars (less than 10% of the 2 top ranking studios), which shows the dominance of BV (Buena Vista Studios), and Uni. (Universal Studios).

Some movie directors are more productive and/or profitable than others, but the correlation between productivity and profitability is about 0.6630, indicating a moderate correlation.

## MOVIE STUDIO BUSINESS STRATEGY RECOMMENDATIONS FOR MICROSOFT
1)	Microsoft shouldn’t jump into what everyone is doing, whether they’re succeeding or not.
   
2)	I recommend Drama, Adventure, Crime, Action, and Comedy as the best 5 	genres for Microsoft as a beginner studio.
   
3)	Competitor analysis reveals that the market has a few dominant studios. I, therefore, urge Microsoft to conduct further analysis of these top studios, including their technology, marketing strategies, and SWOT analysis.
    
4)	Further analysis of BV Studio shows that it made an average profit of about $567 million per genre. Microsoft should target at least $600 million per genre.
   
5)	When it comes to hiring the best talent, Microsoft should focus more on hunting down the best director the world can offer and seek their advice on hiring the rest of the team.
   
6)	The correlation between productivity and profitability of a movie is moderate. Microsoft should engage any of the most profitable directors, regardless of the number of movies they have directed.
   
7)	I recommend the following movie directors: Steven Spielberg, Christopher Nolan, Peter Jackson, Lee Unkrich, Anthony Russo, and Joe Russo.

## STUDY LIMITATIONS
1) I could not determine statistically, the correlation between a genre's popularity and its profitability.
   
2) Data about exhibitor rates and distributor rentals was not available, so I computed a movie's profit by simply subtracting the production budget from the worldwide gross revenue.
   
3) I could not scrape the most up-to-date data from some websites because they required costly subscription plans.

4) The home and mobile video entertainment revenue has by far surpassed the box office revenue. However, I could not afford the Statistica data about home/mobile video entertainment.
   
## RECOMMENDATIONS FOR FUTURE ANALYSIS
1) Future studies should come up with a criterion or data for computing a list of the most profitable single genres.
   
2) Analysis should be done on the latest data on home/mobile video entertainment (Over-the-Top Platforms) market.
   
3) Accurate data about exhibitor rates and distributor rentals should be sought, to enable computation of the accurate profit per movie, genre, studio, or director.
   
4) To find the correlation between a movie’s rating on IMDb and other ranking websites such as Rotten Tomatoes and The Numbers.

## PROJECT DELIVERABLES
There are three deliverables for this project:
* A **GitHub repository**
* A **Jupyter Notebook**
* A **non-technical presentation**

