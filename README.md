# Kickstarting with Excel

## Overview of Project

### Purpose
This data will show you how Louise's play *Fever* can be differentiated from the other listed plays utilizing data from the kickstarter workbook.
The data was used to get a graphical visualization of the analysis of *Outcomes based on launch date* as well as *Outcomes based on goals*. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

![](resources/Theater_Outcomes_vs_Launch.png)

This graph uses the months from the years 2009-2017 to show the results of successful, failed, and canceled outcomes.
You can see with this data set that there was a far greater amount of outcomes with 61% being successful, 36% of the results failed, and the remaining at 3% in cancels.

### Analysis of Outcomes Based on Goals
![](resources/Outcomes_vs_Goals.png)

The purpose of this data is using a goal with different intervals from less than 1,000 up to 50,000 and more. This work only shows data from the play subcategory column in the kickstarter sheet. The line graph shows that the percentage successful and percentage failed lines almost perfectly mirror each other; the trends of these lines are correspondent yet conversed.
### Challenges and Difficulties Encountered
The main problem I encountered was with the formula for finding the 'number successful' found in the *Outcomes Based on Goals* chart. In the countifs formula, I kept overlooking the fact that I had not put in a criteria for the greater than portion. My originial formula looked like ****=COUNTIFS(Kickstarter!$D:$D,">=5000",Kickstarter!$F:$F, "successful","<=9999",Kickstarter!$R:$R, "plays")****

What I needed to add was ****Kickstarter!$D:$D,**** after "successful" which allows <=9999 to know where to get the data from. 

## Results
By using the data from the *Outcomes based on goals*, it is shown that there is a significant drop in success between 45,000 to 49,999. When examining the goal of 40,000 to 44,999, the percentage shows a significant decrease, dropping all the way down to 0% from 67%. It also shows that the highest amount of total projects sits at 534 with the goal of 1,000 to 4,999; this outcome has the second highest success rate.

The theater outcomes based on launch date show that the summer season has the highest amount of plays of the year. Additionally, the data is indicative that no matter the month, the success rate is always higher than the failures. This particular observation can be distinguished as the lowest amount of plays in December still saw a positive amount of successes, even though it was only by a bysmal two. Judging from this data, the best overall month to launch would be May with a result of over 50% being successful. 

This data could be improved by adding a column or columns with percentages of each result. All of the plays are successful for every month, so with the percentage data, we would be able to tell which month has the highest success rate. Although one particular month may have the most successes, this does not mean it is the most successful month of the year when compared to failures. Using the results we have now, I would suggest a stacked bar graph to vizualize these differences.

An improvment to the *Outcomes based on goals* would be deleting the cancel data as it is 0 across the board. With the other information that is provided, we can already conclude that none of the plays were canceled.
