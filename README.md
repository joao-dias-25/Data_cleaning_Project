![IronHack Logo](https://s3-eu-west-1.amazonaws.com/ih-materials/uploads/upload_d5c5793015fec3be28a63c4fa3dd4d55.png)

# Project: Data Cleaning and Manipulation with Pandas

## Overview

The goal of this project is to combine everything you have learned about data wrangling, cleaning, and manipulation with Pandas so you can see how it all works together. For this project, you will start with this messy data set [Shark Attack](https://www.kaggle.com/teajay/global-shark-attacks/version/1). You will need to import it, use your data wrangling skills to clean it up, prepare it to be analyzed, and then export it as a clean CSV data file.

**You will be working individually for this project**, but we'll be guiding you along the process and helping you as you go. Show us what you've got!

## General aproach

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
"can I see which areas have more shark-attacks?"

and plot some results to see some outliers  


cleaning steps




---

## Technical Requirements

The technical requirements for this project are as follows:

* The dataset that we provide you is a significantly messy data set. Apply the different cleaning and manipulation techniques you have learned.
* Import the data using Pandas.
* Examine the data for potential issues.
* Use at least 8 of the cleaning and manipulation methods you have learned on the data.
* Produce a Jupyter Notebook that shows the steps you took and the code you used to clean and transform your data set.
* Export a clean CSV version of your data using Pandas.

## Necessary Deliverables

The following deliverables should be pushed to your Github repo for this chapter.

* **A cleaned CSV data file** containing the results of your data wrangling work.
* **A Jupyter Notebook (data-wrangling.ipynb)** containing all Python code and commands used in the importing, cleaning, manipulation, and exporting of your data set.
* **A ``README.md`` file** containing a detailed explanation of the process followed in the importing, cleaning, manipulation, and exporting of your data as well as your results, obstacles encountered, and lessons learned.  Look [here](https://www.makeareadme.com/) for tips on how to structure a README.md file.






## Suggested Ways to Get Started

* **Examine the data and try to understand what the fields mean** before diving into data cleaning and manipulation methods.
* **Break the project down into different steps** - use the topics covered in the lessons to form a check list, add anything else you can think of that may be wrong with your data set, and then work through the check list.
* **Use the tools in your tool kit** - your knowledge of Python, data structures, Pandas, and data wrangling.
* **Work through the lessons in class** & ask questions when you need to! Think about adding relevant code to your project each night, instead of, you know... _procrastinating_.
* **Commit early, commit often**, don’t be afraid of doing something incorrectly because you can always roll back to a previous version.
* **Consult documentation and resources provided** to better understand the tools you are using and how to accomplish what you want.

## Useful Resources

* [Pandas Documentation](https://pandas.pydata.org/pandas-docs/stable/)
* [Pandas Tutorials](https://pandas.pydata.org/pandas-docs/stable/tutorials.html)
* [StackOverflow Pandas Questions](https://stackoverflow.com/questions/tagged/pandas)
* [Awesome Public Data Sets](https://github.com/awesomedata/awesome-public-datasets)
* [Kaggle Data Sets](https://www.kaggle.com/datasets)
