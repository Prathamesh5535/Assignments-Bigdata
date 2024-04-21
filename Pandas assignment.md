Q1. How do you load a CSV file into a Pandas DataFrame?
 load a CSV file into a Pandas DataFrame using the read_csv() function:

python
Copy code
import pandas as pd

# Load CSV into DataFrame
df = pd.read_csv('file.csv')
Q2. How do you check the data type of a column in a Pandas DataFrame?
 check the data type of a column using the dtype attribute or the dtypes property:

python
Copy code
# Check data type of a column
print(df['column_name'].dtype)
# Or
print(df.dtypes)
Q3. How do you select rows from a Pandas DataFrame based on a condition?
 select rows based on a condition using boolean indexing:

python
Copy code
# Select rows based on condition
filtered_df = df[df['column_name'] > 5]
Q4. How do you rename columns in a Pandas DataFrame?
 rename columns using the rename() function:

python
Copy code
# Rename columns
df = df.rename(columns={'old_name': 'new_name'})
Q5. How do you drop columns in a Pandas DataFrame?
 drop columns using the drop() function:

python
Copy code
# Drop columns
df = df.drop(columns=['column_name'])
Q6. How do you find the unique values in a column of a Pandas DataFrame?
 find unique values using the unique() function:

python
Copy code
# Find unique values
unique_values = df['column_name'].unique()
Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
 find the number of missing values using the isnull() function followed by sum():

python
Copy code
# Count missing values
missing_values = df.isnull().sum()
Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
 fill missing values using the fillna() function:

python
Copy code
# Fill missing values
df['column_name'] = df['column_name'].fillna(value)
Q9. How do you concatenate two Pandas DataFrames?
 concatenate DataFrames using the concat() function:

python
Copy code
# Concatenate DataFrames
concatenated_df = pd.concat([df1, df2])
Q10. How do you merge two Pandas DataFrames on a specific column?
merge DataFrames using the merge() function:

python
Copy code
# Merge DataFrames on specific column
merged_df = pd.merge(df1, df2, on='column_name')
Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
 group data using the groupby() function followed by an aggregation function:

python
Copy code
# Group data and apply aggregation
grouped_df = df.groupby('column_name').agg({'column_name': 'mean'})
Q12. How do you pivot a Pandas DataFrame?
pivot a DataFrame using the pivot() function:

python
Copy code
# Pivot DataFrame
pivoted_df = df.pivot(index='index_column', columns='column_name', values='values_column')
Q13. How do you change the data type of a column in a Pandas DataFrame?
 change the data type using the astype() function:

python
Copy code
# Change data type of a column
df['column_name'] = df['column_name'].astype('new_dtype')
Q14. How do you sort a Pandas DataFrame by a specific column?
 sort a DataFrame using the sort_values() function:

python
Copy code
# Sort DataFrame by column
sorted_df = df.sort_values(by='column_name')
Q15. How do you create a copy of a Pandas DataFrame?
 create a copy using the copy() function:

python
Copy code
# Create a copy of DataFrame
copied_df = df.copy()


Continuing with the answers:

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
 filter rows based on multiple conditions using logical operators like & (and) and | (or):

python
Copy code
# Filter rows based on multiple conditions
filtered_df = df[(df['column1'] > 5) & (df['column2'] < 10)]
Q17. How do you calculate the mean of a column in a Pandas DataFrame?
 calculate the mean of a column using the mean() function:

python
Copy code
# Calculate the mean of a column
mean_value = df['column_name'].mean()
Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
calculate the standard deviation of a column using the std() function:

python
Copy code
# Calculate the standard deviation of a column
std_deviation = df['column_name'].std()
Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
 calculate the correlation between two columns using the corr() function:

python
Copy code
# Calculate the correlation between two columns
correlation = df['column1'].corr(df['column2'])
Q20. How do you select specific columns in a DataFrame using their labels?
select specific columns using indexing with column labels:

python
Copy code
# Select specific columns by labels
selected_columns = df[['column1', 'column2']]
Q21. How do you select specific rows in a DataFrame using their indexes?
 select specific rows using slicing with row indexes:

python
Copy code
# Select specific rows by indexes
selected_rows = df.iloc[2:5]  # Select rows 2 to 4
Q22. How do you sort a DataFrame by a specific column?
 sort a DataFrame by a specific column using the sort_values() function:

python
Copy code
# Sort DataFrame by a specific column
sorted_df = df.sort_values(by='column_name')
Q23. How do you create a new column in a DataFrame based on the values of another column?
 create a new column based on the values of another column using assignment:

python
Copy code
# Create a new column based on another column
df['new_column'] = df['column_name'] * 2
Q24. How do you remove duplicates from a DataFrame?
 remove duplicates using the drop_duplicates() function:

python
Copy code
# Remove duplicates from DataFrame
df = df.drop_duplicates()
Q25. What is the difference between .loc and .iloc in Pandas?

.loc: It is used for label-based indexing, which means you specify row and column labels explicitly.
.iloc: It is used for integer-based indexing, where you specify row and column positions by integer index.