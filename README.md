# Lead-Scoring-using-Logistic-Regression


The problem statement of the case study revolved around an education company named X Education that sells online courses to industry professionals.
X Education faced a problem of getting a lot of leads, but the lead conversion rate being very poor. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’.<br/>
X Education appointed us to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers.<br/>
Our end-goal is to build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads. A higher score would mean that the lead is hot, i.e. is most likely to convert and vice versa.
We began with inspecting the data given, doing the necessary conversions and perform missing value analysis on it. We dropped columns with more than 60% missing values.
We dropped many columns which were insensitive and did not show much variance in them. EDA of individual features helped us handle outliers and bucket insignificant categories into one. EDA also revealed some interesting findings such as which sources led to most lead conversions, what segment of people were more likely to get converted, and did more engaging websites get more leads.<br/>
We proceeded to do data preparation for logistic regression modelling, and performed Coarse tuning using RFE and narrowed the analysis down to top 15 features. We then used P-value and VIF for fine-tuning and cutting down on insignificant features.<br/>
On our final model of 13 features, we plotted the ROC Curve and visualize our model’s performance. To find the ideal cutoff we plotted multiple line plots of accuracy, specificity and sensitivity for different threshold values and found the intersection, and also considering sensitivity as our target metric, as we are ok if a uninterested aspirant is approached, but we can't afford to not approach interested candidates as we will be losing business, we chose a cutoff of 0.3.<br/>
With this Cut-off we used the trained model to Predict on the Test Set and compute different evaluation metrics such as precision, recall and accuracy. We ended with a sensitivity of 82.47%.<br/>
Learnings acquired:
- Feature Selection: Which to select and which NOT to? (Using both business intuition as well as EDA visuals.)
- Imputation Techniques: Which imputation will not disturb the data integrity? (Primarily business intuition and understanding was required to answer this)
- Modelling Metrics: RFE & P-value, VIF to narrow down on significant features.
- Metric Selection: Which metric serves our business purpose well? (Analysing our final goal)
- Assigning Lead Score: Presenting a list of potential hot leads to the sales team which in turn will boost the conversion ratio.
- Experience of solving an end to end business analytics problem, understanding segments and behaviour of aspirants, business KPIs and thought process to propose future course of action based on analytics.
