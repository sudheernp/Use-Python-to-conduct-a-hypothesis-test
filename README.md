# Data Analysis Projects

## Project 1: Hypothesis Testing for Department of Education

### Activity Overview
In this project, we continue the scenario from an earlier part of the course, where we are data professionals working for the Department of Education of a large nation. We are tasked with analyzing data on the literacy rate for each district in two of the nation’s largest states: STATE21 and STATE28. Due to limited resources, we can only survey 20 randomly chosen districts in each state. Our goal is to determine if the difference between the mean district literacy rates in these two states is statistically significant.

### Conducting a Hypothesis Test
#### Step 1: State the Null and Alternative Hypotheses
- Null Hypothesis (𝐻0): There is no difference in the mean district literacy rates between STATE21 and STATE28.
- Alternative Hypothesis (𝐻𝐴): There is a difference in the mean district literacy rates between STATE21 and STATE28.

#### Step 2: Choose a Significance Level
We will use a significance level of 5% (0.05) for this analysis.

#### Step 3: Find the P-Value
We will calculate the p-value using the `scipy.stats.ttest_ind()` function with the `equal_var` parameter set to False to account for unequal variances.

#### Step 4: Reject or Fail to Reject the Null Hypothesis
If the p-value is less than 0.05, we will reject the null hypothesis, indicating a statistically significant difference in mean district literacy rates between the two states.

### Conclusion
Based on our analysis, we have found a statistically significant difference in mean district literacy rates between STATE21 and STATE28. This information will assist the Department of Education in making decisions about distributing government funding to improve literacy.

---

## Project 2: Air Quality Analysis for Repair Our Air (ROA)

### Introduction
In this project, we work for an environmental think tank called Repair Our Air (ROA), which aims to improve air quality in America using the Environmental Protection Agency's Air Quality Index (AQI). We conduct hypothesis tests to guide policy recommendations for ROA.

#### Key Decisions Tested
1. **Metropolitan-Focused Approach**: We test if the mean AQI in Los Angeles County is statistically different from the rest of California.
2. **Regional Office Location**: We compare the AQI between New York and Ohio to determine if New York has a lower AQI.
3. **Policy Impact**: We investigate if Michigan's mean AQI is greater than 10, indicating potential impact from a new policy.

### Conducting Hypothesis Tests
- We use a 5% significance level for all tests.
- For two-sample t-tests, we use Welch's t-test with `equal_var` set to False to account for unequal variances.

### Conclusion
- Los Angeles County has a statistically different mean AQI from the rest of California.
- New York has a lower mean AQI than Ohio.
- We couldn't conclude that Michigan's mean AQI was greater than 10 at the 5% significance level.

### Findings for Management
We present the null and alternative hypotheses, conclusions, and p-values for each test to our manager. We also specify the type of test, whether it's one-tailed or two-tailed, and how we performed the t-test from stats.

### Communication with Stakeholders
For stakeholders, we convey the 5% significance level and our conclusions. We provide sample statistics for context, allowing stakeholders to understand the results effectively.

---

**Key Takeaways**
- Even with small sample sizes, we can make statistically significant conclusions.
- The Los Angeles mean AQI is statistically different from the rest of California.
- New York has a lower mean AQI than Ohio.
- We couldn't conclude that Michigan's mean AQI was greater than 10 at the 5% significance level.

**Communication with External Stakeholders**
We provide the significance level, conclusions, and sample statistics for each test to external stakeholders for a clear understanding of our findings.
