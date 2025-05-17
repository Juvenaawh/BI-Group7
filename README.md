# BI Group 7 – Mini Projects

**Course:** Business Intelligence 
**Group Members:** Kamilla, Jeanette, Juvena

---

## Project Overview

This repository contains an overview of mini projects completed as part of the Business Intelligence course. All projects are developed using **Jupyter Notebooks** and focus on key data science skills including preprocessing, exploration, and visualisation.

---

### MP3 – MACHINE LEARNING FOR ANALYSIS AND PREDICTION

**Folder:** `MP3`

Focus:  
A mini project exploring **COVID death toll**, using Python for data analysis, visualisation and prediction by regression, classification and clustering algorithms.

**Key files:**
- `Covid-MP3.ipynb`

**Datasets Used:**
- `owid-covid-latest.csv`

---

## Tools Used

- Jupyter Notebook  
- Python (pandas, matplotlib, seaborn, etc.)  
- Streamlit (visualisation of data) 
- Collaborative programming

---

## Running the Streamlit App 

The Streamlit is under development — only a basic placeholder is available for now.

To run the Streamlit dashboard locally, follow these steps:

Open Anaconda Navigator
Launch Anaconda and open VSCode from within Anaconda.

Navigate to the Streamlit Folder
In VSCode, open a terminal and make sure you're in the Streamlit directory of the project.

Install Required Packages
In the terminal, run the following command to install all necessary packages:

pip install streamlit

Once dependencies are installed, launch the app with:

streamlit run pages/main.py

This will open a local Streamlit web app in your browser.
You can also run these commands in any other terminal (e.g. Windows Terminal, macOS Terminal) as long as your Python environment is activated.


Which machine learning methods did you choose to apply in the application and why?,
Linear Regression to predict COVID-19 deaths per million based on total cases. This method was chosen because it is good at predicting numbers and tendensies in the data.
Random Forest Classification to classify countries into high or low COVID-19 mortality groups. We chose this method because it is good at classification.
KMeans Clustering to group countries based on total_cases, life_expectancy, and population. we used this method to group the countries so that we could compare countries with similar death rates.

How accurate is your solution of prediction? Explain the meaning of the quality measures.,
Linear Regression had limited accuracy. It explained only 30% of the variation in deaths per million, with an RMSE of 1039, which indicates high average error.
Random Forest Classification achieved 88.1% accuracy, with high precision 0.85 for low mortality and 0.91 for high and a strong overall performance.
Silhouette Score for clustering was 0.53, indicating reasonably good separation between clusters.

What could be done for further improvement of the accuracy of the models?,
We would include more features variables like vaccination rate, healthcare capacity, or government policies that could improve predictions.
maybe more feature engineering, creating new features like cases per hospital bed or something extra that maybe can reveal stronger patterns.
To improve model accuracy, we would like to include more relevant data that could help confirm or disprove our hypotheses. During the project, we noticed that several columns contained many missing or zero values, even though the data could have been important. Having access to more complete and consistent datasets with fewer missing values would likely lead to more reliable models and better predictive performance.

Which were the challenges in the project development?,
One of the main challenges was that the data was skewed due to a few very large countries with extremely high values. This made it difficult to work with outliers, because removing them would mean excluding entire countries. In the end, we decided to keep them and try to work around their influence. Another challenge was the lack of additional features to compare and analyze the data more deeply. For example, our scatter plots could have benefited from more contextual variables to explore different scenarios. We also realized that some of our visualizations could have been more meaningful or useful in terms of insight. 
