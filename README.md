# Case-Study-3---Foodie-Fi
It's the 3rd Case study of 8 week SQL challenge of Data with Danny
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/00b67ec7-e4ef-499f-9436-67fbf9f661b8)
### Introduction:
Subscription-based businesses are super popular and Danny realized there was a large gap in the market - he wanted to create a new streaming service that only had food-related content - something like Netflix but with only cooking shows! 
Danny found a few smart friends to launch his new startup Foodie-Fi in 2020 and started selling monthly and annual subscriptions, giving their customers unlimited on-demand access to exclusive food videos worldwide!
Danny created Foodie-Fi with a data-driven mindset and wanted to ensure all future investment decisions and new features were decided using data. This case study uses subscription-style digital data to answer important business questions.

#### Available Data:
Danny has shared the data design for Foodie-Fi and also short descriptions of each of the database tables - our case study focuses on only 2 tables but there will be a challenge to create a new table for the Foodie-Fi team.
All datasets exist within the foodie_fi database schema - be sure to include this reference within your SQL scripts as you start exploring the data and answering the case study questions.

### ER Diagram:
![image](https://github.com/mausumi45/Case-Study-3---Foodie-Fi/assets/98810351/b5c7fa9b-1a33-43e7-b8c0-bc7eb172c69e)

### Table-1 (Plans):
Customers can choose which plans to join Foodie-Fi when they first sign up.
Basic plan customers have limited access and can only stream their videos and is only available monthly at $9.90
Pro plan customers have no watch time limits and are able to download videos for offline viewing. Pro plans start at $19.90 a month or $199 for an annual subscription.
Customers can sign up to an initial 7 day free trial will automatically continue with the pro monthly subscription plan unless they cancel, downgrade to basic or upgrade to an annual pro plan at any point during the trial.
When customers cancel their Foodie-Fi service - they will have a churn plan record with a null price but their plan will continue until the end of the billing period.

### Table 2(subscriptions):
Customer subscriptions show the exact date where their specific plan_id starts.

## Case Study Questions:
This case study is split into an initial data understanding question before diving straight into data analysis questions before finishing with 1 single extension challenge.

#### A. Customer Journey
Based off the 8 sample customers provided in the sample from the subscriptions table, write a brief description about each customer’s onboarding journey.

Try to keep it as short as possible - you may also want to run some sort of join to make your explanations a bit easier!

If customers downgrade from a pro plan or cancel their subscription - the higher plan will remain in place until the period is over - the start_date in the subscriptions table will reflect the date that the actual plan changes.

When customers upgrade their account from a basic plan to a pro or annual pro plan - the higher plan will take effect straightaway.

When customers churn - they will keep their access until the end of their current billing period but the start_date will be technically the day they decided to cancel their service.
