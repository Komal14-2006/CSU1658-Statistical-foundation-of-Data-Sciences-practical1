Question 1 — Identify Duplicates Using prof and Compute Age Statistics
Workflow
Check the dataset for duplicate instructor entries using the instructor identifier (e.g., prof field).
Identify how many instructors appear more than once.
Compute the overall average age and standard deviation using all observations.
Then filter the dataset so that each professor appears only once.
This reduces the dataset to 94 unique instructor observations.
Recalculate the mean and standard deviation of age using only the unique instructors.
Description
The goal is to compare how age statistics change when duplicates are removed.
If an instructor appears many times (teaching multiple sections), their age is repeatedly counted.
Removing duplicates gives a more accurate picture of the true instructor population.
Differences between the two sets of statistics indicate how repeated instructors influence the results.

Question 2 — Determine if Lower-Division Courses Receive Higher Evaluations (Bar Chart)
Workflow
Split the dataset into:
Lower-division courses (introductory courses)
Upper-division courses (advanced courses)
Compute the average teaching evaluation score for each course level.
Create a bar chart to compare the two average values visually.
Interpret the bar heights to determine which group receives higher scores.
Description
Lower-division courses often involve beginners who may evaluate instructors differently.
If the bar for lower division is higher, it suggests:
"Lower-division courses receive higher teaching evaluations."
This visual comparison helps quickly identify differences in perceived teaching effectiveness across levels.

Question 3 — Plot the Relationship Between Age and Teaching Evaluation
Workflow
Treat age as the independent (explanatory) variable.
Treat evaluation score as the dependent (response) variable.
Use a scatterplot to map age on the x-axis and evaluation on the y-axis.
Look for:
upward trend
downward trend
no pattern
Description
This visualization helps reveal whether older or younger instructors tend to receive different ratings.
Possible patterns:
Positive slope: Older instructors receive better evaluations.
Negative slope: Younger instructors rate higher.
No clear slope: Age does not influence evaluations.

Question 4 — Gender-Differentiated Scatterplot (Age vs Evaluation)
Workflow
Plot the same age–evaluation scatterplot.
Differentiate the observations by gender (e.g., male vs female).
Use:
different colors
different markers
(visually distinguishing gender groups)
Description
This visualization reveals whether the relationship between age and evaluations differs between males and females.
For example:
Female instructors may show a stronger upward trend with age.
Male instructors may show a flatter or declining pattern.
Overlapping clusters may indicate similar ratings across genders.
This helps identify whether gender influences evaluation patterns when age is considered.

Question 5 — Scatterplot Differentiating by Gender and Tenure
Workflow
Plot a scatterplot with:
age on the x-axis
evaluation score on the y-axis
Separate data points using:
different colors for gender
different shapes or sizes for tenure (yes/no)
Create a combined visualization showing 4 groups:
Male, tenured
Male, non-tenured
Female, tenured
Female, non-tenured
Description
This is the most detailed scatterplot. It answers questions such as:
Do tenured instructors receive higher evaluations?
Does gender influence evaluations differently for tenured vs. non-tenured faculty?
Does age interact with tenure or gender in affecting evaluation scores?
Such a plot reveals complex multi-factor relationships among age, gender, tenure, and evaluation performance.
