# Data Cleaning in Excel
Certainly! Here's the GitHub README file for the data cleaning process using Excel:

---

# Data Cleaning Process in Excel

This guide outlines the steps for cleaning and standardizing data in Excel. Follow the instructions below to ensure your data is accurate and properly formatted.

## Steps

### 1. AutoFit Columns in "Data" Sheet

1. Right-click on the sheet name “Data” and select `View Code`.
2. In the VBA editor, select `Worksheet` from the dropdown.
3. Enter the following code:
   ```vba
   Cells.EntireColumn.AutoFit
   ```
4. Close the VBA editor.

### 2. Copy Data to a New Sheet

1. Copy all data from the “Data” sheet.
2. Paste it into a new sheet and name it “Clean Data”.

### 3. AutoFit Columns in "Clean Data" Sheet

1. Right-click on the sheet name “Clean Data” and select `View Code`.
2. In the VBA editor, select `Worksheet` from the dropdown.
3. Enter the following code:
   ```vba
   Cells.EntireColumn.AutoFit
   ```
4. Close the VBA editor.

### 4. Remove Duplicates

1. Select all data in the “Clean Data” sheet.
2. Go to the `Data` tab and select `Remove Duplicates`.

### 5. Filter Data and Remove Blank Cells

1. Select all data in the “Clean Data” sheet.
2. Go to the `Data` tab and click on `Filter`.
3. Remove any blank cells from the data.

### 6. Standardize the "President" Column

1. Define a new column and name it “President”.
2. Enter the formula `=PROPER(C2)` in the first cell of the new column (replace C2 with the appropriate cell reference).
3. Drag the fill handle (the “+” sign at the bottom-right corner of the cell) down to fill the column.
4. Copy the entire column and paste it as text into a new column named “President”.
5. Delete the previous two columns used for the “President” data.
6. You can enter formula `LOWER(C2)/UPPER(C2)` according to your need.

### 7. Correct Typing Errors

1. In the “Party” column, press `Ctrl+F` to open the Find and Replace dialog.
2. Replace “republicans” with “Republican”.
3. Replace “Whig   April 4, 1841  â€“  September 13, 1841” with “Whig”.
4. Replace “Demorcatic” with “Democratic”.

### 8. Remove Additional Spaces in "Vice" Column

1. Define a new column and name it “VicE”.
2. Enter the formula `=TRIM(C2)` in the first cell of the new column (replace C2 with the appropriate cell reference).
3. Drag the fill handle down to fill the column.
4. Copy the entire column and paste it as text into a new column named “Vice”.
5. Delete the previous two columns used for the “Vice” data.

### 9. Set Currency Column Format

1. Select the “Currency” column.
2. Go to the `Home` tab, select `Number` from the dropdown, and set the format to `Number`.

### 10. Format Date Columns

1. For the “Date Update” column:
   - Select the column.
   - Go to the `Home` tab, select `Short Date` format.
2. For the “Date Create” column:
   - Select the column.
   - Go to the `Home` tab, select `Short Date` format.

## Conclusion

Following these steps ensures your data is clean, standardized, and free of errors. This process helps maintain data integrity and improves the quality of your analyses.

---

Feel free to modify and extend the README file as needed for your specific use case.
