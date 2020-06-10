# Classification-Models
## Data
The German Credit Scoring Data consists of information about 1000 individuals. The first 20 variables are a mix of categorical and numerical variables, and act as independent variables for this data. The 21st column is a binary variable which indicates whether the customer defaults or not - this is the resultant variable. Value 1 of this variable indicates that the customer is likely to default on a credit payment.
## Goal and background
The objective of this analysis is to build a classification model with the best predictive power. We do so by fitting different predictive models onto the training and testing subsets of the dataset and evaluating the in-sample and out-of-sample performance of each model. The following models’ performances are compared:
•	General Linear Model
•	Tree model - CART
•	Advanced Tree Models - Random Forest, Boosting
•	Generalized Additive Model
•	Neural Network
The optimum probability in this case is given to us as 1/6 (equivalent to 5:1 asymmetric cost).
## Approach
We begin the analysis by an initial exploratory data analysis to get a preliminary understanding of the relationships among the different variables. The data is then split into 70% training data set and 30% testing data set (seed is set to 13480226 to facilitate reproducibility).
## Findings
<table>
<tr><td>Model	<td>In-sample MR<td>In-sample AUC	<td>OOO-sample MR<td>	OOO-sample AUC</tr>
<tr><td>General Linear Model <td>	0.32	<td>0.83<td>	0.3<td>	0.81</tr>
<tr><td>Regression Tree	<td>0.28<td>	0.83<td>	0.95<td>	0.73</tr>
<tr><td>Random Forest	<td>0.42<td>	0.78<td>	0.54<td>	0.78</tr>
<tr><td>Boosting	<td>0.36<td>	0.89<td>	0.31	<td>0.8</tr>
<tr><td>Generalized Additive Model	<td>0.42<td>	-	<td>0.43<td>	-</tr>
<tr><td>Neural Network	<td>0.42<td>	-	<td>0.24<td>	-</tr></table>
<br><td>General Linear Model (logistic model) is the most preferred predictive model for this dataset.
