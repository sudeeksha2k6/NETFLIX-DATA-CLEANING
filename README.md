# NETFLIX-DATA-CLEANING
**Refining the Netflix dataset for analysis using Python pandas.**
**Objective**__
The goal of this task is to clean and preprocess the Netflix dataset using Python and pandas so that it is ready for analysis.
TASKS DONE:
1. Checked the dataset structure using df.head(), df.info()
2. Checked the number of rows and columns using df.shape
3. Identified and handled missing values in columns: Director, Cast, Country, and Rating, using isnull() in Python.
4. Used df.duplicated().sum() command to check for duplicates. Since the result is np.int64(0), we can say that there are no duplicates. Therefore, .drop_duplicates() was not used.
5. Standardised column names to lowercase with underscores. [.columns = df.columns.str.lower().str.replace(" ", "_")]
6. Converted date formats to a consistent type (e.g., dd-mm-yyyy). [df['date_added'] = pd.to_datetime(df['date_added'], errors='coerce')]
7. Checked and fixed data types.
8. Filled empty cells with appropriate information (unknown, not rated).
9. Extracted useful information such as year_added and numeric duration (DURATION UNIT ALSO ADDED LIKE SEASON OR MINUTES).
    
****Files Included in This Repository**
task1_clean.ipynb → Jupyter Notebook containing the full data-cleaning code

netflix_titles original.csv → Original raw dataset

netflix_cleaned.csv → Final cleaned dataset ready for analysis

screenshots/ → Images showing important outputs after cleaning

README.md → Description of the task and work done

**TOOLS USED**
Python
Pandas
Jupyter Notebook

**Outcome**
The dataset was successfully cleaned, missing values were handled, formats were standardized, and the final data is now ready for exploratory data analysis.
