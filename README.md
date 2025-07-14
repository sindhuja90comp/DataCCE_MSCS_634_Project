Healthcare Data Analysis - MSCS 634 Project Deliverable 1
Dataset Summary
The dataset consists of 55,500 patient records with 15 attributes including demographic details (Age, Gender, Blood Type), hospital stay information (Date of Admission, Discharge Date, Room Number), financial data (Billing Amount), and medical details (Medical Condition, Medication, Test Results). The data covers a broad range of patients and treatments, providing a comprehensive overview of healthcare service utilization.

Key Insights from Analysis
Age distribution reveals a median age around 52 years with most patients between 35 and 68 years.

Billing Amounts vary widely with a few outliers on both low and high ends, necessitating outlier analysis.

Gender categories required cleaning due to inconsistent labels (e.g., "male", "Male", "m").

Correlation heatmap indicated relationships among numerical variables such as Age, Billing Amount, and Room Number.

Visualizations including histograms and box plots helped uncover data distribution patterns and potential anomalies.

Data Cleaning and Exploration Steps
Loaded dataset and inspected structure with .info(), .head(), and .describe().

Handled missing values in the 'Age' column by imputing median values to maintain data consistency.

Removed duplicate rows to avoid redundant patient records using drop_duplicates().

Standardized categorical data, particularly the 'Gender' column, by trimming spaces and unifying labels to 'Male' and 'Female'.

Stripped whitespace characters from all string columns to prevent inconsistencies.

Conducted exploratory data analysis with histograms, boxplots, and correlation heatmaps to visualize distributions, identify outliers, and understand variable relationships.

Challenges and Solutions
Inconsistent categorical data: Varied gender labels required cleaning using string manipulation and replacements.

Handling missing values: Used median imputation for 'Age' to preserve data integrity without skewing distributions.

Outliers in financial data: Identified via box plots; further steps for outlier treatment are planned for subsequent project phases.

Large dataset size: Efficiently handled 55,500 records in Pandas ensuring smooth preprocessing and visualization.
