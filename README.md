# Challenge 1

# Purpose
This analysis was to show the success versus failure rates for kickstarter theater campaigns by month. By looking at trends it may be able to highlight if certain times of the year are more likely to result in a sucessful campaign or not.

# Analysis
*Based On Launch date*
A pivot table and pivot chart were used to examine the data. The number of successful, failed, and canceled campaigns were tallied by each month of the year in the pivot table. The table could be sorted by parent category or year. For this particular set, parent category was selected as Theater.

![Capture1](https://user-images.githubusercontent.com/82550431/135974796-73265b9a-3467-4d69-9037-345798a2dafd.PNG)

The chart above shows that May has the highest number of success. June and July are also months with high numbers of success. This was not due purely to a higher number of campaigns because the number of failures remained similar to other months. The month with the lowest number of success was December, and it is similar to the number of failures.

*Based On Goals*
![Capture2](https://user-images.githubusercontent.com/82550431/135975061-07e7fea0-18c6-4ba1-a720-02efea9ba346.PNG)

For the goal based analysis, the countifs command was used to look at the number of successful, failed, and canceled campaigns in certain goal ranges, and focused only on the subcategory plays. This information was plotted in a line graph to show how the percent of successes and failures changed as the goal amount increased. 

# Challenges & Diffculties
Ensuring the counfifs formula had or the correct parameters and finding a simple way to duplicate it for all the combinations.
When using the Countifs function, to compare one cell to another the syntax is "=" &CELL is needed, which is different than just "=1000" or "=successful" used for constant parameters. Using the cell command allows copying the cells for failed and canceled without having to manually update the formula for each.

# Results
* Two conclusions on the outcomes based on Launch date
  1. May has better success, as well as June and July
  2. December is the least likely to result in success since the numbers are 50/50
* Conclusion on outcome goals
  1. A campaign goal of less than $5000 has a higher likelihood of success than other goals. Goals over $45,000 has the least likelihood of success based on past campaigns.
* Limitations on this dataset
  1. A campaign goal of less than $5000 has a higher likelihood of success than other goals. Goals over $45,000 has the least likelihood of success based on past campaigns.
* Other tables/graphs that could be created
  1.Looking at the success by month as percent successful per month could help to show months like May and June were more successful as a percent rather than just due to a larger number of campaigns. We could look at a box and whisker plot to see if the campaigns with high goals were outliers.
