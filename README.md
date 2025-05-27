# AB_testing
AB testing  for my reference with the base outline and a bit detailed in depth analysis
we have a data set 
from kaggle
credits to kaggle
credits to Adarsh Anil Kumar for publising the Dataset in kaggel


Firstly Understanding data set

User ID	Group	Page Views	Time Spent	Conversion	Device	Location
14292	B	3	424	No	Mobile	Northern Ireland
11682	A	9	342	No	Mobile	Scotland
19825	A	2	396	No	Desktop	Northern Ireland
16080	B	4	318	No	Desktop	Wales
18851	A	1	338	Yes	Desktop	Scotland
this is the sample data set 
> converting the data to our use case
    > check for duplicates
    > standerdize the data
    > make data Usable
> now import the libraries 
manipulate
> compare two main groups A & B
> check for conversion (my KPI) then calculate the conversion rate and check for the difference if the Group A is better than B
   > Group A is the main data with the no changes made 
   > Group B is the the data we are getting by the changes we made 
now compare them 
if your results are better in Group B then you can use the new changes if the resuls are not good you have to fine new approch

in my case
--- Conversion Counts ---
Number of conversions in Group A: 136
Number of conversions in Group B: 349

--- Total Users per Group ---
Total users in Group A: 2519
Total users in Group B: 2481
Group A Conversion Rate: 5.40%
Group B Conversion Rate: 14.07%
Conversion Rate Difference (Group B - Group A): 8.67 percentage points
go with the new model 


Summary of Key Findings from the Analysis:

Conversion Rates:
Group A (Control): 5.40%
Group B (Variation): 14.07%
Conversion Rate Difference: Group B showed a significant improvement of 8.67 percentage points over Group A.
Statistical Significance: The Chi-squared test yielded a P-value of 0.0000, which is much less than the standard significance level (alpha = 0.05).
Conclusion: The difference in conversion rates between Group A and Group B IS statistically significant. This strongly suggests that the changes implemented in Group B genuinely led to the observed improvement in conversion.
