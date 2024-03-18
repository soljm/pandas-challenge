# Pandas-Challenge
From Module 4: Data Analysis with Python from the Data Analytics Boot Camp by Monash University and EdX.

By implementing skills learnt throughout the module, an attempt at the challenge has been submitted here.
## Contents
- The CSV files given as resources
- Main `.ipynb` file under the **PyCitySchools** folder
## Explanations
### Local Goverment Area (LGA) & School Summary
The two CSV files were turned into DataFrames and merged together. Conditionals were used to determine how many students passed maths and reading.

The `.groupby()` function was used after calculating how many students had passed maths and reading to separate the students into their respective schools. 
### Highest & Lowest Performing Schools (by % Overall Passsing)
Using `sort_values()`, the DataFrame created in school summary was sorted according to the values in `% Overall Passing`. `Ascending=False` was added to get highest to lowest values for the highest-performing schools.

Formatting by `.map()` was done to make the DataFrame neat and easier to read.
### Maths & Reading Scores by Year
Used `.groupby()` to group the merged DataFrame into **school names** and **year**. The calculated the mean and used `.unstack()` to modify the DataFrame to show **year** in the columns instead of as part of the index.
### Scores by School Spending, School Size & School Type
Established the bins using the code provided. The `.groupby()` function was used to group the data according to the values of the bins given. The mean of all relevant columns were calculated in the same step as the values would already be grouped. 

Formatting was done to keep DataFrame neat and easy to read.

## Credits
Credits to my friend, NT, who gave me pointers on the following:
- `.unstack()`
- `.groupby() [[...]].mean().map()` for scores by school spending, which was then implemented in the remaining parts to keep code concise and consistent.

