STAT 382
Spring 2025
Project 2
Problems
DUE DATE: FRIDAY, APRIL 18, 2025 by 11:59 PM on Gradescope
LATE DUE DATE: SUNDAY, APRIL 20, 2025 by 11:59 PM on Gradescope
with penalty of 10 percentage points per day late
For this project, you will be given some data regarding a sample of gym members. You will
conduct various types of analysis and summarize your results in a report. You should create
your report in RMarkdown. Your report should read like a professional report that could
be read by someone without an extensive statistics background. Answers should be given in
complete sentences and paragraphs. Graphs should be appropriately labeled. When statistics
are computed, include an explanation of what information can be determined from those values.
For the report itself, hide chunks of code where appropriate to make your output cleaner. Submit
both your Markdown file and the knitted code as a PDF document. (You may create an HTML
file, and when you open it, then Print to PDF.)
Submit both files to Gradescope.
When submitting Project 2, make sure you do the following things:
1. Use only methods used in this course. Code or responses from outside sources, including
AI, will be considered Academically Dishonest. Do not use AI to improve your grammar
or spelling.
2. Any outside sources should be properly cited. Geeks for Geeks and StackExchange (and
Chegg, CourseHero, AI etc) are not acceptable sources.
3. Clearly identify where each Task starts in your final document.
4. Knit your code to create a HTML file. Convert the HTML file to a PDF. Submit this
PDF.
5. Submit your .Rmd code (what you used to create the HTML file).
6. All values and graphs, not just code, needs to be provided in the PDF document. Values
as comments in the code will be ignored.
7. All values and code related to a particular task are in the region identified with that task
in the code or final document, and not elsewhere. For example, if you need to create a
table in Task 2, we don’t want to have to look in Task 4 to find the table.
8. All text and explanation written should be the “white space” in the .RMD document, and
not as comments in the code.
For example,
‘‘‘{r}
## DISCUSSION SHOULD NOT BE HERE.
‘‘‘
Discussion should be HERE
1
9. When stating hypotheses for regression and ANOVA analyses, make sure to state them
using symbols, not words. If you need to use certain symbols, you can write them out.
For example, write mu for µ; write tau for τ; write beta for β; write “not equal to” for ̸=.
Note that a phrase like “not all” is acceptable.
Part of these projects is to have you practice writing a report. If you were to hand this document
to your manager at work, they would want something that looks like a report, not just a bunch
of code without any output.
Unless the Task asks you to code something, we will be looking in your PDF file for your answer,
not the RMD file.
Dataset Information:
The data set gym2.csv contains data for a number of gym members. There is a header in the
dataset. The variables are:
Age - Age of the gym member.
Weight - Member’s weight in kilograms.
Height - Member’s Height in kilograms.
Max BPM -Maximum heart rate (beats per minute) during workout sessions.
Avg BPM - Average heart rate (beats per minute) during workout sessions.
Resting BPM -Heart rate at rest before workout.
Session Duration - Duration of each workout session in hours.
Calories Burned - Total calories burned during each session.
Workout Type - Type of workout performed (e.g., Cardio, Strength, Yoga, HIIT).
Fat Percentage - Body fat percentage of the member.
Water Intake - Daily water intake during workouts.
Workout Frequency - Number of workout sessions per week.
Experience Level - Level of experience, from beginner (1) to expert (3).
BMI - Body Mass Index
Gender - 1 if the member identifies as gender 1, 0 if they do not.
bmi class - A classificiation Body Mass Index based on CDC definitions
2
Tasks:
Task 1) Convert Workout_Type, Experience_Level, Gender, and bmi_class to factors in the data
frame. Make the factor ordered where appropriate. Include the code in your project but
you do not need to comment on it.
Task 2) Create a simple linear regression model to predict Calories_Burned using Workout_Frequency
as a predictor.
Your response should include a scatterplot of the data.
Your response should include checking the assumptions for linear regression (linearity,
normality, and equal variance). Continue with the analysis even if the assumptions
are not met. Note: For the normality check, we would like either a QQ Plot and/or
the Shapiro-Wilk Test.
In your analysis, perform a hypothesis test to determine if the independent variable
explains some of the variation in the dependent variable (complete with hypotheses,
p-values, decision, and conclusion).
Include the equation of the regression line, and the value of R2
.
Calculate and include the value of the Pearson correlation coefficient from the data.
Include an explanation of what the values of r and R2 tell you, whether you believe
there is a linear association, how well you believe the model fits the data, and why
you believe those things.
Conduct any hypothesis tests at a 6% significance level.
Task 3) Create a multiple linear regression model without interactions to predict Water_Intake
as predicted by Age, Fat_Percentage and Weight.
Your response should include checking that the assumptions for linear regression
are met (linearity, normality, equal variance, and independence. Yes, we know that
the dataset is not a time-series, but do the independence test anyway for practice).
Continue with the analysis even if the assumptions are not met.
In your analysis, perform a hypothesis test to determine if the independent variables
explain some of the variation in the dependent variable (complete with hypotheses,
p-values, decision, and conclusion).
Include the values of R2 and R2
adj in your report.
If any of the independent variables are involved, conduct a hypothesis test to deter-
mine which ones are important (complete with hypotheses, p-values, decision, and
conclusion). Explain how you decided which were important.
Conduct any hypothesis tests at a 3% significance level.
3
Task 4) In Project 1, we considered if Water_Intake varies by bmi_class. Conduct a One-Way
ANOVA test to see if the mean value of Water_Intake varies by bmi_class at a 4%
significance level.
Check that the assumptions for ANOVA are reasonably met (normality and equal
variance). Continue with the analysis even if the assumptions are not met. Describe
your results in a paragraph, including any relevant graphs.
In a second paragraph, describe the results of the test. Your paragraph should include
hypotheses tested, the p-value, the decision you made, and your conclusion. Your
conclusion should be understandable to a person with limited statistical knowledge.
If there is an effect, conduct a Tukey Test and describe what those results tell you.
If there is not an effect, explain why we would not need to conduct a Tukey Test.
Task 5) Conduct a Two-Way ANOVA test with interactions to test the effects of Workout_Type
and Experience_Level on the variable Calories_Burned.
Check that the assumptions for ANOVA are reasonably met (normality and equal
variance). Continue with the analysis even if the assumptions are not met. Describe
your results in a paragraph, including a bar chart of average calories burned for each
predictor.
In a second paragraph, describe the results of your test. Your paragraph should in-
clude hypotheses tested, p-values, the decisions you made, and your conclusion. Your
conclusion should be understandable to a person with limited statistical knowledge.
You do NOT need to create an interaction plot or conduct a Tukey test.
Regardless of whether you find interactions significant or not, you need to write a
statement whether or not you need to test for main effects and why for full credit. If
you find that you should test for main effects, conduct the appropriate tests.
Conduct any hypothesis tests at a 8% significance level.
4
