## Neural Network Model for Alphabet Soup

1. Overview of the analysis: Explain the purpose of this analysis.

2. Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

- What variable(s) are the target(s) for your model? 

-- IS_SUCCESSFUL

- What variable(s) are the features for your model?  

-- The remianing columns after EIN and NAME are removed. The remaining columns contain valid informatiion to remain in the model

- What variable(s) should be removed from the input data because they are neither targets nor features? 

-- EIN and NAME

Compiling, Training, and Evaluating the Model

- How many neurons, layers, and activation functions did you select for your neural network model, and why?

-- I used 80 for the first layer and 30 for the second layer. Using boht relu in the 2 hidden layers and sigmoed for the output layer. I first selected 80/30 at the demenstrated respons from the starter coded indicated using this based on the output. I did however run at 8 and 3 as well and returned the same results. I did this to identify if we had oversampling. 

- Were you able to achieve the target model performance?

-- I was not able to achieve the target model performance of 75%. The max that I was able to get was 73%. 

- What steps did you take in your attempts to increase model performance?

-- As stated above, I had tried both 80/30 and then 8/3 both getting about that same performance. I tried multiple ways.  
I review the details of the columns and identified 2 of them that might be able to be removed. AFFILIATION and STATUS and with both we got better or worse even getting down to 65%. Changed the layers in multiple ways. Relu/Relu,  sigmoid/sigmoid, sigmoid/sigmoid/relu, linear/linear, even going into a 4rth layer. Change nuerons from 60/80/30, 80/30/30 and  80/60/30/40. The other items we tried to change was the Epocks from 50 up to 140.  See screenshots in the readme 

3. Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

--To Summarize the results of the deep learning model: In the model We used multiliple variations of nuarons, layers espochs and activations functions with most all of them coming between 73 and 73% accuracy and lossed between 55 and 60 at its worst.  We are looking to lower the losses. I would recommend that we evaluate the Data Qaulity and Quantity to give us more useful information to train the data. With more data it give more opportunities. Also, would try to to expirament with with different hyperparameters tuning to give more to find more optimal combinations. 