# Module_5_Challenge
 We had to do the following tasks: 
1. Prepare the Data - 

Ran the provided package dependency and data imports, and then merged the mouse_metadata and study_results DataFrames into a single DataFrame.

Checked the number of unique mice IDs in the data, and then checked for any mouse ID with duplicate time points. Displaed the data associated with that mouse ID. Then created a new DataFrame where this data was removed. Used this cleaned DataFrame for the remaining steps.

2. Generate Summary Statistics

Created a DataFrame of summary statistics. 

The summary statistics included:
	1. A row for each drug regimen. These regimen names should be contained in the index column.
	2. A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

3. Create Bar Charts and Pie Charts

Generated two bar charts. Both charts to be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

	a. Created the first bar chart with the Pandas DataFrame.plot() method.

	b. Created the second bar chart with Matplotlib's pyplot methods.

4. Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

	a. Created the first pie chart with the Pandas DataFrame.plot() method.

	b. Created the second pie chart with Matplotlib's pyplot methods.

5. Calculate Quartiles, Find Outliers, and Create a Box Plot

Calculated the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculated the quartiles and IQR, and determined if there are any potential outliers across all four treatment regimens. Use the following substeps:

Created a grouped DataFrame that shows the last (greatest) time point for each mouse. Then merged this grouped DataFrame with the original cleaned DataFrame.

Created a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

Looped through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Appended the resulting final tumor volumes for each drug to the empty list.

Determined outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generated a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlighted any potential outliers in the plot by changing their color and style.


6. Created a Line Plot and a Scatter Plot

Selected a mouse (l509) that was treated with Capomulin, and generated a line plot of tumor volume versus time point for that mouse.

Generated a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

7. Calculate Correlation and Regression

Calculated the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

Ploted the linear regression model on top of the previous scatter plot.
