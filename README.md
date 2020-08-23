<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Project: Data Cleaning and Manipulation with Pandas  

## Content
- [Project Description](#project-description)
- [Project Goals](#project-goals)
- [Data Workflow](#data-workflow)
- [Deliverables](#deliverables)



## Project Description  

In this project I received a .csv file which i tryed to manipulate the data so I could clean it and hopefully obtain some insights.
On the Data workflow I will try to describe how I takle the problem.



## Project Goals

During this project i will:
* Learn how to "clean" the data for ploting
* Practice how clean data using vectorized methods.
* Begin to practice basic plotting.

## Data Workflow


First I analyse the shape of the raw data. It had 5992 rows( of records on shark attacks) and 24 columns.
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

checking the data for each colums with dtype fucntion to see how can I manipulate the data

Seams meaningless start cleaning without a purpose.

So I ask myself:

- what kind of meaningfull "stories" could I obtain from the data?

What i would like to know since there wasn't any direction on what is the final porpuse of the cleaning.

so I question myself:

- "Is there a stereotype of victim?, Can I obtain a histogram of attacks related to Age?"
- "Which type of shark has the most attack and fatality?"
- "Does the season make a different on shark attacks?
- "is there a relation between provoked and the Activity?
- "Can I see which areas/countries have more shark-attacks?"

Base on this questions i start the clean the data on the respective columns

<img src="http://www.uptourist.com/wp-content/uploads/2015/05/extreme-cleaner-5-shark-tank-cleaner.jpg" width="400"/>


cleaning steps

- Remove duplicated columns, checking the boolean results when comparing the values.
- Remove columns with a lot of unique values (like names or url links , leave one with the most unique values for index or pivot column
- Strip strings from spaces and uppercases to make better counting types of values
- Create a column for converting and storing  a datetime data for easy manipulating.
- and plot some results to see some outliers 

clearly and for obvious reasons there is more records on the last 100 years.

make more sence to focus on cleaning the recent data for a better analysis.

I decide not to remove any rows with NaN values, because i don´t know the purpose of the cleaning.

## Deliverables


* **A Jupyter Notebook (.ipynb) file: data-wrangling **
* **The raw data in GSAF5.csv file**
* **Mydatacleaning.csv file**
* **A gitignore file**
* **A README.md file**  

