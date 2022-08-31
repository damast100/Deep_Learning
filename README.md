# Deep_Learning

### **Step 4: Write a Report on the Neural Network Model**

For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for AlphabetSoup.

The report should contain the following:


### **1. Overview of the analysis: Explain the purpose of this analysis.**

-We were provided data from a nonprofit organization that was used to create a neural network model to help predict the candidates that would be successful, based on features within the dataset, if funded by the nonprofit.


### **2. Results: Using bulleted lists and images to support your answers, address the following questions.**


#### Data Preprocessing

##### A. What variable(s) are the target(s) for your model?
	-The variable that was our target was the IS_SUCCESSFUL column which marked 1 for successful.
##### B. What variable(s) are the features for your model?
	-All of the other columns besides IS_SUCCESSFUL were our features columns.
##### C. What variable(s) should be removed from the input data because they are neither targets nor features?
	-The EIN and NAME columns were removed as they were not relevant to training the model.

#### **Compiling, Training, and Evaluating the Model**
##### **How many neurons, layers, and activation functions did you select for your neural network model, and why?**
![image](https://user-images.githubusercontent.com/100641752/187561869-4867e937-a1c4-466b-9a7e-268deaa20cb6.png)

##### Were you able to achieve the target model performance?
	-I was not able to achieve the target model performance of 75%
##### What steps did you take in your attempts to increase model performance?
	-I attempted three different times to change certain items within the model to optimize it. 
	-On all three attempts, I change the number of classifications and changed the nodes from 40 to 20 on the first hidden layer and 30 to 40 on the second hidden layer. 
	-On the first attempt, I also changed the epochs to 25 from 100. 
	-On the second attempt, I changed the classification numbers and nodes as indicated previously but changed the epochs back to 100. 
	-On the third attempt, I kept everything the same as the second attempt except I added a third hidden layer with nodes equal to 80.

### 3. Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
-The model worked best with on the first optimization with less epochs as it brought it up to 72.65% with only two hidden layers and using relu and sigmoid activations. I would recommend using a random forest model to help increase the model performance as it can handle large datasets and easier to understand.
