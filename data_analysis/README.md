## Data analysis notebooks for COMM318 _Stories from data_ Final Project

* This folder should contain the a series of Jupyter notebooks you create to do the data analysis.

* __data_analysis__: This folder contains Jupyter notebooks containing data explorations that were used to examine the inital questions of what months and states had high cases/deaths and the relationships between peak searches for COVID-19 symptoms as well as mental health symptoms. Using Google Trends data as well as open COVID-19 data from the web, I examined and analyzed these data in the following notebooks: 

    * __initial_data_exploration_COVID.ipynb__: this notebook includes the initial data exploration and analysis of the 'us_states_cases.csv' which was retrieved from github. 
        * After loading in the data and renaming it as 'covid_df' the notebook:
            * examines the shape of the dataframe, the columns and rows and what they represented
            * grouping the data in different ways to view state specific cases/deaths by month
            * plotting specific states' cumulative cases/deaths over time
            * plotting mean cases and deaths by states and ranking them highest to lowest

    * __initial_data_exploration_symptoms.ipynb__: this notebook includes the initial data exploration and analysis of the '2020_US_daily_symptoms_dataset.csv'
        * After loading in the data and renaming it 'sympdaily_df' the notebook:
            * drops unnecessary symptoms and 'Naan' rows
            * renames columns to make them more readable including mapping on state abbreviations and state regions onto given state columns
            * saving cleaned data as a new csv
            * exploring specific dates and months in the dataset
            * grouping the data by state and month and examining certain state mean symptom searches
            * plotting the state search mean for different symptoms
            * ranking from highest to lowest mean search symptoms by state
            * grouped date and symptoms; plotted them to see national search over time
            * find correlation between symptoms
            * Look at different ways to use data in a story including measurement and internal comparison

    * __COVID_and_symptoms_merged.ipynb__: this notebook merges the data from the "symptoms_clean.csv" and "covidstate_clean.csv" to examine and explore the combined relationships between COVID cases and deaths and symptom searches that include COVID symptom searches as well as mental health symptom search during the COVID-19 era ranging from January 2020-October 2020
    
    * __data_exploration_final.ipynb__: this notebook loads in both the cleaned and updated csv files used in the initial data explorations mentioned above. This notebook loads in the csv files from the 'comm318_F20_Final_Project/data/clean' folder titled 'covidstate_clean.csv' and 'symptoms_clean.csv' and explores the relationship between COVID-19 cases and deaths  in each state compares with Google trend searches for COVID symptoms such as 'cough' and 'fever' as well as mental health symptoms including 'anxiety' and 'depression.' It follows the exploration steps:
            * Analyzes COVID 19 Google Trends symptom search by:
                * ranking mean symptoms 'anxiety' 'depression' 'cough' and 'fever' search by state from highest to lowest
                * plotting individual states with the highest and lowest mean symptoms search 
                * plotting the national average symptom search over time
                * finding correlation between symptom search nationally
            * Analyzes the COVID 19 cases and deaths per state by:
                * ranking the mean cases and deaths by state from highest to lowest
                * plot specific states with the highest and lowest cases and deaths over time
            * Merges the two dataframes of 'symptoms_df' and'covid_df'
                * create 'new_cases' which is the daily incremental increase in COVID cases
                * plot all states for 'new_cases'
                * look at individual states for daily increases in COVID cases
                * find correlations between 'new_cases' and symptoms
                * plot on heatmaps to see which months had the highest relationships between cases and symptom search

                