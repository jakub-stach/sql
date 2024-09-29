# Assignment 1: Design a Logical Model

## Question 1
Create a logical model for a small bookstore. 📚

At the minimum it should have employee, order, sales, customer, and book entities (tables). Determine sensible column and table design based on what you know about these concepts. Keep it simple, but work out sensible relationships to keep tables reasonably sized. Include a date table. There are several tools online you can use, I'd recommend [_Draw.io_](https://www.drawio.com/) or [_LucidChart_](https://www.lucidchart.com/pages/).

--uploaded as .png within the assignment as a single ERD with everything in it

## Question 2
We want to create employee shifts, splitting up the day into morning and evening. Add this to the ERD.

--done see in the single ERD

## Question 3
The store wants to keep customer addresses. Propose two architectures for the CUSTOMER_ADDRESS table, one that will retain changes, and another that will overwrite. Which is type 1, which is type 2?

_Hint, search type 1 vs type 2 slowly changing dimensions._

--added both kinds of architectures in there and showed them as 1 or 2, pick one that works best.

type 1 is the one that holds a single level of information (i.e. gets overwritten), type 2 retains change

Bonus: Are there privacy implications to this, why or why not?
```
Your answer...
```
with type 1 we hold less data about the customer's history which can be considered obtrusive in some cases 

## Question 4
Review the AdventureWorks Schema [here](https://imgur.com/a/u0m8fX6)

Highlight at least two differences between it and your ERD. Would you change anything in yours?
``` 
Your answer...
The AdventureWorks Schema is a lot more detailed, complex, and uses colours to separate different functional/conceptual areas of the DB. It also looks to have undergone some level of normalization, even in the case of sales, those are a lot more detailed with specific splits for things like taxes, currency, quotas, cc info and territories. 

If I had all the time in the world I would love to go through a project that designs and utilizes a db in a real world scenario. I've done some SIS mapping previously and it was quite challenging even for a small scale aspect of it so I imagine a large DB would take hours on hours of work. 
```

# Criteria

[Assignment Rubric](./assignment_rubric.md)

# Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `September 28, 2024`
* The branch name for your repo should be: `model-design`
* What to submit for this assignment:
    * This markdown (design_a_logical_model.md) should be populated.
    * Two Entity-Relationship Diagrams (preferably in a pdf, jpeg, png format).  --> please let me know if you'd like the alt for the addresses, I did them all in one place as alternateives
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sql/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `model-design`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via our Slack at `#cohort-4-help`. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
