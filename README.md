# Neural_Network_Charity_Analysis
## Overview 
With my knowledge of machine learning and neural networks, I used the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, I received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. With thise data, I will be able to do the following:

- Preprocess the data for the neural network model 
- Compile, train, and evaluate the model
- Optimize the model

## Results:

**Data Preprocessing:**
- What variable(s) are considered the target(s) for your model? "IS_SUCCESSMUL" variable
- What variable(s) are considered to be the features for your model? Every variable except "IS_SUCCESSMUL". The following: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT
- What variable(s) are neither targets nor features, and should be removed from the input data? "EIN" and "NAME"

**Compiling, Training, and Evaluating the Model**
- How many neurons, layers, and activation functions did you select for your neural network model, and why?

I had 2 hidden layers: 1 layer had 80 neurons and another layer had the second has 30 neurons
<img width="928" alt="Screen Shot 2021-12-29 at 8 59 19 PM" src="https://user-images.githubusercontent.com/88408350/147722928-2770ccfb-a197-4bc7-9ae8-60f513c176e1.png">

- Were you able to achieve the target model performance?

I was not able to achieve the target model performance of 75%. My accuracy score was ~73%
<img width="627" alt="Screen Shot 2021-12-29 at 9 02 06 PM" src="https://user-images.githubusercontent.com/88408350/147723024-f4b95d00-b284-4a77-82e1-dd88615627d3.png">

- What steps did you take to try and increase model performance?

I made 3 additional attempts of my model performance, but still could not reach the target model performance score of 75%.

Attempt #1: My accuracy score was ~72.9%

<img width="621" alt="Screen Shot 2021-12-29 at 9 04 38 PM" src="https://user-images.githubusercontent.com/88408350/147723191-b9c0450a-cdf7-42fd-84fc-55ffe47fef85.png">


Attempt #2: My accuracy score was ~72.7%

<img width="624" alt="Screen Shot 2021-12-29 at 9 04 52 PM" src="https://user-images.githubusercontent.com/88408350/147723194-e951fcd3-71b4-4954-8ba2-e0f5ae4fa434.png">


Attempt #3: My accuracy score was ~72.6%

<img width="621" alt="Screen Shot 2021-12-29 at 9 05 21 PM" src="https://user-images.githubusercontent.com/88408350/147723200-081c1c60-09f0-4136-a3e3-e04ef742a3d9.png">

## Summary:

The overall results of the deep learning model did not reach the target of 75% accuracy, but was close each time at about ~73%. AFter creating more neurons and hidden layers, our results did not get any closer to the target score probably due to overfitting. I recommend using a different model to solve this classification problem like the Random Forest Classifier by sampling the data to combine several decision trees. By doing so, this will give us a more accurate score to evaluate its performance against our deep learning model. The Random Forest Classifier does not overfit the data and can efficiently run on both smaller and larger datasets in a faster time. 
