# ASSIGNMENT: Sampling and Reproducibility in Python

Read the blog post [Contact tracing can give a biased sample of COVID-19 cases](https://andrewwhitby.com/2020/11/24/contact-tracing-biased/) by Andrew Whitby to understand the context and motivation behind the simulation model we will be examining.

Examine the code in `whitby_covid_tracing.py`. Identify all stages at which sampling is occurring in the model. Describe in words the sampling procedure, referencing the functions used, sample size, sampling frame, any underlying distributions involved, and how these relate to the procedure outlined in the blog post.

Run the Python script file called whitby_covid_tracing.py as is and compare the results to the graphs in the original blog post. Does this code appear to reproduce the graphs from the original blog post?

Modify the number of repetitions in the simulation to 100 (from the original 1000). Run the script multiple times and observe the outputted graphs. Comment on the reproducibility of the results.

Alter the code so that it is reproducible. Describe the changes you made to the code and how they affected the reproducibility of the script file. The output does not need to match Whitby’s original blogpost/graphs, it just needs to produce the same output when run multiple times

# Author: SIM ONG

```
IDENTIFYING STAGES OF SAMPLING

Infect a random subset of people
    Sampling procedure: Simple random sampling
    Sampling frame: 1,000 people in a community, in a single time period
    Sample size: 100 people

    Functions used:
        The choice() function is used to randomly select units in the sampling frame to infect with the specification that only 10% of the sampling frame is infected.
        The int() function is nested within choice() to ensure that the number of randomly chosen units is an integer.
        The len() function is nested within int() to refer to the number of rows of the ppl dataframe.

    Underlying distribution: Deterministic allocation

    Here, Whitby is creating his frame population with the supposition that "exactly 10% of people at every event are infected, regardless of the type of event."



Primary contact tracing: randomly decide which infected people get traced
    Sampling procedure: Simple random sampling
    Sampling frame: 100 people in the community who are infected
    Sample size: Less than 20 people

    Functions used:
        The rand() function is used to randomize the number of units in the sample with the specification that it is less than 20% of the sampling frame.
        The sum() function is nested within rand() to specify that the number of units in the sample is the thing to be randomized.
    
    Underlying distributions: Bernoulli

    Here, Whitby narrows his sampling frame. He supposes that "an infection has only a 20% chance of being traced to a source event" given that "contact-tracing is imperfect" due to factors like the inaccurate recall of infected people, etc.

    

Secondary contact tracing based on event attendance
    Sampling procedure: Cluster sampling (one-stage)
    Sampling frame: Set of events attended by set of the traced individuals
    Sample size: Events with at least two traced individuals

    Functions used:
        The value_counts() function is used to count the frequency of the types of events attended by those in the sample.
        The isin() method is then used to check the number of infected people who are traced in each cluster.

    Underlying distribution: Depends on the previous stage of contact tracing

    "If two infections are independently traced to the same source event, a special effort is made to test every person who attended that event, with the result that 100% of infections associated with that event are identified."



COMPARING GRAPHS
In the generated graph, the proportion of cases in "Infections from Weddings" (blue) seems to have a normal distribution. Most of the proportion of cases in "Traced to Weddings" (red) seems to be normally distributed with the exception of a number of cases falling in the 0.00-0.05 range.
As such, the script generates a graph that is vaguely similar but not identical to the graph in the original blog post.

After modifying the number of repetitions in the simulations to 100 and running the script multiple times, it's clear that the outputted graphs are different each run. As such, the script is not reproducible.



MAKING THE CODE REPRODUCIBLE
# Altering code to make it reproducible: Set the seed
np.random.seed(123)
    I used the np.random.seed() function to set the seed for generating the random numbers in the script. The results of my chosen seed value 123 are reproducible across multiple runs, and the graphs generated are identical to each other.


```


## Criteria

|Criteria|Complete|Incomplete|
|--------|----|----|
|Altercation of the code|The code changes made, made it reproducible.|The code is still not reproducible.|
|Description of changes|The author explained the reasonings for the changes made well.|The author did not explain the reasonings for the changes made well.|

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 09/04/2025`
* The branch name for your repo should be: `assignment-1`
* What to submit for this assignment:
    * This markdown file (a1_sampling_and_reproducibility.md) should be populated.
    * The `whitby_covid_tracing.py` should be changed.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-1`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
