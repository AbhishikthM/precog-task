# Indian Courts Analysis and Classification

## Brief Description

The goal of this project is to preprocess and analyze data related to various court cases in India. In the first stage of the project, we will use pandas and numpy to explore the data and gain insights. In the second stage, we will build a classifier using the Scikit-Learn library to categorize the data into different types based on our analysis.

## Workflow

1. Initialize the project in a JupyterLab notebook with the given directory structure.
2. Load the data for 2018, state keys, and district keys.
3. Merge the 2018 data and district keys, as the state for almost all cases is Maharashtra.
4. Group the data by district names and case counts.
5. Analyze the number of female petitioners and defendants by grouping the data by district names.
6. Visualize the data using seaborn and matplotlib.
7. Merge the `acts_sections` dataframe with the `act_key` dataframe.
8. Identify the top acts according to case count and visualize the results.
9. Create a plot about the tenure duration against the number of judges.
10. Proceed to the next stage by taking the 2010 cases files. A single year is being taken to prevent kernel crashing.
11. Merge the 'disp_name_key' data frame with the 'cases_2010' data frame to get all the names of the dispositions.
12. Drop all unnecessary columns from the data frames.
13. Use the base features as the time taken for the case, the date of filing, and the dist_code. The target output is the disp_name_s.
14. Split the merged data frame into training and testing data sets.
15. Import and initialize the random forest classifier from sklearn.
16. Train the random forest classifier.
17. Use the test data set to predict values, and create classification reports for performance metrics.
18. Use seaborn and matplotlib to visualize the performance metrics.
19. similar steps for taken for a logaritimic regression model from sklearn as well

## Directory Structure

    ├── data
    │   ├── act_key.csv
    │   ├── acts_sections.csv
    │   ├── cases_2016.csv
    │   ├── cases_2017.csv
    │   ├── cases_2018.csv
    │   ├── cases_court_key.csv
    │   ├── cases_district_key.csv
    │   ├── cases_state_key.csv
    │   ├── disp_name_key.csv
    │   ├── judge_case_merge_key.csv
    │   ├── judges_clean.csv
    │   ├── purpose_name_key.csv
    │   ├── section_key.csv
    │   └── type_name_key.csv

## Dependencies

- pandas
- numpy
- sklearn
- matplotlib
- seaborn

## Preprocessing and Exploration

During the preprocessing and exploration, the plots that were made were:
1. Total number of cases per district, along with the number of female petitioners and defendants.
2. Top 10 acts by case count.
3. Distribution of judges' tenure against the number of judges.

## Classification

For the classification problem, features like district code, the time taken for the case to take course, and the date of filing could be used for predicting the disposition of the case. To do this, we will use the CSV file for the year 2010. We chose a single year due to the high number of data points.

First, preprocess the data by dropping columns that are not needed. Some insights with the classification could be that the date of filing could be related to the type of disposition. For example, if a case involves a group involved in a case at the same time, the disposition might be similar.

after the preprocessing is done , the splitting of training and testing sets was done, once the training was started, the kernel kept crashing , hence
the sets were downsapled.

the random forest classifier is imported and initialzed , using the fit function , the model is trained and then using the testing set we can get predicted values , now we can use a classsification report from sklearn metrics for a report on the performance.

then seaborn and matplotlib is used for viasualizing the performance metrics.

the models are saved in the models folder in the repository , they can be loaded in using the joblib library and used for predictions.


