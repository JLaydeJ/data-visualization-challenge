# Pymaceuticals, Inc. Analysis
What good is data without a good plot to tell the story?
Apply what you've learned about Matplotlib to a real-world situation and dataset. 

# Background
You've just joined Pymaceuticals, Inc., a new pharmaceutical company that specializes in anti-cancer medications. Recently, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

As a senior data analyst at the company, you've been given access to the complete data from their most recent animal study. In this study, 249 mice who were identified with SCC tumors received treatment with a range of drug regimens. Over the course of 45 days, tumor development was observed and measured. This study aimed to compare the performance of Pymaceuticals’ drug of interest, Capomulin, against the other treatment regimens.

The executive team has tasked you with generating all of the tables and figures needed for the technical report of the clinical study. They have also asked you for a top-level summary of the study results.

# Prepare the Data
- Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

- Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

- Display the updated number of unique mice IDs.

# Generate Summary Statistics
Create a DataFrame of summary statistics. Remember, there is more than one method to produce the results you're after, so the method you use is less important than the result.

Your summary statistics should include:

- A row for each drug regimen. These regimen names should be contained in the index column.

- A column for each of the following statistics: mean, median, variance, standard deviation, and SEM of the tumor volume.

# Create Bar Charts and Pie Charts
Generate two bar charts. Both charts should be identical and show the total number of rows (Mouse ID/Timepoints) for each drug regimen throughout the study.

- Create the first bar chart with the Pandas DataFrame.plot() method.
  ![pandasbar](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/021a83a0-f17d-4e81-abb2-163e27e79b4c)



- Create the second bar chart with Matplotlib's pyplot methods.
  ![bar](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/1a8c0adb-3884-41be-9052-d018b8404cc4)




Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

- Create the first pie chart with the Pandas DataFrame.plot() method.
  ![pie](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/7766a3df-213a-401f-94a9-44f098069c00)



- Create the second pie chart with Matplotlib's pyplot methods.
  ![pie](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/65528e68-4891-4470-b206-3bee404e7755)



# Calculate Quartiles, Find Outliers, and Create a Box Plot
Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:

- Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.

- Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.

- Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.

- Determine outliers using the upper and lower bounds, then print the results.

Using Matplotlib, generate a box plot that shows the distribution of the final tumor volume for all the mice in each treatment group. Highlight any potential outliers in the plot by changing their color and style.
![outliers](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/af410a51-5b0f-465a-9601-4688989256be)



# Create a Line Plot and a Scatter Plot
Select a single mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.
![line](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/35fb9eca-ab12-403e-8bd3-5539f50da288)



Generate a scatter plot of mouse weight versus average observed tumor volume for the entire Capomulin treatment regimen.
![scatter1](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/de920224-d5ee-4456-aaad-ec484924ad63)



# Calculate Correlation and Regression
Calculate the correlation coefficient and linear regression model between mouse weight and average observed tumor volume for the entire Capomulin treatment regimen.

Plot the linear regression model on top of the previous scatter plot.
![regression scatter](https://github.com/JLaydeJ/data-visualization-challenge/assets/134284646/651cf510-ee19-482b-a211-d79dff129e92)

