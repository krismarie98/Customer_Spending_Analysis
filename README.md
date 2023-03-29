# Customer_Spending_Analysis
## Overview:
### For this project the goal was to create an analysis using customer spending data. Additionally, I wanted to try and create a machine learning mmodel to try and correctly predict the customer spending score (if the spending score was over or under 75 which was the 75th percentile). This data was a smaller data set just under 2000 data points. I did have to make some adjustments to the data and drop any null value and make sure there weren;t any duplicates. I also had an issue with the age column because the ages did not make sense. For example, the age of one customer would be listed as two years old but the profession would be a doctor. So I thought the easiest thing would be do drop the age column so it would not skew the data. I also got rid of the customer id column. The left over columns were the profession, work experience, annual income, gender, family size, and spending score. 
## The Process:
### The next step in making the data usable was encoding the data and changing the spending score column into are target value.The encoding process creating more columns and for both the non integer columns such as gender and profession column. With the spending score column I decided to to classify it and I used the describe function to gain some knowledge of the data. With that data I figured out what the 75th percentile was whcih happened to be 75 so I changed my spending score column to mark 1 if the row data was greater than or equal to 75 and 0 if not. This allowed me to create my machine learning model which I thought the random forest machine learning model would be best because of the amount of columns. Once that was done I created my model by first scaling the data and setting my x values or factors and my target values.
![image](https://user-images.githubusercontent.com/112527054/228586956-36852b27-6cc3-43c4-90db-dd103ac5f9ae.png)
## Results:
### Random Forest Model: For this model the accuracy was at 66%.
![image](https://user-images.githubusercontent.com/112527054/228593407-0468da67-f83f-4c1c-a398-3cc5b6de9fb7.png)
### Decision Tree Model: I also did this model to see if I could get better results but the changes were little at 57% accuracy.
![image](https://user-images.githubusercontent.com/112527054/228594420-be895c3f-1d7d-42fb-a757-2f618ee90538.png)
## Summary:
