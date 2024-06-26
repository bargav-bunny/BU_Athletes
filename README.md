# Performance Analysis of BU Athletes 

This project is aimed at identifying the correlation between admissions data (e.g., test scores and high school GPA) and the performance of student-athletes throughout their careers at BU. This analysis provides the athletics department with some great insights to better understand and support the students they serve.
Below is a guide to the purpose of each notebook and their dependencies.

## Notebook Descriptions

### 1. **dataframe.ipynb**
- **Purpose**: Imports, preprocesses, and cleans data from the Boston University Athletics dataset for the 2022-2023 season.
- **Dependencies**: Requires the Excel file "BU Athletics Data 22-23.csv" at the relative path "../data/BU Athletics Data 22-23.csv".
- **Output**: Cleaned data frame ready for further analysis.

### 2. **HS-college-comp.ipynb**
- **Purpose**: Generates scatter plots to explore baseline questions comparing high school and college performance metrics.
- **Dependencies**: Depends on the dataframe created in `dataframe.ipynb`.

### 3. **GPA-change.ipynb**
- **Purpose**: Creates line graphs to visualize changes in GPA over time.
- **Dependencies**: Requires `dataframe.ipynb` to have been run previously.

### 4. **Major1.ipynb**
- **Purpose**: Produces histograms, line graphs, and box plots for detailed analysis of major-specific data.
- **Dependencies**: Utilizes the data frame from `dataframe.ipynb`.

### 5. **HSGPA-CGPA.ipynb**
- **Purpose**: Generates scatter plots and histograms to examine relationships between high school GPA and college GPA.
- **Dependencies**: Needs the "BU Athletics Data 22-23.csv" file at the path "../data/BU Athletics Data 22-23.csv".

### 6. **Language Impact.ipynb**
- **Purpose**: Produces box plots and histograms to analyze the impact of language on performance.
- **Dependencies**: Requires "BU Athletics Data 22-23.csv" file located at "../data/BU Athletics Data 22-23.csv".

### 7. **extension-df.ipynb**
- **Purpose**: Extends the dataset with new features from annual survey data.
- **Dependencies**: Requires "newFeatures.ipynb" in the same directory and survey data files from three academic years at specified relative paths.
- **Output**: Saves extended data frame to "../data/dataframe_with_extension.csv".

### 8. **Polling_analysis.ipynb**
- **Purpose**: Analyzes correlations of new features from the extended dataset.
- **Dependencies**: Depends on the extended data frame from `extension-df.ipynb`.

### 9. **feature-selection.ipynb**
- **Purpose**: Visualizes feature correlations and importance within the extended dataset.
- **Dependencies**: Requires `extension-df.ipynb` to be run beforehand.

### 10. **admission-data-by-gender.ipynb**
- **Purpose**: Displays box plots by gender for the final output of the extension project.
- **Dependencies**: Needs the initial data frame from `dataframe.ipynb`.

### 11. **Regression Analysis.ipynb**
- **Purpose**: Performs regression analysis and graph generation for the mini-extension project.
- **Dependencies**: Depends on "../data/dataframe_with_extension.csv" from `extension-df.ipynb`.

### 12. **.ipynb_checkpoints/newFeatures-checkpoint.ipynb**
- **Purpose**: Generates bar plots related to the main extension project.
- **Dependencies**: Relies on the data frame from `dataframe.ipynb`.

### 13. **GPA_prediction.ipynb**
- **Purpose**: Trains, tests, and validates a model for GPA prediction based on extended dataset features.
- **Dependencies**: Uses "../data/dataframe_with_extension.csv" generated by `extension-df.ipynb`.
