# Telecom Service Quality Analysis

The telecommunications industry is a rapidly growing sector that is constantly evolving to meet the demands of consumers. As technology advances and user behavior changes, telecom operators face a variety of challenges that can impact their business success. In order to stay competitive and meet customer needs, it is important for telecom companies to regularly analyze their data to identify relevant problems and opportunities for improvement.

The aim of this project is to explore the telecom data and find relevant problems faced by telecom operators. By conducting an exploratory data analysis (EDA) on a large volume of telecom data, we can gain valuable insights into user behavior, network performance, customer demographics, and more. Through this analysis, we hope to identify potential areas for improvement, such as  improving customer satisfaction, optimizing network performance and increasing revenue through targeted marketing efforts.

The insights gained from this project can help telecom operators make informed decisions about their business strategy, enabling them to better meet the needs of their customers and stay competitive in the market.
 
## **Approach**

* Univariate Data Analysis:
    * Create histograms to visualize the distribution of the variables related to the hypotheses.
    * Use countplots to compare the frequencies of different categorical variables with respect to the hypotheses.
    * Create box plots to visualize the median, quartiles, and outliers of the continuous variables with respect to the hypotheses.

* Bivariate Data Analysis:
    * Create scatter plots to investigate the relationship between two continuous variables related to the hypotheses.
    * Create box plots to compare the distributions of the continuous variables with respect to the categorical variables related to the hypotheses.
    * Chi-Square Test and ANOVA:
        * Perform the chi-square test to evaluate the relationship between two categorical variables related to the hypotheses.
        * Use ANOVA to evaluate the difference in means between two or more groups related to the hypotheses.

* Multivariate Data Analysis:
    * Use correlation analysis to investigate the strength and direction of the relationship between multiple continuous variables related to the hypotheses.


* Project Summary:
    * Analyze the results obtained from the above tests to draw conclusions about the hypotheses.
    * Provide recommendations to improve customer satisfaction and retention based on the findings.
 
* Libraries Used:
    * NumPy
    * pandas
    * Matplotlib
    * seaborn
    * scikit-learn
    * Warnings
    * sys
 
## **Exploratory Data Analysis (EDA)**

### Univariate Analysis

![image](https://github.com/user-attachments/assets/888cd08c-ac90-4bc5-a57d-4f258a3c25b4)

Possible hypotheses that could be formed for "Age" colum are:
* Most customers fall in the age group of 20 to 40 years.
* There will be outliers present in the age column as some customers might have entered invalid age.

**Observation:** The data now seems to be valid as it also proves our hypothesis of most of the customer ages would be between 20-40. We also found maximum age as 9999 as outliers which were replaced later on.

### Bivariate Analysis

![image](https://github.com/user-attachments/assets/0fc47011-61d9-4da6-b748-00d5d1fe5afa)

* We can observe that January has the highest churn rate of 36.44%, followed by February with a churn rate of 16.57%. March has a churn rate of 14.84%, which is slightly lower than February. After that, the churn rate decreases steadily for the remaining months, with the lowest churn rate being in July with only 1.87%.
* This indicates that there may be some seasonal patterns in the customer churn rate, with the churn rate being highest during the first few months of the year and gradually decreasing towards the end of the year.

![image](https://github.com/user-attachments/assets/9e161b72-5782-487f-b705-7503eff550b8)

**Observation:**
* The distribution of churn reasons is quite similar, which makes it difficult to draw clear conclusions. However, there are a few observations we can make.
* The most common reason for churn is "Unknown," which could suggest that the company needs to do a better job of tracking and understanding customer behavior and reasons for leaving.
* Other common reasons for churn include price, service dissatisfaction, and network reliability, which could indicate that the company needs to focus on improving the quality of its service and offering competitive pricing to retain customers.
* The fact that many customers cited competitor offerings as a reason for leaving suggests that the company may need to do a better job of differentiating itself in the market.
* The presence of unusual reasons such as "43tgeh" with only 16 counts could indicate data entry errors or outliers that should be investigated and corrected.

### Multivariate Analysis

![image](https://github.com/user-attachments/assets/2ba8d9be-5b50-45ce-87b6-b735cdaa3f0f)

**Observation:**
* Based on the scatterplot, we can observe that the customers who have churned are mostly concentrated in the top left quadrant, where their satisfaction score is low but their average revenue per user (arpu) is high. This indicates that despite the customers generating high revenue, they are not satisfied with the service provided and hence are likely to churn.
* On the other hand, customers who are satisfied with the service and are less likely to churn are mostly concentrated in the bottom right quadrant, where their satisfaction score is high and their arpu is comparatively low.
* This information can be used by the telecom company to focus on improving the customer satisfaction score, as it is a key factor in retaining customers. They could analyze the reasons behind the low satisfaction score of high-paying customers and take measures to improve their overall experience. This could include providing better network coverage, offering customized plans, improving customer service, or providing incentives to loyal customers.


## **Project Summary**

In this project, we analyzed a telecom dataset with the aim of identifying insights and making recommendations for the business. We performed univariate, bivariate, and multivariate analyses to identify patterns and relationships between various variables. 

Through EDA, we identified that the company lacks targeted marketing for specific customers, satisfaction scores are low, and the major reasons for churn were attitude of customer support and competition offering better deals. 

### **Recommendations**:

* The company should focus on improving its customer support and services to reduce churn rates and increase customer satisfaction.

* The company should use the demographic and usage patterns of its customers to create targeted marketing campaigns that are more likely to resonate with specific customer segments.

* The company should consider offering incentives to customers who refer friends to use their services, as this can increase customer loyalty and bring in new customers.

* The company should explore ways to increase revenue from customers who generate less revenue, such as by offering targeted promotions or service upgrades.

* The company should continue to monitor its customer satisfaction score and take action to improve it.
