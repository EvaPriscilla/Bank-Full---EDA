# BANK-FULL---EDA
Sumber Dataset : https://drive.google.com/file/d/1dh1UrODNB4oWbap0J4WOWJJjkP217T7e/view?usp=sharing

The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be (or not) subscribed. 
## Features Descriptions
**Bank Client Data :**

1. age : age of the lead (numeric)
2. job : type of job (categorical: "admin.", "unknown", "unemployed", "management", "housemaid", "entrepreneur", "student", "blue-collar", "self-employed", "retired", "technician", "services") 
3. marital : marital status (categorical: "married","divorced","single"; **note: "divorced" means divorced or widowed**)
4. education : educational qualification (categorical: "unknown","secondary","primary","tertiary")
5. default : has credit in default? (binary: "yes","no")
6. balance : average yearly balance, in euros (numeric) 
7. housing : has housing loan? (binary: "yes","no")
8. loan : has personal loan? (binary: "yes","no")

**Related with the last contact of the current campaign:**

9. contact : contact communication type (categorical: "unknown","telephone","cellular") 
10. day : last contact day of the month (numeric)
11. month : last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
12. duration : last contact duration, in seconds (numeric)

**Other attributes:**

13. campaign : number of contacts performed during this campaign and for this client (numeric, includes last contact)
14. pdays : number of days that passed by after the client was last contacted from a previous campaign (numeric, -1 means client was not previously contacted)
15. previous : number of contacts performed before this campaign and for this client (numeric)
16. poutcome : outcome of the previous marketing campaign (categorical: "unknown","other","failure","success")

**Output variable (desired target):**

17. y - has the client subscribed a term deposit? (binary: "yes","no")
## Summary
After analyzing exploratory data on bank data, the following conclusions are obtained:
- We know that the number of clients who have subscribed deposits is 5289 with a percentage of 11.7% and the number of clients who do not subscribe deposits is 39922 with a percentage of 88.3%. Then it can be said that credit marketing has not been completely successful because when compared to customers who subscribe and do not subscribe, the comparison is so far.
- Based on numerical features with respect to y, the results obtained that numerical features have a weak relationship with y.
- Numeric features that affect y are **balance, duration, and days**.
- If you look at the distribution of the graphs on the category features, which can be said to have an influence on y are **default, job, loan, and marital.**
## Challenges
- Huge amount of data.
- Ambiguous meaning of columns of features.
