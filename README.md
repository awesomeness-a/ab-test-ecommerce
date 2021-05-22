# A/B Test Results Analysis 
This repository contains a project in which we analyze the results of an **A/B test performed by an e-commerce company**.
A/B tests are very commonly performed by data analysts and data scientists. It is important to get some practice working with the difficulties of these tests.

*The goal is to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision.*

In this project, we test the *alternative hypothesis* (the new webpage does convert better than the old webpage) against the *null hypothesis* 
(the new webpage converts about the same or worse than the old page).

In order to test our alternative hypothesis, we first perform the **sampling distribution** for the difference in conversion between the two pages over 10,000 iterations 
of calculating an estimate from the null. After that, we compute **z-statistics** using built-in z-test. 

Then, we use **logistic regression** approach to test if the new page conversion rate is not equal to the old page conversion rate. 

Finally, we add one more predictor into our model (country a prospect lives in), and we look at the individual factors of country and page on conversion, 
as well as at interaction between page and country, to see if there's significant effects on conversion.

## `ab_test_ecommerce.ipynb` 
This `Jupyter Notebook` file contains Python code of our data analysis process, step-by-step. The Python libraries used in the process are:
* Pandas
* NumPy
* Matplotlib
* Seaborn
