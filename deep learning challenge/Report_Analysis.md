## Report Analysis

**1. Overview:** The purpose of this analysis is to evaluate the performance of the 
deep learning model that we utilized for Aphabet Soup.  Alphabet Soup is a nonprofit foundation consisting
of more than 34,000 organizations. At first, we apply some machine learning and neural networks to create a
binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. 

**2. Results:** 
* Data Preprocessing
    * The target variable is 'IS_SUCCESSFUL', which indicates whether a charity's application was successful or not. 
    * The remaining columns are considered as features
    * Columns / variables, such as 'EIN' and 'NAME', were dropped from the data.
        These variables are considered does not add any value to the target variable. 
* Compiling, Training, and Evaluating the Model
    * I selected two hidden layers. The first hidden layer has 80 nodes and uses the hyperbolic tangent (tanh) activation function. The second hidden layer has 30 nodes and uses the rectified linear unit (ReLU) activation function. The output layer is single node and uses the sigmoid activation function, which is suitable for binary classification problems.
![alt text](image.png)
    * Based on the above assumptions, the model performance resulted in approximately 73% accuracy. 
![alt text](image-1.png)

    * To improve the performance, I adjusted the number of hidden layers, the number of nodes per layer.  
    Moreover, I applied L2 regularization to prevent overfitting / high variance in the training data. This resulted to an improvement of approximately 79%.  
![alt text](image-2.png) 

**3. Summary**: To summarize, adding additional layers to the model improves its accuracy.  
Indeed, the more layers, the better the machine learning can predict better results. 
