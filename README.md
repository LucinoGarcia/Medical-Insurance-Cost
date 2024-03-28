# Medical Insurance Cost: Project Overview
- 
- 
- 
- 
- 



# Resources 
**Python Version:** 3.10.12 <br>
**Packages:** NumPy, Pandas, Matplotlib, Seaborn<br>




# Data Collection
Dataset was on Kaggle under the title [Medical Insurance Cost Prediction](https://www.kaggle.com/datasets/rahulvyasm/medical-insurance-cost-prediction/data).<br>



# EDA
As can be shown below there is a severe under representation of samples with charges of over $20,000. This is reflective of what we expect to find in the real world but some outcome imbalance is likely to occur.<br><br>
![image](/images/Response_Histogram.png) <br>

The fact that the Linearity Check plot exhibits three quasi-linear patterns that run parallel to one another suggests that age is inexorably intertwined with one or more variables. It could also be posited that age will likely serve as some sort of sub-classifier into a 'tier of cost'. Decision Tree or Random Forest models are better equipped for handling such variables. <br><br>
![image](/images/Ages_Histogram.png) <br>

The other predictors suffered from skewed data but generally exhibibted potential for linear relationships with the response variable. For further insights and graphical representations, the [EDA notebook is found here](/Medical_Insurance_Cost,_EDA.ipynb).



# Model Building
Linear Regression, Decision Tree, and Random Forests were the three model candidates due to their ability to model both categorical and continuous data.


# Potential Implications
