# Comparing and Visualizing New York Times coverage of Presidents Obama and Trump

# Project Motivation: 
In this project, we used the article search API provided by the New York Times to pull data for articles related to Presidents Obama and Trump. We hope you find the visualization of the data insightful. 

# ETL
The New York Times API provided specific keys on article search. The main keys that this project focuses on: 
* Keywords
* Section
* Date
* Headline
For each of the presidents, we queried a two year period starting from 6 months before office to 18 months post-inauguration. This allowed us to compare the news coverage for the presidents during similar timeframes. Our queries yielded nearly 6000 articles.

# SQL Database Schema
we used SQLAlchemy to construct the schema for the SQL database.

# Overview of the NYT presidential coverage article count 
<p align="center">
  <img src="count_overview.png" title="ArticleCountOverview">
</p>
The total article count per month for each of the presidential candidates are compared in the graph above. President Obama's article count is shown in blue, and President Trump's count is showed in red. This graph allowed us to compare and contrast the numbers of the articles The New York Times covered under each of the presidents, and help us uncover the topics in which NYT had dedicated significant time to cover, for example, the significant spike in President Trump's article count in May and June of 2016 is mainly contributed by the topics based on the president's firing of James Comey, who was the director of the FBI at the time. 

# Article breakdown by presidents
<p align="center">
  <img src="distribution_pie.png" title="Distribution of articles by each president">
</p>
This visual provided us with an overview of the number of articles covered by The New York Times for each of the presidents. The chart showed that out of all the articles that The New York Times has published for each of the presidents, there are 18% more articles covered by the newspaper on President Trump than on President Obama during the same time period. 

# Presidental article topic comparison 
<p align="center">
  <img src="topic_comparison_pies.png" title="sections by each president">
</p>
A side-by-side comparison of the sections in which the articles are covered under. National sections were the dominate sections for both presidents, the Business section is the second highest section for President Obama, while Op-Ed is the second highest for President Trump. 

# Keyword Overview 
These interactive visualizations showed the most popular keywords for each of the president tagged by the New York Times. Each president keywords also featured a drop-down tool that allowed one to examine the top keywords associated with the articles broken down by People, Subject, Organization, and Location. 
<p align="center">
  <img src="keywords_obama.png" title="Obama keywords">
  <img src="keywords_trump.png" title="Obama keywords">
</p>

# Next steps: 
* explore different news sources and their coverage of the two presidents, and how the different agency with different viewpoints differ in how they cover the presidents. 
* expand the news source to include Twitter, which is a less filtered and unedited view of the general public's sentiment on presidential news coverage. 
* Leverage natural language processing to gauge the sentiment score of the newspaper coverage on the presidents by headlines, or by the actual content of the article, and be able to compare our findings on their sentiment scores. 
