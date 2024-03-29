<h> A/B Testing/h>

<ins>**Overview**</ins>
Also known as split testing, is a method of comparing two versions of a webpage or a feature of a user interface
to determine which one performs better. It involves showing the two variants (A and B) to similar visitors at
the same time to see the version that gives a better conversion rate.

<ins>**Data Structure**</>
The data follows the schema below
+Silver: The cleaned data ready for analysis
+Gold: Anaylzed data showing findings

The bronze data consists of two tables(cvs files): and orders table

**Table 1: Converion informtion**
+user id(text): unique identifier for each user
+test group(text): user assigned to in an A/B test "converted" indicates the user completed a desire action
+total ads(int): the number of ads the user was exposed to

**Table 2: Conversion time**
user id(text):unique identifier for each user
most ads day(text): the day when the user saw the most ads
most ads hour(timedate): the hour during which the user was exposed to the highest number of ads

<ins>**Code Desription**</ins>
The idea of the dataset is to analyze the groups, find if the ads
were successful, and if the difference between the groups is statistically significant.
