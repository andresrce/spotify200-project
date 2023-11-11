# spotify200-project
This README documents the steps followed in conducting an EDA on a Spotify dataset using Python, with a focus on understanding song features, artist nationalities, and temporal trends in music preferences.

# Data Mounting and Initial Setup
Data Source Connection: Utilized Google Colab to connect with Google Drive for data access.

# Data Loading and Preliminary Exploration
Loading the Dataset: Imported the pandas library to load the Spotify dataset.
Initial Data Inspection: Employed canciones.head() to view the first few rows of the dataset.
Dataset Structure: Used canciones.shape to understand the size and canciones.info() for a summary of data types and non-null values.

# Descriptive Statistics
Summary Statistics: Applied canciones.describe() to obtain a statistical summary of numerical features.
# Correlation Analysis
Correlation Matrix: Computed and visualized using seaborn's heatmap to understand relationships between numerical features.
# Nationality and Continent Analysis
Nationality Analysis: Identified the top nationalities present in the dataset using value counts and bar plots.
Continent Analysis: Similarly analyzed continents for the artists in the top 200 songs.
# Artist Analysis
Top Artists: Examined artists with the most occurrences in the top 200, visualized using a bar plot.
# Song Features Distribution
Features Histograms: Analyzed the distribution of various song features such as 'Danceability', 'Energy', etc., using histograms.
# Top 20 Songs Analysis
Ranking and Frequency: Identified and visualized the top 20 songs in the top 200 based on frequency.
# Time Series Analysis
Trend Analysis: Conducted a time series analysis to observe trends over time. This involved converting the 'Date' column to a datetime object and setting it as an index.
Resampling and Aggregating: Resampled the data to a monthly frequency to analyze monthly trends in various song features.
Time Series Plotting: Created time series plots for key features like 'Danceability', 'Energy', etc., to visualize how these have changed over time.

# Linear Regression Models
# Model with Categorical Variables (Dummy Variables)
Dummy Variable Transformation: Transformed top 5 countries and artists into dummy variables for regression analysis.
Model Building: Used statsmodels to build an OLS regression model with these dummy variables.
# Basic Linear Regression Model
Feature Selection and Preprocessing: Selected relevant features and applied robust scaling.
Model Training and Testing: Implemented a linear regression model using sklearn and divided the data into training and testing sets.
