Matplotlib Challenge:

Challenge/Task:
1. Three osbervable trends
2. Identify mice with duplicate timepoint and remove duplicate data
3. Create a clean data set 
4. Generate Summary Statistics
5. Generate Bar & Pie Charts
6. Calculate Quartiles, Outliers, and Create Boxplots
7. Create Line & Scatter Plots

Three osbervable trends:
1. Drug regimen of Capomulin & Ramicane have the most number of mice to be put under experiment, and mice are selected between male & 
   female evenly. 
2. The Line Chart of 'Capomulin Treatment Stats for Mouse b128' indicates that the experiment of using drug Capomulin is a 
   successful experience as the tumor volume has decreased by 7mm3 by the end of the experiment. Although the tumor appears to 
   grow larger at Day 5; however, the size of the tumor decreases gradually for the rest of the experiment timepoint. 
3. The correlation between Mouse Weight & Average Tumor Volume is 0.84 which is a fairly strong positive relationship. When the mouse 
    weights grows, the tumor also increases. 


Process for running script:
2. Identify mice with duplicate timepoint and remove duplicate data
    - Read the mouse data and the study results
    - Combine the data into a single dataset
    - Checking the number of mice
    - Getting the duplicate mice by ID number that shows up for Mouse ID and Timepoint
    - Get all the data for the duplicate mouse ID
    - Remove duplicate mice from the group

3. Create a clean data set 
    - Creat clean dataframe for clean_study_result & clean_mice
    - Combine clean_study_result & clean_mice dataframes
    - Checking the number of mice in the clean DataFrame

4. Generate Summary Statistics
    - Group by drug regimen data
    - Calculate mean of tumor volume by using groupby & summary statistical method
    - Calculate median of tumor volume by using groupby & summary statistical method
    - Calculate variance of tumor volume by using groupby & summary statistical method
    - Calculate standard deviation of tumor volume by using groupby & summary statistical method
    - Calculate SEM of tumor volume by using groupby & summary statistical method
    - Assemble the results into a single summary dataframe
    - Calculate mean, median, var, std, SEM with aggregation method
    - Rename columns & display final result
    - Set the xlabel and ylabel using class methods
    - Save figure & Display completed bar chart

5. Generate Bar & Pie Charts
    Creating Bar chart with Pandas:
    - Create a group based on the values of drug regimen
    - Count the number for each drug
    - Create a bar chart based off the data of count for each drug
    Creating Bar chart with PyPlot:
    - Create a group based on the values of drug regimen
    - Count the number for each drug
    - Set x_axis range & tick locations
    - Rename xlabel & ylabel
    - Set up xlim range & ylim range
    - Set up display color, size, width, and x_axis label for the bar chart
    - Save figure & Display completed bar chart
    Creating Pie chart with Pandas:
    - Group data based on mouse ID & gender
    - Create a dataframe to count mice by gender
    - Create a pie chart based on gender & formatting the chart
    - Set axis to equal
    - Save figure to the local folder & display final result
    Creating Pie chart with PyPlot:
    - Group data based on mouse ID & gender
    - Create a dataframe to count mice by gender
    - Create label for pie chart
    - Set axis to equal 
    - Create a Pie Chart & formatting the chart
    - Save figure to local folder & display final result

6. Calculate Quartiles, Outliers, and Create Boxplots
    Calculation:
    - Start by getting the last (greatest) timepoint for each mouse
    - Merge this group df with the original dataframe to get the tumor volume at the last timepoint
    - Create a list of four drugs
    - Create a dataframe for all the four drugs
    - Create dataframes for the drug of Capomulin, Ramicane, Infubinol, and Ceftamin
    - Calculate the IQR and quantitatively determine if there are any potential outliers for Capumulin, Ramicane, Infubinol, and Ceftamin
    - Print calcuation results for all four drugs
    Create Box Plot:
    - Generate a box plot of the final tumor volume of each mouse across four regimens of interest
    - Set up boxplot figure size
    - Set up title, xlabel, ylabel names
    - Set up data source & label names for boxplot
    - Save figure & diplay final result

7. Create Line & Scatter Plots
    Line Plot:
    - Select data for mouse b128 which has been put under experiment of taking drug regimen of Capomulin for treatment
    - Collect data for mouse b128 tumor volume
    - Collect data for mouse b128 timepoint
    - Create line plot with data sources & plot formating
    - Set up plot title, xlable, and ylabel
    - Set up plot xlim
    - Add grid onto plot background
    - Save config & display final result
    Scatter Plot:
    - Create data for Capomulin
    - Collect all the data for drug regimen of Capolumin
    - Collect data of average tumor volume vs mouse weight
    - Create a scatter plot with average tumor volume data & weight data & formatting plot
    - Save plot figure & display final result
    Correlation:
    - Collect data for mouse weight & average tumor volume 
    - Calculate correlation between mouse weight & average tumor volume
    Liner Regression Model:
    - Collect data for mouse weight & average tumor volume 
    - Calculate Linear Regression Model
    Equation of Regression:
    - Set up x_values & y_values
    - Calcuate equation of Regression
    Scatter Plot for Regression:
    - Create scatter plot for Regression & formatting plot
    - Set up figure title, xlabel, y-lable and print message of r-squared result
    - Save Regression Scatter figure & display final result

