<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Project: Data Cleaning and Manipulation with Pandas  

## Content
- [Project Description](#project-description)
- [Project Goals](#project-goals)
- [Data Workflow](#data-workflow)
- [Requirements & Deliverables](#requirements-&-deliverables)
- [Mentoring](#mentoring)
- [Presentation](#presentation)
- [Tips & Tricks](#tips-&-tricks)
- [Resources](#resources)

## Project Description  

The goal of this project is to combine everything you have learned about data wrangling, cleaning, and manipulation with Pandas so you can see how it all works together. For this project, you will start with this messy data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). You will need to import it, use your data wrangling skills to clean it up, prepare it to be analyzed, and then export it as a clean CSV data file.


## Project Goals
During this project you will:
* Learn how to "clean" the data for ploting
* Practice how clean data using vectorized methods.
* Begin to practice basic plotting.

## Data Workflow

Is this project i receive a .csv file which i tryed to manipulate the data so i could clean it and hopefully obtain some insights.
throw the next lines i wil try to make a line of thought on how to takle with data.

first I analyse the shape of the raw data it had 5992 rows( of records on shark attacks) and 24 columns.
On the columns a try to understand which kind of data was on each one.

I will in the next step descrive the 24 four columns
(i also quickly check for non values in each colums


    - 1 Case Number           (it seems that the case number is order by date)
    - 2 Date                  ( diferent kind of date type, some records show the the day, some show a year range )
    - 3 Year                  ( seems similar two column date but with the year)
    - 4 Type                  (type of attack provoked , unprovoked)
    - 5 Country               ( it seems to be the country of the attack)
    - 6 Area                  ( it seems to be the region of the attack)
    - 7 Location              (it seems to be location of the attack)
    - 8 Activity              (it seems to be the kind of activity the victim was doing)
    - 9 Name                  (name of the victim)
    - 10 Sex                  (sex gender)
    - 11 Age                  (age) warning: 44,7% of non-values!!
    - 12 Injury               (kind of injury, description?)
    - 13 Fatal (Y/N)          (Fatality)
    - 14 Time                 (time of the attack) warning: 53,6% of non-values!!
    - 15 Species              (shark species) warning: 48,9% of non-values!!
    - 16 Investigator or Source  (investigator name?)
    - 17 pdf                   (a pdf file with the date and a name? )
    - 18 href formula          (the link to a pdf)
    - 19 href                  (another link to a pdf)
    - 20 Case Number.1         (case number seems similar to column 1 "Case Number")
    - 21 Case Number.2         (case number seems similar to column 1 "Case Number")
    - 22 original order        (seems to be the order number of input of the records)
    - 23 Unnamed: 22           (cant see any values) more than 99% non values
    - 24 Unnamed: 23           (cant see any values) more than 99% non values



After my first visualization of the raw data I started to question what can i do with this data, and what kind of cleaning and manipulation should I focus on this project.

checking the data for each colums with dtype to see how can i manipulate the data

Seams meaningless start cleaning without a purpose.

So I ask myself:

- what kind of meaningfull "stories" could I obtain from the data?

What i would like to know since there wasnt any 

"Is there a stereotype of victim?, Can I obtain a histogram of attacks related to Age?"
"Which type of shark has the most attack and fatality?"
"Does the season make a different on shark attacks? (through my first inspection i would need to disgard a lot od data that show me the season/month of attack)
"is there a relation between provoked and the Activity? or is there a more "sensitive" shark who gets triggered more easily?"
"Can I see which areas/countries have more shark-attacks?"

and plot some results to see some outliers 


![extreme cleaning]( http://www.uptourist.com/wp-content/uploads/2015/05/extreme-cleaner-5-shark-tank-cleaner.jpg)



cleaning steps

remove duplicated columns checking the boolean results when comparing
remove columns with only a lot of unique values (like names or url links , leave one with the most unique values for index or pivot column
strip strings from spaces and uppercases to make better counting types of values
create a column for converting a storing datetime data


## Requirements & Deliverables
The **mandatory** requirements that this project needs to satisfy are:
* The project must be planned. That is why creating a Kanban board and readme documentation is important. You can find a template for Trello [here](https://trello.com/b/kImhfE7w/data-projects).
* Your repository must be clean and organized; this means that it must include a *.gitignore* file and a README file and also have a functional file structure.
* Your project must include data from at least 2 different data sources (APIs & web, dataset & APIs, etc.).
* The project needs to be presented within 5 minutes to your colleagues on the day of the presentation.

The **deadline** to turn in the deliverables is Sunday at 23:59.

## Mentoring
The TAs will be your mentors!

Your mentors will:
* Keep track of your project in general terms. Your mentors will be the next people that know more about the project, after you.
* Check if you are following your plan: are you keeping up with your tasks and deadlines? Do you have any obstacles blocking you?
* Help/support you with specific questions.

Your mentors are **not** meant to:
* Know everything.
* Be your managers. You have to be responsible of your own tasks!



## Necessary Deliverables
The following deliverables should be pushed to your Github repo and the link should be submitted via the student portal.

* **A Jupyter Notebook (.ipynb) file**:
The structure should be:
1. Title of the project.
2. Introduction to hypothoses.
3. Data used (sources, limitations, cleaning, etc...)
4. Any analysis and plots created.
5. Any insights derived from your basic analysis.
6. Possible further questions and improvements.
* **A data folder**
* **A ``README.md`` file**  
Look [here](https://www.makeareadme.com/) for tips on how to structure a README.md file.


## Presentation
The presentation time limit is **5 minutes**! Our suggestion is to include at least the following slides in your presentation but feel free to add or remove slides:

* Title of the project
* Team presentation
* Goals of the project
* Data - sources, problems and limitations
* Database - data wrangling/cleaning and database structure
* Organization. Did you follow your workflow plan? Did you add something after starting the project? Did you follow your best practices agreements? Did you think about the risk management?
* Any insights
* Questions you were not able to answer and why
* Learnings

## Tips & Tricks  
* Questions first. Data second.
* Think about the workflow of your analysis BEFORE starting to code.
* You will have more questions than answers. It's not a problem if you can't answer some or any of your questions. Just show us why you couldn't answer them, that itself will be interesting!

## Resources  
### Lists
[AnyAPI](https://any-api.com/)  
[Top 50 Most Popular APIs on RapidAPI](https://blog.rapidapi.com/most-popular-apis/)  
[18 Fun APIs For Your Next Project](https://medium.com/@vicbergquist/18-fun-apis-for-your-next-project-8008841c7be9) 
[reddit datasets](https://reddit.com/r/datasets)
[FiveThirtyEight](https://data.fivethirtyeight.com/)
[FiveThirtyEight on github](https://github.com/fivethirtyeight)
[US Government open data](https://www.data.gov/)

### Some Ideas
[WeatherBit](https://www.weatherbit.io/api)  
[Strava](https://developers.strava.com/docs/reference/)  
[GitHub](https://developer.github.com/v3/)  
[Twitter](https://developer.twitter.com/en/docs.html)  
[LastFM](https://www.last.fm/api)  
[Spotify](https://developer.spotify.com/documentation/web-api/reference/)  
[NYTimes](https://web.archive.org/web/20150325135221/http://developer.nytimes.com/docs/times_newswire_api/)  
[News](https://newsapi.org/docs)  
[Reddit](https://github.com/reddit-archive/reddit/wiki/API)  
[Medium](https://github.com/Medium/medium-api-docs)  
[Twitch](https://dev.twitch.tv/docs/api/reference)  
[IGDB](https://api-docs.igdb.com/)  
[OMDB](http://www.omdbapi.com/)  
[GIPHY](https://developers.giphy.com/docs/)  
[StackExchange](https://api.stackexchange.com/docs)  
[YouTube](https://developers.google.com/youtube/v3/docs/)  
[TheSportsDB](https://github.com/enen92/script.module.thesportsdb)  
[NBA API](https://pypi.org/project/nba-api/)  

### Paper Examples
[Data Analysis with Python](https://medium.com/@williamkoehrsen/data-analysis-with-python-19434f5d6324)  
[The Best Mario Kart Character According To Data Science](https://medium.com/civis-analytics/the-best-mario-kart-character-according-to-data-science-7dfb65d4c18e)  

## Overview

The goal of this project is to combine everything you have learned about data wrangling, cleaning, and manipulation with Pandas so you can see how it all works together. For this project, you will start with this messy data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). You will need to import it, use your data wrangling skills to clean it up, prepare it to be analyzed, and then export it as a clean CSV data file.



