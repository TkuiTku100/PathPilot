# Path Pilot Project

## Introduction

Path Pilot is an innovative feature aimed at guiding users, especially those new to the job market, in finding and pursuing a career path that resonates with their skills, interests, and aspirations. Our goal is to demystify the process of career planning by providing personalized recommendations and actionable insights.

This project leverages a diverse dataset from LinkedIn, enriched with data collected through us, and through BrightData web scraping methods, to understand users' backgrounds, skills, and preferences. The core of Path Pilot lies in its ability to suggest career paths, recommend upskilling opportunities, and connect users with resources.

## Getting Started

To get started with the Path Pilot project, you will need to download the files from this repository. Among these files is a Python Notebook designed to run on Databricks, which is central to executing our analysis and generating career path recommendations.

### Prerequisites

Before you can run the notebook, ensure you have the following:

- A Databricks account.
- A working API key from Gemini

### Installation and Setup

1. **Download the Repository**: Click on the "Code" button and download the ZIP file or clone the repository using Git.

2. **Upload Files to Databricks**: Upload the notebook and CSV files to your Databricks workspace.

3. **Insert Your Credentials**: Open the notebook in Databricks. In the first cell, you will need to replace the placeholders with your specific details:
   - `api_key`: Your Gemini API key.
   - `path_to_test_data`: The path to the "data_profiles_test.csv" file.
   - `path_to_scraped_data`: The path to the "urls_and_skills_2.csv" file.
   - `path_to_output`: The path where you want the output to be saved.

Ensure you follow the Databricks documentation for uploading data and running notebooks if you encounter any issues during these steps.

## Project Structure

- `Notebook/`: Contains the Jupyter Notebook to be run on Databricks.
- `profiles_test_data.csv`: Initial user profiles dataset, with answers from personality questionnaire.
- `urls_and_skills_2.csv`: Dataset containing URLs and scraped skills.
- `final_data.csv`: Enhanced profiles_test_data.csv with career goals (from the API) and intermediate positions (from the MML model) included.
- `output.txt`: An example output from one of our notebook runs, showcasing the expected results and format.
- `README.md`: This file, providing an overview and setup instructions.


## Running the Notebook

After setting up your credentials in the notebook:

1. **Execute the Notebook**: Run each cell in the notebook sequentially. The notebook will perform data analysis, model training, and generate career path recommendations based on the input data.

2. **View Results**: The output will be saved to the path you specified in the `OUTPUT_PATH`, and will be printed out in the notebook itself. Review the results to understand the career path recommendations.
