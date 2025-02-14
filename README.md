Job Matching & Salary Estimation Model
Project Overview

This project aims to help job seekers find the best-matching tech roles based on their skills, experience geographical location and education while providing a salary estimate based on various job-related factors. The model will predict the most suitable job for a user and estimate their expected salary range based on location, qualifications, experience, and company size

Objectives

1. Job Matching: Recommend the best job role based on a user's input (skills, experience, education).
2. Salary Estimation: Predict an estimated salary based on relevant job factors.
3. Automation Risk Assessment: Indicate the likelihood of automation for a suggested job role.

Users will input:

  1.Country & City (for localized salary estimates)

  2.Experience Level (Entry, Mid, Senior)

  3.Qualifications (Diploma, Bachelor's, Master's, etc.)

  4.Skills (Python, SQL, Cloud, etc.)

The model will then output:

  1.The best-matching job title

  2.The predicted salary range

  3.The automation risk associated with the role

Dataset


Name:Job Dataset

Source:Kaggle

Link:https://www.kaggle.com/datasets/ravindrasinghrana/job-description-dataset


It's columns include:
1. Job Id: A unique identifier for each job posting.
2. Experience: The required or preferred years of experience for the job.
     
3.Qualifications: The educational qualifications needed for the job.
  
4. Salary Range: The range of salaries or compensation offered for the position.
     
5.Location: The city or area where the job is located.
  
6.Country: The country where the job is located.
  
7.Latitude: The latitude coordinate of the job location.
  
8.Longitude: The longitude coordinate of the job location.
  
9.Work Type: The type of employment (e.g., full-time, part-time, contract).
  
10.Company Size: The approximate size or scale of the hiring company.
  
11.Job Posting Date: The date when the job posting was made public.
  
12.Preference: Special preferences or requirements for applicants (e.g., Only Male or Only Female, or Both)
  
13.Contact Person: The name of the contact person or recruiter for the job.
  
14.Contact: Contact information for job inquiries.
  
15.Job Title: The job title or position being advertised.
  
16.Role: The role or category of the job (e.g., software developer, marketing manager).
  
17.Job Portal: The platform or website where the job was posted.
  
18.Job Description: A detailed description of the job responsibilities and requirements.
  
19.Benefits: Information about benefits offered with the job (e.g., health insurance, retirement plans).
  
20.Skills: The skills or qualifications required for the job.
  
21.Responsibilities: Specific responsibilities and duties associated with the job.
  
22.Company Name: The name of the hiring company.
  
23.Company Profile: A brief overview of the company's background and mission.


Methodology
1. Data Preprocessing
 
a.Handling Missing Values: Drop missing values in Company Profile

b.Feature Encoding: Convert categorical data (e.g., experience level, job type) into numerical format

c.Feature Scaling: Standardize salary data and Company Size.

2. Model Development
 
  a.Salary Prediction-XGBoost Regressor/Random Forest Regressor

  b.Job Matching - Random Forest Classifier/XGBoost Classifier

3. Model Evaluation
   
  a.Salary Prediction Evaluation: MAE (Mean Absolute Error), RMSE (Root Mean Squared Error)
  
  b.Job Matching Evaluation: Accuracy, F1-score

4.Deployment Plan – Streamlit App

The project will be deployed as an interactive Streamlit web application where users can enter their details and receive:

  1.A recommended job title
  
  2.A predicted salary range
  
  3.An automation risk score

