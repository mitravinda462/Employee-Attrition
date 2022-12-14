# Employee-Attrition

**Introduction**

Amongst the many traits of an organization that attract prospective employees, the attrition rate plays a pivotal role. Attrition, to put it simply, is reduction in a company’s workforce. This may be voluntary (through resignation) or involuntary (through termination). There can be several reasons behind voluntary attrition, such as low pay, stagnancy in job roles (infrequent promotions), personal reasons such as health or familial issues and so on. The problem of employee attrition, if left unchallenged, can be detrimental to the company not only because of the loss of well-trained employees, but also the additional expenses of recruiting new employees and training them. Another crucial side-effect of attrition is its effect on the quality of products and services delivered by the company; ensuring quality is non-negotiable. Thus, there is a need for an efficient and accurate system to predict employee attrition and contributing factors which can be worked upon by employers to curb it. The primary objective of this project, which sets it apart from existing research on its subject matter, is to provide recommendations for what a company can do to retain any particular employee, based on the causes of attrition for employees with similar work lives and the recommendations suggested for retaining them. This way, rather than only predicting how likely the attrition is, we also predict why it happens and what can be done to prevent it.

**Dataset**

The IBM HR Analytics Employee Attrition & Performance dataset was used. It comprises of 35 attributes for 1470 employee records, ranging from descriptive attributes such as gender, age and marital status to attributes directly related to employment such as work life balance, overtime, monthly income and so on.

**System Design**

![emp-att-syst-design1](https://user-images.githubusercontent.com/53876415/205435265-644bbb51-2dbd-4c04-9e4d-51d3dd5308e3.jpg)

**Prediction**

A prediction model was built to predict the susceptibility of employees attrition. As a first step, 80% of the dataset was partitioned into a training set and the remaining 20% was partitioned for testing. The column ‘Attrition’, whose binary value specified whether or not attrition of the employee took place, was considered as the target column. Various classifiers were implemented, such as:
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. K-Nearest Neighbours (KNN)
5. AdaBoost
6. XGBoost
7. Gradient Boosting

**Recommendation**

A recommendation system was built for providing the employer with recommendations of how attrition can be prevented for a newly input record of an employee. The causes
for attrition and recommendations provided for the new record are identified through other most similar employee records using SHAP index and user-based collaborative filtering technique.
