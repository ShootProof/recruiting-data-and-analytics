# Foreground Senior Data Engineer

Here at Foreground, we prefer to have a good idea of a candidate's technical experience and analysis skills before proceeding with portions of our recruiting process. We believe that the exercise below will illustrate a candidate's approach to working with technologies and methodologies that may be commonly used in our Data and Analytics Engineering team.

The data provided for this exercise is a sample derived from the ShootProof (a Foreground brand) database. ShootProof provides a SaaS-based platform designed to serve the business needs of professional photographers, including hosting their photos. Customers to the ShootProof platform subscribe to a plan; these plans are tiered based on the total number of photos which can be hosted. 

## Guidelines

-   This exercise should not take you more than 3 hours to complete. If your solution is taking longer, that's okay—be honest and let us know how long it took and why you think it took that long.
-   The data is provided in a raw csv format. You are welcome to use the DB of your choosing to ingest this data for querying and analysis.
-   Be as thorough as you wish.
-   All exercises are to be performed as if you were on the job.
-   Please include both the answer and the SQL code.
-   Any files (data or otherwise) outside of the previously mentioned .csvs should be ignored. These files represent data or content to support the interviewing of other roles, and using any other data source will provide incorrect results.
-   For each question, write out your thought process and any assumptions you might make. Visualizations are encouraged to support any insights given.

## ShootProof Data Definitions and Notes

**Customer** - A studio in a status of Active or Suspended, on a plan with a value > $0, and no longer in the trial period.

**Churn** - A studio that was considered a customer in the previous time period, that is no longer a customer. This can be the closing of the studio's account (status changes to fraud or cancelled), or the studio moves to a free plan.

**Trial Signup** - All studios start as a trial, the signup date is the same date the studio is created. They will either then convert to a paying customer, transitioned to a free plan, or suspended if the account has too many photos uploaded to qualify for the free plan (< 100 photos). 

**First-time Win** - A "first time win" is when a studio becomes a paying customer (starting a plan having a price >$0) for the first time.

**Return Win (aka Boomerang)** - At ShootProof, we call a customer a "return win" or "boomerang" when they:
1.  First, become a paying customer ("first time win"),
2.  Then churn (see above for logic),
3.  Finally, become a customer again.

**Note on ShootProof Plans** - ShootProof has offered many plans over time, and plans are currency-specific. Most like plans can be grouped based on the max number of photos they allow to be stored. See our website for our standard plan tiers: https://www.shootproof.com/plans

## Data Assessment

1.  What is the likelihood a studio will have the status of "suspended" sometime during their tenure?
2.  What is ShootProof's best time of the year for signups?
3.  Is there an evident worst time of year for churn? If so, when?
4.  How many studio have "boomeranged"?
5.  What is the likelihood a studio boomerangs during their tenure?
6.  When a customer converts (aka their "first time win"), what plan do customers typically start on? Is is fairly flat over our plan tiers, or are one or more significantly more popular than others?


## Deliverables

Submission for this exercise should include the following:
1. Text file including SQL for all answers to the SQL Assessment portion of the exercise.
2. Any visualizations or supporting design documents used to facilitate the answering of the questions above.
