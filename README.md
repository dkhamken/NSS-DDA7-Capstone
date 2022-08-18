# An Analysis of Olympic Figure Skating Success by Age and Country

## Table of Contents
+ [Background Info](#background-info)
+ [Motivation](#motivation)
+ [Data Questions & Focus](#data-questions-&-focus)
+ [Data Sources](#data-sources)
+ [Technologies](#technologies)
+ [The Process](#the-process) 
+ [Dashboard](#dashboard)

## Background Info [^1]
<details>
<summary>Here's a little Olympic Figure Skating history lesson for you</summary>
<br>
The Olympic Games is the largest international sports festival in the world. Figure skating was first introduced in the 1908 Summer Olympic Games and moved to become a part of the Winter Olympic Games in 1924. It was one of the first sports with a category for women and the only Winter Olympic sport with women competitors until 1936[^1].  
</details>

## Motivation[^2][^3]
<details>
<summary>Why did I choose to study this topic?</summary>
<br>
  
<details>
<summary>Personal Experience</summary>
<br>
I was a competitive figure skater for over a decade with dreams of going to the Olympics.
</details>

<details>
<summary>Understanding the Olympic Goal</summary>
<br>
  
    - The Olympic Games were created with the ultimate goals to cultivate human beings, through sport, and contribute to world peace.
    - Olympism is a philosophy of life, exalting, and combining in a balanced whole the qualities of body, will, and mind. 
    - Blending sport with culture and education, Olympism seeks to create a way of life based on 
      * joy found in effort 
      * the educational value of good example
      * respect for universal fundamental ethical principles
</details>

<details>
<summary>Recent Controversy</summary>
<br>
  
    - 15 yo Russian skater, Kamila Valieva, favored to win gold at 2022 Beijing Olympics tested positive for an illegal drug; the ISU’s (international skating union) decision to raise the minimum age for qualification to 17 yo was accelerated post scandal, March 2022.
    - Comment from ISU representative following the proposal, *"..we urgently needed to change to protect the physical, mental, and emotional health of athletes.”*
    - Increasing the age minimum to 17 decreases the risk of injury “if training loads are modified during times of rapid growth” and allows skaters to “expand on their social and emotional skill development” according to the proposal. 
</details>
 
</details>

## Data Questions & Focus
  * Which countries have the most successful figure skating training programs that emulate the Olympic goal which could benefit/contribute to the overall health of an athlete? 
  * In the past decade of Winter Olympic games, which countries produced the most successful figure skaters who are of the the new qualification age?
  * In the past decade of Winter Olympic games, which countries may have a need for training program restructuring (countries with athletes under qualification age)?  

## Data Sources
  * [Olympics Results Webpage](https://olympics.com/en/olympic-games/olympic-results)
  * [Athlete Age](https://en.wikipedia.org/wiki/List_of_Olympic_medalists_in_figure_skating_by_age) 

## Technologies
  * Python
    - [Jupyter Notebooks](https://jupyter.org/)
    - [pandas](https://pandas.pydata.org/)
    - [requests](https://pypi.org/project/requests/)
  * [Excel](https://www.microsoft.com/en-us/microsoft-365/excel)
  * [Power BI](https://powerbi.microsoft.com/en-us/)

## The Process
<details>
<summary>Scrape & Clean</summary>
<br>

  * The majority of the work for this project was done using Python (pandas, requests) to scrape the Olympics Results Webpage to find the result of all medalists (women and men) for Figure Skating in all Winter Olympic Games beginning in Chamonix 1924.
    - Scraped the Olympics result page (using 'for loop') to find a list of all Olympic Games
    - Converted list to a dataframe 
    - Isolated dataframe to only show Winter Games
    - Reformatted/cleaned columns to split the City name, Olympic Year, Season (i.e. 'Chamonix 1924, Winter' was split into three different columns for City:'Chamonix', Year:'1924', Season:'Winter), removed unwanted characters, created column to give Olympic City Games name webpage format (i.e. 'chamonix-1924)
    - Converted new column to list, used list to scrape through Olympics Results Webpage to find all Gold, Silver, Bronze medalists
    - Excel was briefly used to reformat some column headers
    - Power BI used to create new columns based on certain conditions 
</details>
 
<details>
<summary>Build & Prepare</summary>
<br>

  * Power BI was used to build dashboards and filters of all the data to analyze which countries had athletes who were of qualification age or older when winning a medal, focusing on the most recent Olympic Games from 2010 to 2022
</details>
   
## Dashboard

## Footnotes
[^1]: [Hall of Fame | Olympic Figure Skating](https://usopm.org/hall-of-fame/figure-skating/#:~:text=Figure%20skating%20is%20one%20of,with%20women%20competitors%20until%201936.)
[^2]: [Beyond the Games](https://olympics.com/ioc/beyond-the-games)
[^3]: [Figure skating proposal to raise age minimum detailed](https://olympics.nbcsports.com/2022/05/02/figure-skating-age-minimum-international-skating-union-isu-proposal/)
