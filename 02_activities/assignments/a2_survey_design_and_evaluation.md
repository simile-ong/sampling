# Assignment: Questionnaire Design and Sample Evaluation

## Requirements

The goal of this assignment is to practice developing and evaluating sampling materials.

### Part A - Survey Design:

Select one of the scenarios below and design a survey to meet the need(s) outlined in the prompt.

1.	In two to three sentences, describe the purpose of your survey
2.	Describe your target population, sampling frame, sampling units, and overall sampling strategy.
3.	Write a 5-10 question survey to address your chosen scenario below.

##### Scenarios
1.	You work in the Human Resources Department at a large tech company. Over the past few months, the company has been experiencing a high turnover rate across many of its departments, specifically within the entry- and lower-level positions. The company wishes to understand why this turnover is happening, and what changes need to occur to improve employee satisfaction.
2.	You work for a Canadian national political party during a federal election. Throughout the campaign period, your party has seen relatively high approval ratings, but an opposing party is also polling favorably and may still have a chance to win the election. You are one month away from the election and you want to understand what voters want from your party and its leader in order to maintain your lead and eventually win the election.
3.	You are a student researcher in the sociology department at the University of Toronto. You are working on a research project that concerns the relationship between music taste and age. This involves both comparisons between different people of different ages and comparisons of the same individual at different ages during their lifetime. You wish to understand to what extent age influences music taste, specifically as it relates to perceptions of popular music. Your results will be written into an academic paper that you hope to publish.

### Part B - Survey Evaluation:

For the **Canadian General Social Survey on Giving, Volunteering, and Participating, 2018 (cycle 33)**, conducted by Statistics Canada find any and all available documentation for the data gathered and identify and describe the survey features indicated below.
1. Sample type
2. Sample size
3. Target population
4. Sampling frame
5. Survey mode(s) 
6. Timeline
7. Response rate
8. Weights
9. Data processing
10. Cleaning, imputation, etc
11. Sources of error
12. Limitations, known biases, etc
13. Link to documentation and any additional sources used



# Your Changes

## Part A - Survey Design: 

The number of your chosen topic: `#1 -- HR Department at tech company`

Describe the purpose of your survey:
```
The purpose of the survey is to determine the cause of the high turnover rate among employees working entry- and lower-level positions across all departments.
Additionally, the survey seeks to understand what changes could be implemented to increase employee satisfaction and promote retention rates.
```

Describe your target population, sampling frame, sampling units, and observational units:
```
Sampling strategy: Multi-stage stratified sampling
    Obtain a list of target population
        HR should have a comprehensive list of every employee's employment history and salary.
        The company could have an idiosyncratic way of defining "entry-level" and "lower-level" positions, so we can filter the comprehensive list by metrics like job title, years worked, salary, etc. to identify the subset of entry- and lower-level employees.

    The survey questionnaire will be emailed to select entry- and lower-level employees since it is presumably not feasible to survery every one of them in a large company.
        Stratified sampling with be used to select the entry- and lower- level employees who will be invited to fill out the survey.**
        The entry- and lower- level employees will be divided into strata based on departments, and then divided again into sub-strata based on job rank and/ or salary range.
            This will ensure that employees from every department, and employees of different ranks and/ or salary ranges are fairly represented in the sample.
        A predetermined number of employees from every sub-stratum will be randomly selected to complete the survey.
            If departments are of relatively equal size, then the same number of individuals will be selected from each stratum.
            If departments vary drastically in size, then proportional or optimal allocation can be used to determine the percentage of each stratum to be selected.
            The same process can be used to determine the number of individuals to be selected so as to avoid over- or under-representation.

    The survey will be anonymized to encourage respondents to be as honest as possible.

Target population: All entry- and lower-level employees
    The prompt specifies that a high turnover rate is observed "specifically within the entry- and lower-level positions," so the employees who aren't in these positions will be excluded from the target population.

Sampling frame: All entry- and lower-level employees
    The sampling frame should ideally "perfectly coincide with the target population." (Source: https://www.theanalysisfactor.com/target-population-sampling-frame/)
    Since HR has a comprehensive list of all employees, it should be possible to include all entry- and lower-level employees in the sampling frame.

Sampling units: Randomly selected entry- and lower-level employees from each stratum (department) and sub-stratum (job rank/ salary range)

Observational units: Randomly selected employees


** This strategy assumes and hinges upon every selected employee filling out the survey. If the response rate is low among those selected for the survey, we won't be able to conduct a representative survey.
If it were feasible, the survey should be sent to all entry-level and lower-level employees. This could expand the sampling frame.
Once the results of the survey have been collected, the results could be stratified or clustered based on the respondents' departments.

```

Your 5-10 question survey:
```
0. Please fill out personal data (department, job title, number of years working in the company, salary range) -- Dropdown menus
1. How often do you look forward to reporting to work every day? -- Scale of 1-5, with 5 meaning "Always"
2. How content do you feel while you are at work? -- Scale of 1-5, with 5 meaning "Extremely content"
3. Do you enjoy working with most of your colleagues? -- Scale of 1-5, with 5 meaning "Enjoy immensely"
4. Do you enjoy working under your manager? -- Scale of 1-5, with 5 meaning "Enjoy immensely"
5. Do you feel like your workload is manageable? -- Scale of 1-5, with 5 meaning "Extremely manageable"
6. Do you feel like you are fairly compensated for the work you do? -- Scale of 1-5, with 5 meaning "Generously"
7. [If the employees often/ always work onsite] Is your office a conducive space to work? -- Scale of 1-5, with 5 meaning "Extremely conducive"
    [If the employees predominantly/ can freely choose to work remotely] Would working onsite alongside your colleagues and manager make your work more enjoyable? -- Scale of 1-5, with 5 meaning "Definitely"
8. Are you satisfied with your position in the company? -- Scale of 1-5, with 5 meaning "Extremely satisfied"
9. Can you envision yourself working for the company for a long time? -- Scale of 1-5, with 5 meaning "For my entire career"
10. What would enhance your experience at the company the most? -- Select all that apply with options like higher pay, improved workspaces, flexibility to work-from-home, etc.
    Ideally, the question would allow respondents to type in their own responses as an option
    After selection, the respondent would have to rank the options

```

## Part B - Survey Evaluation:

Identify and describe survey features:

```
1. Sample type
Stratified sampling
    Stratification is done at the province/census metropolitan area (CMA) level

2. Sample size
    Expected: 24,000
        According to the source, field sample = ~ 50,000, number of invitation letters sent = ~40,000, expected number of questionnaire completions = 24,000
    
    Actual: 16,760
        Number of invitation letters sent X response rate = 40,000 X 41.9% = 16,760

3. Target population
    All persons 15 years of age and older living in the ten provinces of Canada, excluding full-time residents of institutions

4. Sampling frame
    One or several landline and cellular telephone numbers associated with the same address
        Phone numbers are obtained from the Census and various administrative sources with Statistics Canada's dwelling frame

5. Survey mode(s)
    Electronic questionnaire or CATI (computer assisted telephone interviewing)

6. Timeline
    Data collection occured from 2018-09-04 to 2018-12-28 (115 days)

7. Response rate
    41.9%

8. Weights
    a. Estimation weights
        i. The person weight for respondents that are not 'rejected' and are not volunteers is multiplied by a factor
            This is to adjust for the 'rejecting' of a proportion of respondents that are not volunteers
        ii. The weights were adjusted so that the weighted income distribution of GVP matched the 2017 CIS distribution by province
    b. Bootstrap weights

9. Data processing
    Social Survey Processing Environment (SSPE) set of generalized processing steps and utilities

10. Cleaning, imputation, etc.
    Edits were performed automatically and manually at various stages of processing at macro and micro levels:
        i. Family relationship were checked
        ii. Consistency of survey data was checked
        iii. Flow edits wee done, specifically for CATI data

    Imputation was carried out in nine steps:
        i. Personal and family income
        ii-iv. Formal volunteering variables in the master file
        v-vi. Informal volunteering variables in the master file
        vii-viii. Variables in the donation file and solicitation methods in the master file

11. Sources of error
    a. Sampling error
    b. Non-sampling errors
        i. Non-response bias
        ii. Coverage error
        iii. Response errors
        iv. Processing errors

12. Limitations, known biases, etc.
    a. Selection bias -- Households without phones or have phone numbers not included in the available frame represent a part of the target population that was excluded from the surveyed population
        The results are biased to the extent that the excluded population differs from the rest of the target population
    
    b. Coverage bias -- Sampling frame doesn't match the target population as a result of selection bias
        This is a known bias, but survey estimates were weighted to represent everyone in the target population including those not covered in the survey frame
        The process by which the 2018 frame was created is also an improvement from previous surveys (i.e. using several linked sources instead of random digit dialing strategies), mitigating the bias
    
    c. Non-response error -- Occurs at several stages of the survey
        This is a known bias and adjustments to survey weights were made to account for non-response

13. Link to documentation and any additional sources used
    https://www23.statcan.gc.ca/imdb/p2SV.pl?Function=getSurvey&Id=796234

```

## Rubric

-	All required components are present and complete **Complete / Incomplete**
-	Choice of sampling strategy for Part A is justified and related to survey purpose **Complete / Incomplete**
-	Information for Part B is complete and correct **Complete / Incomplete**

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 18/04/2025`
* The branch name for your repo should be: `assignment-2`
* What to submit for this assignment:
    * This markdown file (a2_survey_design_and_evaluation.md) should be populated and should be the only change in your pull request.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-2`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
