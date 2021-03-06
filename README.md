## Customer Segmentation using Cohort Analysis:

### Introduction: 
A cohort is a group of users sharing a particular characteristic. Strictly speaking it can be any characteristic, but typically the term cohort refers to a time-dependent grouping. For example, a typical cohort groups users by the week or month when they were first acquired. When speaking of groupings that are not time-dependent, the term segment is typically used instead of cohort.

#### Cohort Analysis:
Cohort analysis refers to tracking and investigating the performance of cohorts over time.

For example, if you wanted to see if users you’re acquiring now are more or less valuable than users you’ve acquired in the past, you can define cohorts by the month when they were first acquired. You can then run a cohort analysis to compare year-over-year revenue performance.

Cohort analysis is a subset of behavioral analytics that takes the data from a given data set (e.g. an EMRS, an e-commerce platform, web application, or online game) and rather than looking at all users as one unit, it breaks them into related groups for analysis. These related groups, or cohorts, usually share common characteristics or experiences within a defined time-span.

Cohort analysis allows a company to “see patterns clearly across the life-cycle of a customer (or user), rather than slicing across all customers blindly without accounting for the natural cycle that a customer undergoes.” By seeing these patterns of time, a company can adapt and tailor its service to those specific cohorts. While cohort analysis is sometimes associated with a cohort study, they are different and should not be viewed as one and the same. Cohort analysis is specifically the analysis of cohorts in regards to big data and business analytics, while in cohort study, data is broken down into similar group.

### Objective
The goal of a business analytic tool is to analyze and present actionable information. In order for a company to act on such information it must be relevant to the situation under analysis. A database full of thousands or even millions of entries of all user data makes it tough to gain actionable data, as that data spans many different categories and time periods. Actionable cohort analysis allows for the ability to drill down to the users of each specific cohort to gain a better understanding of their behaviors, such as if users checked out, and how much did they pay. In cohort analysis "each new group [cohort] provides the opportunity to start with a fresh set of users," allowing the company to look at only the data that is relevant to the current query and act on it.

In eCommerce, a firm may only be interested in customers who signed up in the last two weeks and who made a purchase, which is an example of a specific cohort. A software developer may only care about the data from users who sign up after a certain upgrade, or who use certain features of the platform.

### Types of cohorts
- Time cohorts: Deals with grouping customers performing certain activities in a specific time.
- Behavior cohort: Deals with grouping based on thier behaviour, for example buying a specific type of product or subscribing to a service
- Size cohorts: Depends on amount of Money/Time customer invest on a specific product.

#### In order to perform a proper cohort analysis, there are four main stages:

- Determine what question you want to answer. The point of the analysis is to come up with actionable information on which to act in order to improve business, product, user experience, turnover, etc. To ensure that happens, it is important that the right question is asked. In the gaming example above, the company was unsure why they were losing revenue as lag time increased, despite the fact that users were still signing up and playing games.
- Define the metrics that will be able to help you answer the question. A proper cohort analysis requires the identification of an event, such as a user checking out, and specific properties, like how much the user paid. The gaming example measured a customer's willingness to buy gaming credits based on how much lag time there was on the site.
- Define the specific cohorts that are relevant. In creating a cohort, one must either analyze all the users and target them or perform attribute contribution in order to find the relevant differences between each of them, ultimately to discover and explain their behavior as a specific cohort. The above example splits users into "basic" and "advanced" users as each group differs in actions, pricing structure sensitivities, and usage levels.
- Perform the cohort analysis. The analysis above was done using data visualization which allowed the gaming company to realize that their revenues were falling because their higher-paying advanced users were not using the system as the lag time increased. Since the advanced users were such a large portion of the company's revenue, the additional basic user signups were not covering the financial losses from losing the advanced users. In order to fix this, the company improved their lag times and began catering more to their advanced user


#### Prerequisites
- pandas library
- datetime objects
- basic plotting with matplotlib or seaborn
- basic knowledge of k-means clustering



## 2. Problem Statement
In this Data Tale, we will perform Time Cohort Analysis.
Time based Cohort analysis groups the customer by the time they completed their first activity.

The flow of this Analysis will be:
- Segment customers into cohorts based on the month they made their first purchase in.
-  We will then assign a cohort index to each purchase of all the customer. i.e we will mark each transaction based on that customers relative time period difference since his first purchase(Cohort he belongs to).
- Cohort Index assigned  will represent months since the 1st transaction of that particular customer.

- In the Last step, we will calculate various business metrics such as retention rate or Revenue Generated with respect to each Cohort and build a Cohort Chart using Heatmap to represent the results.

