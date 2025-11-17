1. Calculate the percentage of visible minority professors who are tenured
Workflow
Identify variables:
visible minority variable (usually coded as 0 = No, 1 = Yes)
tenure variable (0 = Not Tenured, 1 = Tenured)
Filter dataset:
Select only the instructors who belong to visible minorities.
Compute counts:
Count how many visible minority instructors exist.
Count how many of them are tenured.
Calculate percentage:
Percentage=Visible minority + Tenured/Total visible minority × 100
Interpretation:
Compare the percentage with the overall tenure rate.
If visible minority professors have a much higher or lower tenure rate, then tenure differs by visible minority status.

2. Compare average age by tenure
Workflow
Split dataset by tenure group:
Group 1: Tenured professors
Group 2: Untenured professors
For each group, compute:
Mean age
Standard deviation of age
Interpret meaning:
If means differ significantly, age and tenure may be associated
(older professors tend to be tenured because tenure is achieved over time).

3. Choose the best graph for age and plot it
Workflow
Understand data type:
Age is a continuous numeric variable.
Suitable graph options:
Histogram
Boxplot
Density plot
Choose best:
A histogram shows frequency distribution clearly.
A boxplot is best for comparing age across groups.
If only one variable is studied, the histogram is the best choice, because it shows shape, spread, and central tendency.
Plot description:
X-axis: Age
Y-axis: Frequency
Show 10–12 bins to visualize distribution.

4. Difference between pyplot.bar and pyplot.barh + graph for gender
Theory Description
pyplot.bar
Creates vertical bars
X-axis: categories
Y-axis: numerical values
Best when category names are short or few
pyplot.barh
Creates horizontal bars
X-axis: values
Y-axis: categories
Best when category names are long or many
Workflow for plotting gender distribution
Count number of male and female instructors.
Choose bar chart because gender is a categorical variable.
Represent gender on the x-axis and number of instructors on the y-axis.
Compare heights of bars to interpret gender distribution.

5. Find the median evaluation score for tenured professors
Workflow
Filter data:
Keep only rows where tenure = 1.
Select the evaluation variable:
Usually named eval, teaching_eval, or evaluation.
Compute the median:
Arrange values in ascending order.
The value in the middle is the median.
If even number of observations, median is the mean of the two center values.
Interpretation:
Median shows the “typical” teaching score unaffected by extreme ratings.
