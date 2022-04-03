# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

**Dataset: samplePurchases.csv**

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

- Step 1: Open the workbook `4_1_cohorts.pbix`, then click 'Enable'. Add `Customer ID` and `InvoiceDate` to _Values_ of the _Python visual_, making sure it they are not summarized.
- Step 2: Import the required packages - pandas, numpy, seaborn, matplotlib.pyplot, and calendar.
- Step 3: Create a new column in the _dataset_ dataframe called _cohort_. 
- Step 4: Find the minimum cohort for each customer and save the results in a new dataframe called _cohortsDF_. Rename the columns to "Customer ID" and "first_cohort".
- Step 5: Count the number of unique customers in each `first_cohort`, saving the results as "chart". Rename the columns to "first_cohort" and "num_customers".
- Step 6: Create a bar plot with `first_cohort` (setting as type "string") on the x-axis and `num_customers` as the height value.

#### End goal:

Solution Check: How many customers made their first purchase in December 2009?

![image](https://github.com/jacoma/sme-bi-course-application/blob/python_power_bi/exercises/ex-1-sol.png)

## 2nd VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

**Dataset: samplePurchases.csv**

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-2-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.

**Initial File: ex-2-initial.pbix**

- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix`

**Solution File: ex-2-sol.pbix**

#### Learning Objective

Visualization the percentage of customers who purchased an item N months after their first purchase.


#### Motivation

SOMETHING ABOUT RETENTION


#### Steps to be executed by the student (max 6)

*Each bulleted instruction is a complete sentence that describes a specific task.*

- Step 1: Open the workbook `4_2_retention_heatmap.pbix`, then click 'Enable'.
- Step 2: Add the columns from cohortsDF to the original dataset by merging the two dataframes.
- Step 3: Create a list of unique `cohort` values, called "cohortList". Make sure to use np.sort() before converting to a python list, also called "cohortList".
- Step 4: Calculate the difference in months between the order cohort and the customer's first order for **each row** of the "dataset" dataframe. Save as a new column called `num_months`.
- Step 5: Create a new pivot table of `first_cohort` by `num_months`, using a unique count of the `Customer ID` as the aggregation.
- Step 6: Create a heatmap, including annotations with a percentage format ('.0%').

#### End goal:

Solution Check: What percentage of customers who bought their first product in 12/2009, also bought a product in 4/2010?

![image](<img width="1043" alt="image" src="https://user-images.githubusercontent.com/42221446/161410982-19e4c2a4-9b0f-48cb-924b-6d82ea864b30.png">)

