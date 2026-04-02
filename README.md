# Tasks Performed

1. Data Quality Issues
Checked data types, missing values, and duplicate records.
Identified that user_id is an identifier column and should not be treated as an analytical feature.

2. Handling Missing Values
Since the dataset originally had no missing values, artificial missing values were introduced in the hours_per_week column for demonstration.
These values were handled using mean imputation, which is suitable for numerical data.

3. Outlier Detection
Used the IQR (Interquartile Range) method to detect outliers in hours_per_week.
The results showed no significant outliers, so no major removal was required.

4. Normalization
Two normalization techniques were applied to the numerical features:

Min-Max Scaling (range between 0 and 1)
Z-score Standardization (mean = 0, standard deviation = 1)

5. PCA (Principal Component Analysis)
The correlation between the numerical features was checked before applying PCA.
The correlation between hours_per_week and completion_rate_percent was very weak, which means PCA was not necessary for this dataset, although it was still applied for demonstration purposes.

# Tools and Libraries
Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn
# Final Results
Checked and confirmed the dataset structure and data types
Demonstrated handling of missing values using mean imputation
Detected no major outliers in hours_per_week
Scaled numerical features using Min-Max and Z-score normalization
Showed that PCA was not strongly needed due to weak correlation between features
