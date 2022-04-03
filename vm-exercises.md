# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [x] Add datasets used to the `datasets/` folder

**Dataset: glassdoor_reviews.csv**

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.

**Initial File: ex-1-initial.pbix**

- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix`

**Solution File: ex-1-sol.pbix**

#### Learning Objective

Build cohorts, to be used in the final retention visualization, using the customers' first purchase dates.


#### Motivation

Somethings about retention analysis.


#### Steps to be executed by the student (max 6)

*Each bulleted instruction is a complete sentence that describes a specific task.*

- Step 1: Open the workbook `4_1_cohorts.pbix`, then click 'Enable'. Add `Customer ID` and `InvoiceDate` to _Values_ of the _Python visual_.
- Step 2: Import the required packages - pandas, numpy, seaborn, matplotlib.pyplot, and calendar.
- Step 3: Create a new column in the _dataset_ dataframe called _cohort_. 
- Step 4: Find the minimum cohort for each customer and save the results in a new dataframe called _cohortsDF_. Rename the columns to "Customer ID" and "first_cohort".
- Step 5: Count the number of unique customers in each `first_cohort`; rename the columns to "first_cohort" and "num_customers".
- Step 6: Create a bar plot with `first_cohort` (setting as type "string") on the x-axis and `num_customers` as the height value.

#### End goal:

Solution Check: How many customers made their first purchase in December 2009?

![image](FINAL IMAGE INSERT HERE)

## 2nd VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

**Dataset: glassdoor_reviews.csv**

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-2-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.

**Initial File: ex-1-initial.pbix**

- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix`

**Solution File: ex-1-sol.pbix**

#### Learning Objective

Understand common phrases, and their relationship to other variables, from unstructured text data by using Power BI's built-in Text Analytics model.


#### Motivation

Along with understanding sentiment, extracting key phrases and/or words is an important part of text analytics. Simple counts of these terms, or term frequency, provides information on main topics found in a document. Relationships can also be evaluated between terms and other characteristics within the dataset, i.e. sentiment score.


#### Steps to be executed by the student (max 6)

*Each bulleted instruction is a complete sentence that describes a specific task.*

- Step 1: Click on "Transform Data" to open the Power Query editor.
- Step 2: Highlight the "Feedback" column and click "Text Analytics" in the Home banner; choose "Extract Key Phrases".
- Step 3: Build a 100% stacked bar chart using Key Phrases on the x-axis and a distinct count of Review ID on the y-axis.
- Step 4: Add "Attrition" to the legend.
- Step 5: Filter key phrases for those occuring at least five times (i.e. distinct count of review ID >= 5).
- Step 6: Add a table for the Feedback column.

#### End goal:

Solution Check: What percentage of reviews which mentioned "Google" are by people who left the company (i.e. "Attrition = Yes")?

![image](https://user-images.githubusercontent.com/42221446/132422473-f5591420-d8f5-444c-b2eb-a3579424e2b1.png)

