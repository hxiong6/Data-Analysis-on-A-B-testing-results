# Data-Analysis-on-A-B-testing-results

The objective of this project is to analyze the A/B testing result from an ecommerce website new UI experiment: **does the new UI design lead to a better conversion rate?**

(Diaclaimer: this is a school project based on  simulated data set)

- Performed exploratory data analysis (EDA) for preliminary data quality check 

- Proposed hypotheses regarding the causes of conversion rate drop in the test group

- Examined experiment bias using decision tree algorithm to automate the experiment data quality check, identified the states having issue with randomization 

- Re-did Welch’s T test on remainder dataset and results showed no stats sig difference between groups

- Proposed business recommendation regarding the implementation of the new UI

1) examine if the randomization is done right for the two 'problematic' states;

2) if no, then we can try **rebalancing** the data with adjustments or propensity score matching, and re-do the t-test on balanced data for NC/IN.

3) We don't have treatment data for PA, and PA is the one of the key states (highest conversion rate in the test group) in our customer base. We need to re-do the experiment in a correct way for PA.

4) based on the welch's t test result, **there exixts no significant difference b/w the new and old UI in terms of conversion rate (group by state)**, we can therefore make business decision based on other considerations, i.e., cost of replacement, code base maintenance, long-term consideration such as acquisition, branding.
