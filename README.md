# Kickstarting with Excel

## Overview of Project

### Purpose
This data will show you how Louise's play Fever differentiate using data from the kickstarter workbook.
The data was used to get a visualization of the analysis of outcomes based on launch date and outcomes based on goals 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

![](resources/Theater_Outcomes_vs_Launch.png)

With this graph it uses the months from the years bewteen 2009-2017 to show the results of successful, failed, and canceled outcomes.
You can see with this data set that there was a far greater amount of outcomes at 61% being successful, with 36% of the results at failed. The remaining amount of Cancels at 3%. 

### Analysis of Outcomes Based on Goals
![](resources/Outcomes_vs_Goals.png)

The purpose of this data is using a goal with different intervals from less than 1,000 to up to 50,000 and more. This work only shows data from the play from subcategory column in the kickstarter sheet. The line graph shows that lines almost perfectly mirror each other.
### Challenges and Difficulties Encountered
The main problem i got stuck on was the formula for finding the number successful on Outcomes Baseded on Goals chart. In the countifs formula I missed the fact that i had not put in a criteria for the greater than portion. My originial formula looked like ****=COUNTIFS(Kickstarter!$D:$D,">=5000",Kickstarter!$F:$F, "successful","<=9999",Kickstarter!$R:$R, "plays")****

What I needed to add was ****Kickstarter!$D:$D,**** after successful this allows <=9999 to know where to get the data from. 

## Results
By using the outcome from the Outcomes based on goal you will learn that there is a significant drop in success between 45,000 to 49,999. dropping all the way down to 0% from 67% at the goal of 40,000 to 44,999. It also shows that the highest amount of total projects sits at 534 with the goal of 1,000 to 4,999 this outcome has the second highest success rate.

The theater outcomes based on launch date the summer season has the highest amount plays of the year. Another point that no matter month the succes rate is always higher than the failures. Even the lowest amount of plays in december saw a positive amount of successes even though it was only by a bysmal two. Judging from this data the best month to launch would be May with a result of over 50% being successful. 

This data would be improved by adding a column or columns with percentages of each result. All of the plays are successful for every month so with the percentage data we will be able to tell which month has the best success rate. Just because a month has the most successes does not mean it is the most successful month of the year when compared to failures. Using the results we have now i would suggest a stacked bar graph to vizualize those differences.

An improvment to the outcome based on goals would be to delete the cancel data as it is 0 accross the board. With the other information that we have we can already conclude that none of them were canceled.
