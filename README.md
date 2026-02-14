Lab 3 about EDA:
What does the data represent?
Are there missing values?
Are there outliers?
What patterns exist?
Which variables influence others?

here,the functions that are being used for future purpose(as a reminder) for the future model: 


1-  df.head()

Purpose:
Displays the first 5 rows of the dataset.

Explanation:
Used to preview the dataset structure and verify it loaded correctly.
note : u can put -1 to show all rows (note from the dr aftab).

2-
df.columns

Purpose:
Shows all column names.

Explanation:
Used to check available variables before analysis.

3-
df.groupby()

Purpose:
Groups data based on a categorical column.

Example:

df.groupby('address')

4-.mean()

Purpose:
Calculates the average of numeric values.

Example:

df.groupby('address')['G3'].mean()

5-.sort_values()

Purpose:
Sorts results in ascending or descending order.

Example:

.sort_values(ascending=False)

6-plt.figure()

Purpose:
Creates a new plot with specified size.

Explanation:
Used to define plot dimensions.

7-.plot(kind='bar')

Purpose:
Creates a bar chart.

Explanation:
Visualizes comparison between categories.

8-plt.title()

Purpose:
Adds a title to the plot.

9-plt.figure()

Purpose:
Creates a new plot with specified size.

Explanation:
Used to define plot dimensions.

10-.plot(kind='bar')

Purpose:
Creates a bar chart.

Explanation:
Visualizes comparison between categories.

11-plt.title()

Purpose:
Adds a title to the plot.

12-plt.ylabel() / plt.xlabel()

Purpose:
Labels the axes of the plot.

13-plt.show()

Purpose:
Displays the final plot.
