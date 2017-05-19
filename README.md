# AB-Testing

 A-B Testing 
By Olivia Jonah May 17 2017 
=========== 
Experiment Design 
----------------- 
### Metric Choice 
> List which metrics you will use as invariant metrics and evaluation metrics here. (These should be the same metrics you chose in the "Choosing Invariant Metrics" and "Choosing Evaluation Metrics" quizzes.) 
> 
> For each metric, explain both why you did or did not use it as an invariant metric and why you did or did not use it as an evaluation metric. Also, state what results you will look for in your evaluation metrics in order to launch the experiment. 
#### Used metrics 
- **Invariant:** Number of cookies, Number of clicks 
- **Evaluation:** Gross conversion, Retention, Net conversion 
#### Selection reasoning 
#### Invariant Metrics 
- **Number of cookies:** This is a good invariant, since it is used as unit of diverse and the number of cookies assigned to the control and experiment groups should be random and approximately 
equal. 
- **Number of clicks:** Since clicks happen right before the experiment , the number of clicks shouldn’t be affected by the experiment. 
- **Click-through-probability:** This invariant is the number of unique cookies to click the 
"Start free trial" button divided by the number of cookies to view the course homepage , it is normalized for each group of users, and is highly correlated with two other metrics that I already using. 
####Evaluation Metrics 
- **Gross conversion:** This is important evaluation metric for our experiment, because it depends directly on number of enrollments. 
- **Net conversion:** Since the experiment aims at reducing the number of frustrated students and increase percent of paying users, this metric reflects the potential preservation of paying students who complete the course. 
####Unused Metrics 
- **Number of user IDs: this variant is not normalized so it won’t be a good pick and robust compared to cookies as unit of diversion in this experiment. 
- **Retention: Primary reason not to keep this metric is the high duration due to the required sample. We also are expecting retention to increase based on the numerator –( number of user IDs to make a payment) not decreasing by much and the denominator (number of user IDs to enroll in the free trial) to decrease. It has already been captured both in the via gross conversion and net 

conversion. With expected changes in the numerator and denominator, it would be somewhat complex to identifying the individual effect of each. Additionally, the unit of diversion (a cookie) is different from the unit of analysis (the denominator of retention, user IDs in a free trial). This can affect our experiment in size or length. 
#### Final decision making 
As will be shown later **Retention** is hard to use, because to measure it we need too much page views (more than 4m), which will take too much time. So, in this experiment I will only use **Gross conversion** and **Net conversion** as evaluation metrics. 
After the experiment, to be able to make the decision to accept the change the following must be true: 
- **Gross conversion:** Should significantly decrease (Number of trials should be lower) 
- **Net conversion:** Should not significantly decrease (Number of paying customers should not be lower) 
### Measuring Standard Deviation 
> List the standard deviation of each of your evaluation metrics. (These should be the answers from the "Calculating standard deviation" quiz.) 
> 
> For each of your evaluation metrics, indicate whether you think the analytic estimate would be comparable to the empirical variability, or whether you expect them to be different (in which case it might be worth doing an empirical estimate if there is time). Briefly give your reasoning in each case. 


###Calculating Variability Type of metric 

Distribution 

Estimated variance 


Probability 

Binomial(normal) 

P^(1-P^)/N 


