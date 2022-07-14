# sql_projects

## Usage Funnels
*A funnel is a marketing model which illustrates the theoretical customer journey towards the purchase of a product or service.*

![funnels](https://user-images.githubusercontent.com/90055202/178894638-4b97598f-2368-488e-a829-010b5c5ac4b8.svg)

**1. Compare Funnels For A/B Tests**
A/B test:
- 50% of users view the original control version of the pop-ups
- 50% of users view the new variant version of the pop-ups
*How is the funnel different between the two groups?*

**onboarding_modals** table:
- user_id - the user identifier
- modal_text - the modal step
- user_action - the user response (Close Modal or Continue)
- ab_group - the version (control or variant)

**2. Build a Funnel from Multiple Tables**
The data is spread across several tables:
- browse - each row in this table represents an item that a user has added to his shopping cart
- checkout - each row in this table represents an item in a cart that has been checked out
- purchase - each row in this table represents an item that has been purchased

## Calculating Churn Rate
*The churn rate is a percent of subscribers at the beginning of a period that cancel within that period* (= the number of these users who cancel during the month divided by the total number).
**subscriptions** table:
- id - the customer id
- subscription_start - the subscribe date
- subscription_end - the cancel date
