# Virtual Machine (VM) Exercises

## 1st VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

Dataset: glassdoor_reviews.csv

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-1-intial.twbx` or `ex-1-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
Initial File: ex-1-initial.pbix

- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-1-sol.twbx` or `ex-1-sol.pbix`
Solution File: ex-1-sol.pbix

#### Learning Objective

Derive sentiment insights from unstructured data, i.e. text, by leveraging the built in Text Analytics ML models.


#### Motivation

In the world of Business Intelligence and Analytics, there is often both structured and unstructured data. New tools, such as Power BI's Text Analytics, make it easier to siphon insights from the latter. This opens up new doors for understanding business performance and opportunities. Sentiment Analysis is one of the more common methods given its impact in understanding customer experiences.


#### Steps to be executed by the student (max 6)

*Each bulleted instruction is a complete sentence that describes a specific task.*

- Step 1: Score the sentiment for each "Feedback" record using the Power BI "Text Analytics" AI feature; choose "Score Sentiment".
	Note: Information about data privacy - important to ensure sensitive data is handled properly to prevent leakage. Power BI provides different privacy levels, each one specifying different degrees of isolation from other data sources.
- Step 2: Change data type for "Score Sentiment" to Decimal Number.
- Step 3: Calculate column called "Sentiment Category", splitting into 3rds, to define Negative (<=0.33), Neutral(>0.33 and <0.66), and Positive (>=0.66).
- Step 4: Build a bar chart using this new field on the x axis and a distinct count of Review Id on the Y axis.
- Step 5: Add a table displaying the "Feedback" column.

#### End goal:

Solution Check: What are the key points of the first note of Feedback within the Neutral bucket?

![image](https://user-images.githubusercontent.com/42221446/132422149-1662bafd-b951-4fa7-8aae-5350e1d0ed84.png)

## 2nd VM Exercise

#### Dataset

- [ ] Add datasets used to the `datasets/` folder

Dataset: glassdoor_reviews.csv

#### Files

- [ ] **Initial**: Add file to the `exercises/`  folder with the name `ex-2-intial.twbx` or `ex-2-intial.pbix`, depending if you are auditioning for a Tableau or Power BI course.
Initial File: ex-1-initial.pbix

- [ ] **Solution**: Add file to the `exercises/`  folder with the name `ex-2-sol.twbx` or `ex-2-sol.pbix`
Solution File: ex-1-sol.pbix

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

