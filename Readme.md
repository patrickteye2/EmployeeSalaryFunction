# Employee Salary Data Processing — Python & R Notebook

This notebook provides a step-by-step workflow for **searching employee salary data**, exporting the results, and handling data using both **Python** and **R**.


## Features

### Python Section:
- Unzips a dataset file (`.zip`)
- Loads a `.csv` dataset using `pandas`
- Defines a function `employee_function()` to:
  - Prompt for an employee name
  - Search for the employee (case-insensitive)
  - Return:
    - A full row of data (as a table)
    - A salary summary (as a dictionary)
- Exports matched results to a `.csv` file
- Compresses the `.csv` file into a `.zip` archive
- Removes intermediate files to keep the workspace clean

### R Section:
- Unzips the output zip file using `unzip()`
- Reads the extracted `.csv` file using `read.csv()`
- Displays the contents using `head()` or viewing the full table
- Can be extended to perform further analysis in R

## How to Use

1. Run the Python cells from top to bottom.
2. When prompted, enter a valid employee name.
3. View the returned table and salary summary.
4. Review the exported file or process it in R (optional).
5. Use the R cells to unzip and analyze the CSV.

## Example Inputs

- `PATRICK GARDNER`
- `JANE DOE`
- (Employee names must match what's in the `EmployeeName` column of the CSV.)

### Sample Output

table,
{'Name': 'PATRICK GARDNER', 'Salary': 326373.19}

## Notes

- Be sure that `Total.csv.zip` is present in the same folder as the notebook.
- The script will automatically clean up temporary files after zipping.
- You can run this entire workflow inside **Jupyter Notebook** or **JupyterLab**.

---
