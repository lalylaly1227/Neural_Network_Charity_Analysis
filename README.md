# Neural_Network_Charity_Analysis

# Overview of the analysis

From Alphabet Soup’s business team, a CSV file containing more than 34,000 organizations that have received funding from Alphabet Soup over the years to use for our analysis. This assignment consists of three technical analysis deliverables and a written report in an effort to develop a model that will accurately predict sound investments for the foundation. 

### Deliverable 1: Preprocessing Data for a Neural Network Model (also known as artificial neural networks, or ANN)

<img width="468" alt="Screen Shot 2022-09-29 at 7 49 35 PM" src="https://user-images.githubusercontent.com/105124485/193161574-2e0017f7-2ec4-4c43-925a-be3634169c94.png">

### Deliverable 2: Compile, Train, and Evaluate the Model

<img width="575" alt="Screen Shot 2022-09-29 at 7 50 09 PM" src="https://user-images.githubusercontent.com/105124485/193161609-2a7eab70-e7bb-4291-9982-a96678a44fae.png">

<img width="524" alt="Screen Shot 2022-09-29 at 7 49 57 PM" src="https://user-images.githubusercontent.com/105124485/193161599-1e7eb56f-8c3b-4536-9d83-864e6498230f.png">

### Deliverable 3: Optimize the Model

<img width="311" alt="Screen Shot 2022-09-29 at 7 48 42 PM" src="https://user-images.githubusercontent.com/105124485/193161643-2d68236f-cda1-4f4e-93c5-fce4c3fc0f2e.png">

<img width="533" alt="Screen Shot 2022-09-29 at 7 48 28 PM" src="https://user-images.githubusercontent.com/105124485/193161662-410a74d1-2373-4012-bc62-3fdc47557d7c.png">

### Deliverable 4: A Written Report on the Neural Network Model (README.md)

## Results 
Once I completed the Sequential model design, I will use the Scikit-learn model -> fit -> predict/transform workflow, which follows the same general steps across all of data science:
* Decide on a model and create a model instance. (For my optimization model I used the Random Forest model because it is able to achieve comparable predictive accuracy on large tabular data with less code and faster performance.
* Split into training and testing sets, and preprocess the data
* Train/fit the training data to the model
* Use the model for predictions and transformations.

o	Data Preprocessing
* Application_type seemed most valuable
* In the original model I removed the "EIN", "NAME" as the starter code suggested, but for my optimization model, I kept “NAME”

o	Compiling, Training, and Evaluating the Model
* For my original model I used nodes_hidden_layer1 = 80 and nodes_hidden_layer2 = 30
* I used activation code “relu” for both layers and “sigmoid” for the output layer.
* For my optimization model, I increased the number of layers and neuron units hidden_nodes_layer1 =  90, hidden_nodes_layer2 = 30, and hidden_nodes_layer3 = 10
* For my optimization model, I used the activation codes “relu” for the first layer and “sigmoid” for the other two layers and the output layer
* With the simple optimizations I did to the code, I was able to increase the accuracy level from 73% to 78%. Additionally, I reduced the epochs from 100 to 50, thus increasing the speed.

## Summary
Sometimes less is more.  I found that the Random Forest worked best with less code and more speed. At the same time with a greater degree of accuracy.
