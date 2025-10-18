# Android-App-Data-Analysis
This project  includes extensive data cleaning on the Google Play Store dataset containing 10,840 mobile applications with 13 original features. The cleaning process addresses common data quality issues including missing values, inconsistent formatting, incorrect data types, and categorical variable standardization.

🛠️ Data Cleaning Steps Performed
1. Data Loading & Initial Exploration
Mounted Google Drive and loaded the dataset

Initial data inspection and understanding of data structure

Identified missing values and data quality issues

2. Column Name Standardization
Converted column names to lowercase

Replaced spaces with underscores

Standardized version-related column names

3. Missing Value Treatment
Rating: Filled missing values with '0' and converted to float

Current Version: Filled missing values with 'Unknown'

Android Version: Filled missing values with 'Unknown'

Type: Filled missing values with 'Unknown type'

4. Text Data Cleaning
Category: Replaced underscores with spaces and converted to title case

Genres: Replaced semicolons with spaces

Current Version: Standardized "Varies with device" to "Unknown"

5. Data Type Conversion & Feature Engineering
Price: Removed '$' symbol and converted to float

Rating: Converted from object to float type

Installs: Removed '+' and ',' characters, converted to integer

Size: Standardized "Varies with device" to "Unknown"

6. Categorical Variable Enhancement
Created review categories:

Most high reviewed app (>100,000 reviews)

High reviewed app (20,000-100,000 reviews)

Average reviewed app (5,000-20,000 reviews)

Low reviewed app (<5,000 reviews)

Created installation categories:

Most downloaded app (>100,000 installs)

High downloaded app (40,000-100,000 installs)

Average downloaded app (7,000-40,000 installs)

Low downloaded app (<7,000 installs)

7. Data Segmentation
Separated dataset into Free Apps (10,039 records) and Paid Apps (800 records)

Maintained data integrity throughout segmentation

📈 Key Features After Cleaning
Clean column names: snake_case formatting

Standardized categorical variables: Consistent naming conventions

Proper data types: Numerical columns as floats/ints, categorical as objects

Missing value handling: Appropriate imputation strategies

Enhanced features: Derived categorical variables for better analysis

🎯 Potential Use Cases
The cleaned dataset is now ready for:

📱 App store analytics and insights

⭐ Rating prediction models

💰 Free vs. paid app performance analysis

📊 Category-wise trend analysis

🎮 Genre popularity studies

🛠️ Technologies Used
Python 3

Pandas - Data manipulation and cleaning

Google Colab - Execution environment

Google Drive - Data storage

📁 Dataset Information
Original Size: 10,840 records × 13 columns

Cleaned Size: 10,840 records × 14 columns

Free Apps: 10,039 records

Paid Apps: 800 records

Missing Values: Completely handled

🚦 Getting Started
Clone this repository

Upload the Google Play Store dataset to your Google Drive

Update the file path in the notebook

Run the cells sequentially to reproduce the cleaning process

📊 Next Steps
This cleaned dataset is now prepared for:

Exploratory Data Analysis (EDA)

Machine Learning modeling

Data visualization

Business intelligence dashboards
