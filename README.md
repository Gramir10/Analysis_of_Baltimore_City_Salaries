# Analysis_of_Baltimore_City_Salaries
The midterm (Expanded) version of the my previous project. Through the sampling of employees from 2014 to 2019, we can create a predictive model to estimate future budgets.

Baltimore is known for many things such as its aquarium or quirky city culture, however, the unfortunate fact of the matter is that it's also a city known for its steady string of corruption scandals (enough to have its own archive even! https://baltimorefishbowl.com/stories/tag/corruption/). This begs the question, where is Baltimore City's funding going? Who's getting paid more than they should, and who should be getting paid more? How can we track systemic corruption between city departments?
How do identify which departments should be flagged for further review? In this analysis, we aim to answer these questions by investigating Baltimore City Salaries and how many employees in each department deviate significantly from their official salary, and by how much.</br>
</br>
# Identifying our initial population
Our goal is to check which departments have been over/under paying their employees. We will be using Baltimore City Employee Data from 2014, 2016, 2018, 2019. From this data, the parameters we're most interested in are: What was actually earned (Gross Salary), Person's Name, Person's Position/Title, What Department are they part of? </br>
From these parameters, we can now hone in on the population in the data that we're interested in investigating in. Using vlookup and several filters, we can now filter our population out by the following parameters:</br>
:white_medium_small_square: Person must X exist all 4 years (Name doesn’t disappear from the set)</br>
:white_medium_small_square: Person X must work all 4 years within the city</br>
:white_medium_small_square: Person X must not have a listed gross or annual salary of $0</br>
:white_medium_small_square: Person X must have been employed before May of 2013</br>
These parameters serve to filter out bad data points (individuals whos there is insufficient or incorrect data on, or individuals whos pay also accounts for a previous year's salary).</br>
With these filters in place, we have now defined our population and can now move onto the actual analysis of the data.</br>
</br>
# Data Analysis: Pinpointing the affected population
Now that we have our initial population, we now investigate the difference between Expected Pay vs Actual Pay. To define a significant difference from the actual pay, we check whether the individuals in each data point are either over or underpaid by at least a standard deviation. </br>
 
AVERAGE GROSS SALARY AS A FUNCTION OF AVERAGE ANNUAL SALARIES
![Alt Text](url_here)
ANY GRAPH DESCRIPTION/EXPLANATION

From here, we can now filter out the two populations we're most interested in via Pivot Tabes: The significantly overpaid population, and the significantly underpaid population.

TOTAL # OF OVERPAID EMPLOYEES BY DEPARTMENT
![Alt Text](url_here)
GRAPH DESCRIPTION

TOTAL # OF UNDERPAID EMPLOYEES BY DEPARTMENT
![Alt Text](url_here)
GRAPH DESCRIPTION

From both of these graphs, we can see that there is a large number of individuals in a wide variety of departments that are both over/underpaid. Overlaying these two graphs on top of each other, we get the following:

BALTIMORE'S OVERPAID, UNDERPAID, AND TOTAL EMPLOYEE COUNT(REMANING CITY DEPARTMENTS)
![Alt Text](url_here)

For clarity's sake, here is a final analysis of Baltimore's 6 largest departments:

From these final two graphs, we actually see that there isn't much overlap between groups in underpaid and groups in overpaid departments. Departments in Baltimore are generally one or the other.</br>
</br>>
Using this data, we can identify which departments are over/underpaid and should be flagged for review. This system could be using for cities other than Baltimore in the future, and it can also be implemented to monitor Baltimore's departments in the future.</br>
</br>
# Flaws in the Data

</br>
# Possible Future Expansions to this Project

</br>
# References
https://data.baltimorecity.gov/browse?category=City+Government

