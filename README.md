# DATA_VIZ_CHALLENGE



This assignment is broken down into the following tasks:

1- Prepare the data.
in this section:
-We'll run the provided package dependency and import data.Then we will merge the mouse_metadata and study_results DataFrames into a single DataFrame.
-We'll also display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate timepoints.Then we will display the data associated with that mouse ID, and create a new DataFrame where this data is removed. 
-Finally, for this section we'll display the updated number of unique mice IDs.

2-Generate Summary Statistics
In this portion we are tasked to do the following:
-Creating a DataFrame of summary statistics which will include:
*A row for each drug regimen.
*A column for each of the mean, median, variance, standard deviation, and SEM of the tumor volume.

3-Create Bar Charts and Pie Charts
Here we'll:
-Generate two identical bar charts showing the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.
*The first bar chart will be created with the Pandas DataFrame.plot() method.
*The second bar chart will be created using Matplotlib's pyplot method.
-Generate two identical pie charts showing the distribution of female versus male mice in the study.
*The first pie chart with the Pandas DataFrame.plot() method.
*The second pie chart with Matplotlib's pyplot method.

4-Calculate Quartiles, Find Outliers, and Create a Box Plot
In this section,we'll:
-Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. 
-Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens.For this purpose we'll use the following substeps:
*Creating a grouped DataFrame showing the last (greatest) time point for each mouse then Merging this grouped DataFrame with the original cleaned DataFrame.
*Creating a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
*Looping through each drug in the treatment list and locating the rows in the merged DataFrame that correspond to each treatment. Then we'll append the resulting final tumor volumes for each drug to the empty list.
*Determining outliers by using the upper and lower bounds, and then printing the results.
-Using Matplotlib,to generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group and Highlight any potential outliers in the plot by changing their color and style.

5-Create a Line Plot and a Scatter Plot
For this portion we'll 
-Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
-Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.

6-Calculate Correlation and Regression
Finally, we'll
-Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.
-Then we'll Plot the linear regression model on top of the previous scatter plot.
