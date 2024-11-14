# Project: Employee Payment Record Management

## Introduction

This project consists of a Python program and an R script to manage employee payment records, including processing employee data, exporting details to a CSV file within a zipped folder, and displaying the data in R. The Python script handles data processing and export, while the R script is designed to unzip the folder and read the CSV file to display the employee data.

## Table of Contents
* 1. Files Included
* 2. Features
* 3. Instructions
* 3. Requirements
* 4. Setup Instructions
* 5. Example Usage

## 1. Files Included
The following files are included in this project:
* Salary_Function_Toye.ipynb: Jupyter Notebook containing the Python code for processing employee payment data, exporting details, and creating a zipped archive.
* Employee Profile.zip: A zipped folder containing individual employee details in CSV format.
* Salary_function_R.R: An R script that unzips the folder and reads the employee details CSV file for display.
* README_2.md: Documentation detailing the project setup, usage, and requirements.

## 2. Features
* Employee Data Processing: The Python code reads employee payment data from a provided CSV dataset, stores data in a dictionary format, and organizes it for easy retrieval.
* Get Employee Details: A function, get_employee_details(name), is provided to retrieve details of a specified employee from the dataset.
* Error Handling: Error handling is implemented to ensure the code runs smoothly, even if data or file issues arise.
* Export and Zip Employee Details: The function export_employee_to_csv(name) exports specific employee details to a CSV file and automatically saves it in a zipped folder named "Employee Profile."
* Data Extraction and Display in R: The R script script.R unzips the "Employee Profile" folder and reads the CSV file, displaying the employee data in a structured format.


## 3. Instructions
#### Python Setup
* 1. Open and Run Salary_Function_Toye.ipynb:
    *Launch Jupyter Notebook and open main.ipynb.
    *The notebook contains all code necessary to process employee data, retrieve specific details, and export records to a zipped CSV file.
* 2. Retrieve Employee Details:
    *Use the function get_employee_details(name) to retrieve a dictionary of employee details by name.
    *Example: get_employee_details("PATRICK GARDNER")
* 3. Export and Zip Employee Details:
    *Use the function export_employee_to_csv(name, df) to export specific employee details to a CSV file and store it within the "Employee Profile" zipped folder.
    *Example: export_employee_to_csv("PATRICK GARDNER", df)
* 4. Error Handling:
    *The code includes checks for missing data or file issues. If an employee is not found, an error message will appear.
    
#### R Setup
* Run Salary_Toye_R.R:
    *Open RStudio (or your R environment) and run Salary_Toye_R.R.
    *The script will unzip the "Employee Profile" folder and read the employee details CSV file for display.
* View Employee Data:
    *The script reads the CSV file using read_csv and displays the content in R, allowing for further data analysis or visualization
    
## 4. Requirements
#### Python Libraries
* pandas: For data manipulation and processing
* os: For directory management and file operations
* csv: For writing data to CSV format
* zipfile: For creating a zip archive

#### R Libraries
* readr: For reading CSV files
* utils: For unzipping files


#### Setup Instructions
* Install Required Python Libraries:
    *Install Python libraries using pip install pandas if they are not already installed.
* Install Required R Libraries:
    *Ensure readr and utils packages are available in your R environment. Install with install.packages("readr") if necessary.


## 5. Example Usage
#### Python Code
#### Retrieve employee details
* get_employee_details("PATRICK GARDNER")
#### Export and zip employee details
* export_employee_to_csv("PATRICK GARDNER", df)
#### R
#### Unzip and display employee data
* source("script.R")
