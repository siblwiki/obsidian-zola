
<aside>
🖱️ A process by which **we check that the *variables* that we created for our analysis can be reproduced with the raw data**.

In order to do this, RAs check 15% of the raw data against a file that the analyst created (usually a grad student or Sapna) and recreate any new variables that were created.

</aside>

### 1. Finding data for checking:

Download the data from the Qualtrics survey (if it was run online/MTurk). This is the raw data file. The lab manager or analyst will send you their analysis data.

### 2. Naming the files:

Rename the raw data file with Qualtrics, the study name/number and the date in the title. Example:

```
Qualtrics data_Managing Perceptions Study 1_1.30.2019.xlsx).
```

Rename the analysts file with their name, and all of the other information. Example:

```
Sapna’s data_Managing Perceptions Study 1_1.30.2019.xlsx
```

### 3. Check 15%:

Choose 15% of the responses randomly from the analysis data to check. Make sure to get 2-5 from each condition if it’s a large dataset.

### 4. Highlighting:

If cell values in the raw data file match the corresponding cells in the analyst’s data file, then highlight them green in both files. If the cell value in the raw data file does not match the corresponding cell in the analyst’s data, highlight it red in both files.

### 5. Calculations of computed variables:

When there are variables in the analysis file that are not in the raw data, usually the grad student/Sapna/lab manager will let you know what computations they ran to create them (see step 6 for how to check these variables). These variables are usually at the end of the analysis file and sometime have “_R” in their name.

### 6. Check computed variables:

In order to check computed variables, you will need to replicate the calculations that the analyst made using the raw data file. This requires adding variables to your raw data and then reverse coding/averaging/changing values from other variables in this file to make them match up.

Some common computations are:

**Reverse coding:** Flipping all of the values on a 7-point Likert scale to the other end of the scale (e.g., 1s changed to 7s, 2s changed to 6s, 3s changed to 5s, etc.)

**Recoding race and gender variables:** This could involve changing numeric values to text (e.g., “1” changed to “African American/Black”, “2” changed to “Asian/Asian American”, etc) or vice versa.

**Computing a filter:** For example, the analyst might have filtered out participants that did not finish the survey, test responses (i.e., 999s), or participants who identified themselves as “Non-Binary”. The filter column would have a “0” to indicate the rows that were filtered out for the analysis.

**Creating a composite variable:** Sometime the analyst will make a variable that is the average of the participants’ responses to 2+ of the questions in the survey. They will let you know which variables they used to compute each composite variable.

### 7. Cross-check raw data and analysis

Check that the total number of responses in both the raw data and the analysis data match up. If the total number is different, try to figure out why

Hint: usually it’s because some of the responses were filtered out.

### 8. Summarizing your data check:

Once both files have been checked and highlighted, you will need to email the lab manager/grad student with a summary of what you found.

The email should include:

1. The total number of rows you checked
2. a list of the variables in the analysis file that were not in the raw data file
3. a summary of how you computed these variables
4. your best guess at why any cells that are highlighted red did not match up across the files.

Example:

```
Hi [lab manager], I checked 15% of the 120 responses (18 responses total) across both files for Follow Your Passions Study 4. All of the data checked out except for one response in the “likelyApply” variable. See below for details.

Response ID: R_jko29nthslhi

Qualtrics data: “likelyApply”= 2,4

Sapna’s data: “likelyApply”= 2

It looks like the participant selected two responses and Sapna decided to use only the first one for her analysis.

I also computed the gender_R, and filter_$ variables using these formulas:
    gender_R: 1 - “Man”, 2 -“Women”, 3 – “Non-Binary”, 4 – “Unsure”
    filter_$BB: It looks like all of the participants that selected “1” for the consent variable have a “0” in the filter_$ variable. My guess would be that these participants were excluded because they did not consent.
```

### 9. Report:

Let your lab manager/supervisor know if you notice anything strange. Even if it seems small, it could be a big issue later on if not corrected!