Boston Listings Data Cleaning and Analysis
Overview

This project focuses on cleaning and preparing a dataset of Airbnb listings in Boston for analysis. The primary objective is to ensure the dataset is accurate, consistent, and ready for further analysis while addressing issues like missing values, outliers, and incorrect data types.
Objectives

    To identify and address inconsistencies and missing values in the Boston Listings dataset.
    To prepare the dataset for future analysis, focusing on key variables such as price, minimum_nights, number_of_reviews, reviews_per_month, and availability_365.
    To document the cleaning process with Python code in a Jupyter Notebook.

Dataset Description

The dataset contains listings of Airbnb properties in Boston and includes the following key variables:

    Neighbourhood: The neighborhood where the property is located (Categorical).
    Room_type: Type of property (e.g., Entire home/apt, Private room) (Categorical).
    Price: Nightly price of the property in USD (Continuous).
    Minimum_nights: Minimum number of nights for booking (Continuous).
    Number_of_reviews: Total reviews received (Continuous).
    Reviews_per_month: Average monthly reviews (Continuous).
    Availability_365: Days the property is available for booking in a year (Continuous).

Cleaning Process
Steps Taken:

    Handling Missing Values:
        Imputed missing values in price with the median to avoid skewness.
        Replaced missing values in reviews_per_month with 0, assuming properties with no reviews have zero reviews.

    Data Type Correction:
        Ensured numerical variables (price, minimum_nights, etc.) are stored as integers or floats.
        Converted categorical variables (Neighbourhood, Room_type) into appropriate data types for analysis.

    Outlier Detection and Handling:
        Detected outliers in numerical columns using Z-scores.
        Visualized outliers with boxplots for price and minimum_nights to ensure accurate detection and treatment.

    Categorical Data Optimization:
        Converted object-type columns to categorical types to improve memory efficiency.

    Duplicate Removal:
        Identified and removed duplicate rows to prevent skewing of results.

    Correlation Analysis:
        Generated a heatmap to examine relationships between numerical variables for insight into potential multicollinearity.

    Dataset Finalization:
        Saved the cleaned dataset in Cleaned_Boston_Listings.xlsx.

Deliverables

    Python Code:
        Assignment 1.ipynb: Jupyter Notebook containing the Python code for cleaning the dataset.
    Cleaned Dataset:
        Cleaned_Boston_Listings.xlsx: The final, cleaned dataset ready for analysis.
    Documentation:
        Detailed cleaning steps documented in Assignment 1_Arafat_Ahmed.docx.

Tools and Technologies

    Python: Used for data cleaning and preparation.
        Libraries: pandas, matplotlib, seaborn, and numpy.
    Jupyter Notebook: For interactive data cleaning and visualization.
    Microsoft Excel: To save and review the cleaned dataset.

Instructions for Use

    1. Clone the repository:
    git clone https://github.com/YourUsername/BostonListingsAnalysis.git
    2. Open the Jupyter Notebook:
    jupyter notebook Assignment\ 1.ipynb
    3. Follow the code in the notebook to clean your dataset or review the steps already taken.

Acknowledgments

This project was completed as part of an assignment for MKT 568 at WPI Business School. Special thanks to the course instructors for guidance and the Inside Airbnb project for the dataset.
