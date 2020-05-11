## AB Test analysis. 
Author: Jose Maria Prieto for Data Analyst Udacity nano degree exercise
*****

### Introduction
project: A/B test run by an e-commerce website. Goal is to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.
*****
### Part I - Probability
Direct observations of the collected inputs
*****
### Part II - A/B Test
Run a hypothesis test continuously as each observation was observed.
*****
### Part III - A regression approach
result you achieved in the previous A/B test can also be achieved by performing regression.
*****
### Conclusions - Null hypothese not rejected. The new page is not capable of converting more
Along this excercise we try to analyse the collected data about in an AB test, that compare the old_page with the new_page. around half of the visitors has been exposed to one or the other version of the web and its convertions has been tracked on the data. Our mission has been to find significant influence (using a significance level of 0.05) on the convertion rates of the 2 pages in order to dictaminate the interest or not of this change.

Our null hypothesis (H0) has been that the old landing page has the same or higher convertion rate than the new page , and our alternative hypothesis (H1) has been that the old landing page has lower convertion rate than the new page.

We performed a preliminary observation of the 2 samples after cleaning the data, and afterwards an A/B test analysis using two different methods: simulating from the Null and calculating the Z-score. Both methods had same output: not possible to reject the null hypothesis, Hence, the landing page has not significant positive effect on the converted rate.

While using the regression approach based on a logistic model due to the binary nature of the variable of interest, the convertions, we´ve got a p-value which was different from the previous method, this was due to different null and alternative hypotheses (single vs double sided). Nevertheless, the output provided by the regression model agreed with the results in the A/B test.

As last validation, in order to ensure that the country variable is not distorting results, we've introduced the country of visitors, as an additional factor into the regression model. as per the results, landing page and country do not provoke significant changes on the convertion rate.

As general conclusion of this analysis, the change of the landing page as tested is not recommended, since it does not improve the existing one in terms of conversions.**Keywords**: python, probability, ab test, z score, p value, logistic regression
