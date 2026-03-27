# Day 5 – Pandas CSV I/O & DataFrame Basics

A hands-on Jupyter notebook covering how to read, inspect, and write tabular data using **pandas** and **NumPy** in Python.

---

## Topics Covered

### 1. Reading a CSV File
Load a CSV file into a DataFrame using `pd.read_csv()`. Also covers using a custom separator (e.g. `;`) via the `sep` parameter.

### 2. Inspecting the DataFrame
- `df.head()` — preview the first 5 rows
- `df.describe()` — summary statistics (count, mean, std, min, max, percentiles) for numeric columns. Note: categorical columns are excluded since statistical aggregations don't apply to them.

### 3. Filtering Rows
Boolean indexing to filter rows based on a condition, e.g. `df[df['A'] > 3]`.

### 4. Reading CSV from a String Buffer (`StringIO`)
Use `io.StringIO` to read CSV data directly from a Python string — useful for testing or working with in-memory data without needing a file on disk.

### 5. Selecting Specific Columns (`usecols`)
Use the `usecols` parameter to load only the columns you need, improving memory efficiency.

### 6. Specifying Data Types (`dtype`)
Pass a dictionary to `dtype` to explicitly define the data type for each column (e.g. `np.int64`, `float`, `'object'`).

### 7. Managing Indexes (`index_col`)
- `index_col=0` — set the first column as the row index
- `index_col=False` — force pandas to use the default integer index, ignoring any index-like column in the file

### 8. Handling Escape Characters (`escapechar`)
Use `escapechar` to correctly parse text fields that contain special characters like embedded quotes.

### 9. Saving Data to CSV
Export a DataFrame back to disk with `df.to_csv('output_test.csv')`.

---


