# Indian courts anaysis and classification



Brief description of the project: the goal of the project is to preprocess the given data that is based on various cases and find insights about the data during the first stage of the project using pandas and numpy. later , a classifier is to be built, which uses the insights from the analysis and prerocessing to categorize the data into different types (this is to be done using the pytorch library)

#workflow of building the project
initially starting the project on a jupyterlab notebook 
the directory structure is given below 
initializing the 2018 year data , the state keys , the district keys 
merging mainly the 2018 and district keys because the state for almost all the cases is maharastra
grouping the district names with the cases counts 
there also seems to be information about the female peititioner and defendants , 
grouping the district names with the sum of the female petitioner and defendants 
using seaborn and matplotlib to visualize the data 


## Directory Structure
├── data
│   ├── act_key.csv
│   ├── acts_sections.csv
│   ├── cases_2016.csv
│   ├── cases_2017.csv
│   ├── cases_2018.csv
│   ├── cases_court_key.csv
│   ├── cases_district_key.csv
│   ├── cases_state_key.csv
│   ├── disp_name_key.csv
│   ├── judge_case_merge_key.csv
│   ├── judges_clean.csv
│   ├── purpose_name_key.csv
│   ├── section_key.csv
│   └── type_name_key.csv

## Dependencies
 pandas,
 numpy,
 pytorch,
 matplotlib,
 seaboarn

## Installation

Describe the installation process for your project.

## Usage

Explain how to use your project.

## Preprocessing and Exploration

Describe the preprocessing steps taken and insights obtained during exploration of the data.

## Classification

Describe the classification problem identified, the steps taken to build the classifier, and the insights obtained.

## Bonus Task

If you have completed the bonus task, describe your findings.

## Contributors

- [Contributor 1](https://github.com/contributor1)
- [Contributor 2](https://github.com/contributor2)

## License

This project is licensed under the terms of the MIT license.
